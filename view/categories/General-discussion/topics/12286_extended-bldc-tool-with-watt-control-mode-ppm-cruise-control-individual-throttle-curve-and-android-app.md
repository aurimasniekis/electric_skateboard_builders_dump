# Extended BLDC-TOOL with Watt Control Mode, PPM Cruise Control, individual Throttle-Curve and Android App

### Replies: 1539 Views: 78310

## \#1 Posted by: Ackmaniac Posted at: 2016-11-01T22:46:40.004Z Reads: 2354

```
Hello

I want to represent my modified BLDC-Tool with modified Firmware.
The main goal of that modification is to have maximum possible control over the board. Because i didn't like that i can use only 50% of my throttle at higher speeds.
And the second big thought was to have cruise control via PPM with my mini remote. Just simply because it is possible.
And after a while of fine adjustment, i found out that also a throttle-curve adjustment is necessary to have full control for high power boards.

So here are the Features:

## **Watt control mode**

Finally, Watt Mode is made especially to give you much more control at higher speeds. At the beginning, you think the VESC has less power but then you learn that you simply have to pull the trigger a bit more. And when you start to carve at higher speeds you will definitely feel the difference. And another advantage is that when you set a watt limit (motor settings) the power feels the same over the whole battery capacity.

<img src="/uploads/db1493/original/3X/6/e/6e7b7520e037c4b2b86cc1c1b6fde9cf82cbfc2b.JPG" width="690" height="412">

**There are 3 new Control Modes for Watt Control:**

* **Watt no reverse with Brake** (recommended) (also exists for Nunchuk)
Depending on your "Motor max" and  "Battery max" settings you will loose throttle range at higher speeds in "Current Control". 
With Watt control, it has the advantage that it uses the entire throttle range at any speed. This makes the board more controllable especially when you like carving at higher speeds.
.
This works at every speed as long as the Motor settings allow this much Power at this speed. Of course, at close to max speed (motor KV) the efficiency of the motor can't produce that power anymore. But you can set the real maximum values in the motor settings and just define here how much power you want. So it is very easy to program a beginner mode with maybe 250 Watt.
.
The maximum Watts that can be reached are defined by the "Battery max" in the motor settings. You can calculate it by 3.6V a cell * cells in series * battery max. E.g. 10S4P battery with battery max set to 25A then you have 3.6V * 10S * 25A =  900 Watts. You can limit the maximum watts in the motor settings which explained further down in this post. If there is no limit set then it will calculate the maximum reachable watts by the actual Battery Voltage.
.
E.g. maximum reachable watts are 1000 Watt. Then 30% throttle will be 300 Watt, 50% throttle 500 Watt, 80% throttle 800 Watt and 100 % throttle 1000 Watt.

* **Watt** (also exists for Nunchuk)
"Watt" Control Mode works like "Watt no reverse with Brake" with the difference that you also have a reverse. The only problem with the standard reverse function is that when you brake hard the wheels can start to spin backward while you still move forward.
.
To avoid that i added the parameters "Enable maximum ERPM for direction switch"
.
<img src="/uploads/db1493/original/3X/8/c/8c742fee86c89c7232b03de809337feafae2b011.png" width="649" height="38">
.
When this is enabled and you brake hard then the brakes will work like in "Watt with no reverse". To drive backward you have to release the throttle and brake again. But this only works when you are below the ERPM (4000 in the picture). If you are above it will brake normally again.
When you drive backwards and you are above 4000 ERPM in the backwards direction then it will accelerate backwards and won't brake. If you are below 4000 ERPM backwards and you accelerated shortly to go forward and brake again then it will enable the normal brake again. To drive backwards you have to release the throttle and brake again.
.
How do i find the perfect ERPM for that parameter?_
The best is to go down a hill. Then do a full brake. You will see that the motors are not able at very low speed to stop the board from moving. If the value is set correct you can now release the throttle and brake again and the motors should start to accelerate backwards. If that is not the case then the value is too low. In my tests 4000 ERPM worked very well. For most setups that is like 4 km/h.
-
It sounds complicated but it becomes very intuitive after a short while. If you don't need it to go backwards then just simply use "Watt no reverse with Brake"

* **PID speed control no acceleration**
This mode is experimental, when you press the throttle then it only activates the Cruise Control and hold the speed. Brakes work as normal. So there is no acceleration. This might be good to legalize the board in some Countries.

## **Offset for Traction Control**
<img src="/uploads/db1493/original/3X/f/9/f976626f8d4743bf96bab97dce5dbb7070b82927.png" width="690" height="76">
Problem is that the standard firmware always reduces the power at one VESC when traction control is enabled. Because the RPM reading of the VESC is not very precise and can differ by +-400 RPMS. And that means that at 500 updates per second the Current for the VESC bounces a lot. Alos when you make do a curve then the inner wheel is slower than the outer wheel. So the outer wheel will get less power and by this it creates a power steering. To prevent this you can define an offset where the VESC should not reduce the power and deliver the same current to both VESCs. Above that offset, the normal traction control will step in. If you set this to 3000 for the most setups this will not enable traction control if the speed difference between both VESCs is lower than 3 km/h.So the traction control only reduces the power when it is really needed.

## **PPM pulse can be precisely adjusted by center position**
<img src="/uploads/db1493/original/3X/0/c/0c612707a83b1f4642698c3e7c4ec5b741d6e906.png" width="685" height="28">
This way the center position can be adjusted to the real value. And from that position the max throttle values for both directions can be adjusted. So you can use the whole throttle in both directions. With the standard firmware mostly not all the throttle range can be used in one direction. This again gives you more control and sensibility.
.
<img src="/uploads/db1493/original/3X/5/c/5c0f575f4ceed340bf45fff47dd44827ae2f300f.png" width="584" height="34">
.
If you don't know how to setup the Pulsewith values you can use the auto wizard which tells you what you have to do. before you use the wizard it is wise to disable the Control Mode first. Otherwise, the motors will start to spin (not really a problem).

## **Use Max Watts Limit**
To limit the maximum watts the motor will output you can do that in the Motor General Tab by enabling "Use max watts limit" and define a watt limit.
<img src="/uploads/db1493/original/3X/3/1/3191cd534d2e71f8ce2943cf26d9a520af85e795.png" width="690" height="413">
**IMPORTANT** you have to do this for **each motor** individually, Master and Slave.
If you set this value to 1000 then 25 % throttle will be 250 watts and 100% throttle will be 1000 watts. Of course, the throttle curve will have an influence. 
The battery max has the higher priority, So if the battery max is set to 10A and your battery has 36V then you can only produce 360W maximum. If you set the value to 1000 Watts then you can only use 36 % of your throttle because afterward the battery max blocks a higher power output.
So just make sure that the battery max allows the VESC to produce that many watts. You can also easily limit the VESCs power output with this parameter so that it would be very easy for the kids to ride the board.

## **Throttle Curve**
Here you can define the throttle curve. There are 3 different spots you can define along the throttle curve for braking and accelerating. 
When you change the values via the boxes then you will see the difference immediately in the Diagram. This is very intuitive and easy to understand.
Please always use the three values and don't try to set the values to the same value as another spot. That means don't set the same value for 2 or 3 boxes. Always choose values that make sense.
It works for the modes Watt, Current, PID and Duty Cycle. And also in watt reverse, if you use the ERPM limit.
And it only works for acceleration. Braking is the same as always.
<img src="/uploads/db1493/original/3X/4/9/49e9c17cdeae96c06f564d1327e6d5de1f183aa4.JPG" width="690" height="412">
Here you can see the results of the throttle curve adjustments.
.
The Y values are there to define how much % of the power should be used and the X values define at which throttle position.
So in the picture, you see that the brake curve is normal and the acceleration curve uses 
12.5% power at 25% throttle, 
30% power at 50% throttle and 
60% power at 75% throttle. 
With the Edge sharpness Factor you can make the curves rounder. But if you use crazy values then the curves might get stupid. So be careful what settings you use here. But you can always see what happens with the power output in the diagram.


## **Cruise Control for dual setups via steering channel connected to the second VESC:**

<img src="/uploads/db1493/original/3X/5/d/5dfc87f763d59036cbcf08b7c47b553b4b58468d.JPG" width="690" height="410">

At the slave Vesc the steering channel can be connected and in the PPM settings the "Cruise Control via Secondary Channel" can be activated. This enables the cruise control when the throttle is not pulled and the steering channel is turned more than 30% to left or right. In this mode braking is always possible, just to avoid stupid reactions in a shocking moment. And when you pull the throttle the cruise control will also be deactivated to avoid that the throttle is accidentally pulled while cruise control is active and then have a big surprise when cruise control is released. So i hope that i can avoid scary situations.
I recommend to set the Speed control settings in the Advanced tab to 0,00400 for KP and KI and leave KD to 0,00000. You can see my settings in the next screenshot
For cruise control the 2 VESC's need to be connected via can bus and the Slave VESC needs to send the status via can and the Master VESC needs to enable "Multiple ESCs over Can"

In the picture below you see that you have additional options when you use the steering to activate the Cruise Control.
You can define what should happen when the Pulsewidth is negative (lower than 50%) or positive (higher than 50%). If you use the motor settings the behavior will be like you set it up in the Motor advanced tab. Otherwise, you can define if you want to allow the speed controller that it can use the brakes if you go faster or not. 
For example it is possible when you steer right that cruise control ´doesn't brake when you are too fast and when you steer left that it dos use the brakes. This way you can use the cruise control for carving and downhill. 
<img src="/uploads/db1493/original/3X/1/2/129363912de80a95d8d05b12275c002811e173c0.jpg" width="476" height="162">

Hint: mostly when you steer right it gives lower signal and when you steer left it gives a higher signal.

## **Disable Breaking at Cruise Control**

<img src="/uploads/db1493/original/3X/b/5/b5938ec1b8bec3be74f74bd321913c0b7554917d.png" width="690" height="412">

You can disable the breaking at cruise control with the parameter "Braking allowed for Speed Controller" because it is very annoying when you want to carve at cruise control. Whoever tried it knows what i am talking about. The disadvantage is that when you want to maintain a constant speed downhill the cruise control will not brake if it is faster then the speed when you activated the cruise control.
BTW: I changed Cruise Control in BLDC mode from duty cycle Control to Current Control because it enables a much smoother ride. And when the breaking should be disabled at cruise control because you can really switch off the motors. In Duty Cycle Control there are always some small corrections with breaking which are disturbing.



So finally before i upload my code to Github it would be cool if anybody wants to give the whole changes a try. The modified BLDC-Tool only works in Ubuntu (No Windows). And you have to flash the VESCs with my modified Firmware because otherwise, the BLDC-Tool would not work.

I tested the modifications a lot and i didn't change any safety features of the VESC. So it should not blow up the VESC in any way. But of course, i don't give any warranty. So the testing is at your own risk. But i think there are some brave members here.

(Only for VESC Hardware Version 4.10 or higher. Actual Version 4.12 and VESC-X is fine.

If anybody wants to test you can download the files here.
[Windows BLDC-Tool, Modified Firmware, Ubuntu BLDC-Tool and Android app
](https://www.dropbox.com/sh/t7dl90owz5ccbyl/AAANyC-yQCMeveA7errNRnYqa?dl=0)

[App in Google Play Store](https://play.google.com/store/apps/details?id=ackmaniac.vescmonitor)

## Here are some additional install instructions. Read them before please:

Be aware that this is only for Hardware Version 4.10 or above (VESC-X as well).

Important: You have to flash the Firmware with this modified BLDC-Tool.

Open the downloaded BLDC-Tool
Upload (Flash) the new Firmware File "VESC_Ackmaniac_Mod_2_54.bin" which is available in the Dropbox link.
Adjust the settings of your VESC. I would not recommend to use a saved config. It would be better and safer to set the values manually. So you should make screenshots of your old setup or write it down.
It is always possible to flash back to Vedders original Firmware.

This Firmware has the Version 2.54. So don't be surprised by that. When you start the Modified BLDC-Tool the first time it tells you that the Firmware is not the same. So you have to flash it with my modified firmware. So no mistakes can happen anymore with the Firmware flash.

But please be careful when you test it. 
I take no responsibility if something goes wrong. If you don't except that then please don't use this software. 
**It is at your own risk.** 
Before you take the first ride test acceleration, braking and cruise control (if used) on the bench and at low speed to make sure everything works properly. 
**I don't want that anybody gets hurt.**

If you have trouble then let me know. And i really would appreciate some feedback.

**And if somebody wants to honor all the work. (many hundred hours)**
:point_down::point_down::point_down::point_down::point_down::point_down::point_down::point_down::point_down::point_down::point_down::point_down::point_down::point_down::point_down::point_down:
:point_right: **[Donations](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=GJ59FXYPUQHUY)** :money_mouth: **[Donations](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=GJ59FXYPUQHUY)** :money_mouth: **[Donations](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=GJ59FXYPUQHUY)**:point_left:
:point_up_2::point_up_2::point_up_2::point_up_2::point_up_2::point_up_2::point_up_2::point_up_2::point_up_2::point_up_2::point_up_2::point_up_2::point_up_2::point_up_2::point_up_2::point_up_2:

When you want to send a donation then don't use dots. (Germany uses commas). So use full numbers or a comma.

Or if you want to buy a Raptor 2 and want to save 100$ and support me with 100$.
[Raptor 2](http://www.enertionboards.com/raptor-2-direct-drive-electric-skateboard/?setCurrencyId=2&afmc=6q)
```

---
## \#2 Posted by: onloop Posted at: 2016-11-02T00:32:38.590Z Reads: 1560

```
WOW!.... this is awesome!

ill send you a VESCX beta for sure.
```

---
## \#3 Posted by: Ackmaniac Posted at: 2016-11-02T00:42:37.514Z Reads: 1524

```
Don't want to be unpolied but I would need 2 :innocent: because of the additional can bus communication and the cruise control signal over the slave VESC ppm channel. Only problem for you is that this would not support your nano-x because there is no second steering channel. But I think the reverse button could be modified for that. So if you have too many nano-x beta laying around feel free. :joy:
```

---
## \#4 Posted by: E-Boarding Posted at: 2016-11-02T07:54:13.753Z Reads: 1472

```
> This is another Watt control mode which only enables Cruise Control. 
> Acceleration is not possible. This way you have to push to gain speed 
> and when you pull the throttle cruise control will be activated with a 
> max power of the adjusted Watt. Breaking is always possible. (This was a
>  test to legalize the Longboard in Germany. Because acceleration is not 
> allowed. Only assistance to keep the actual speed might by OK.)

I'm waiting for this and would test it with a single drive but unfortunately I've to get Ubuntu first or wait for a Win-Version...
What's your experince, met some police? Do you have a video of the no acceleration-mode or something? Is it fun to ride?
```

---
## \#5 Posted by: Ackmaniac Posted at: 2016-11-02T08:26:18.964Z Reads: 1344

```
It is fun to ride. Like a mix of natural Longboarding and E-Longboarding. 
So you realize how much power your board produces. Other benefit is the less Wh usage which is in average at only half. Because no acceleration and not such high speeds. Other benefit is that you can adjust the Watts very accurate. Because in many country's they have a regulation that only 250 Watts or 500 Watts are allowed. This is now easy doable. 
You even can add the Efficiency of like 90% (250 / 0.9 = 277 Watts Output). 
But it seems that this doesn't legalize the Board in Germany. But i needed to give it a try. Maybe it helps for other country's or they change the law. 
I am working also on other stuff at the moment which allows you to change the mode at any time via APP or the remote. So this way this would be the default setup and via app i can enable full power. Once you switch the board ON and OFF again you are back in this mode. (Let your mind flow for what that could be good for :wink: But keep it four you)

But anyway. This is only a additional Mode which is a try to get the board legalized. The main mode is the "Watt no reverse with brake" which gives you way more control at higher speeds.
```

---
## \#6 Posted by: Maxid Posted at: 2016-11-02T17:15:33.082Z Reads: 1218

```
I am wondering why there is apparently so little interest in this. This thread deserves way more views and comments.
Personally I am just too cowardly to try it out before there are more reviews.

However: Where are the download links?
```

---
## \#7 Posted by: chinzw Posted at: 2016-11-02T17:20:00.722Z Reads: 1166

```
There would be a ton more interest if there was source code and pre compiled firmware available.
```

---
## \#8 Posted by: jmasta Posted at: 2016-11-02T17:27:47.429Z Reads: 1148

```
Also, only Ubuntu (for now?)

Looks cool though
```

---
## \#9 Posted by: ThomasRBK Posted at: 2016-11-02T17:34:01.805Z Reads: 1128

```
Looks awesome mate!
```

---
## \#10 Posted by: Bender Posted at: 2016-11-02T17:37:21.609Z Reads: 1130

```
I'm very interested 
Waiting for some testing and an OS X version
```

---
## \#11 Posted by: Ackmaniac Posted at: 2016-11-02T18:18:41.465Z Reads: 1122

```
I have the firmware and the BLDC-Tool ready, but only for Ubuntu. Firmware would work everywhere but without the modified BLDC-Tool it doesn't make sense. 
Does anybody know how to compile t for windows. Did some first tests and can get in running in QTCreator but not yet as standalone exe. Some help would be appreciated.

If anybody wants to test for Ubuntu send me your email via PM and i send you the files.
```

---
## \#12 Posted by: chinzw Posted at: 2016-11-02T18:27:02.630Z Reads: 1081

```
I'd like the source code if you can provide that.
```

---
## \#13 Posted by: treenutter Posted at: 2016-11-02T18:32:58.747Z Reads: 1090

```
@Ackmaniac this is such great work! You've done an amazing job not only identifying features that esk8'ers need, but you also implemented them which is even more impressive. I'll PM you for details on downloading.

Do you have plans to keep up with Vedder's official BLDC-Tool releases and firmware? Or, perhaps, to collaborate w him directly to integrate your work into the official release?
```

---
## \#14 Posted by: Ackmaniac Posted at: 2016-11-02T19:06:39.324Z Reads: 1046

```
It would be great if i can leave a footprint in the Esk8 community if this would be part of the official version. I really think it has the potential. 
But i also think that Benjamin doesn't have time at the moment to listen to any of those modifications because of the VESC 6. But i think that if i get a good feedback from the community then he could be interested.
```

---
## \#15 Posted by: E-Boarding Posted at: 2016-11-02T19:20:08.343Z Reads: 1007

```
Vedder is developing a new VESC-Tool for Vesc 6.0
```

---
## \#16 Posted by: SageTX Posted at: 2016-11-02T19:21:31.911Z Reads: 998

```
Was planning on using steering channel as on/off for leds/lights.   

Could the cruise be set to enable with -30 pm Only so that +30 can still be used with a switch (and servo splitter)?

Just a tweak I thought might be helpful.
```

---
## \#17 Posted by: Ackmaniac Posted at: 2016-11-02T19:52:41.441Z Reads: 995

```
It would be possible to do that. But i think i have a better idea how to control the lights. But for that another device would be needed which can be controlled by the Remote. But more on that in the future. In Germany we try to avoid as much attention as possible because the police can fuck us badly here. But when i have my other stuff ready i might think about lights.
But it could be possible to activate the cruise control at only one direction. It also would be possible to enable cruise control without brake when you steer left and cruise control with brake when you steer right. First of all i want to get impressions how people like the cruise control and if they have safety concerns.
BTW cruise control in current control for BLDC mode works much better than cruise control with duty control. It is really smooth now.
```

---
## \#18 Posted by: solarcross Posted at: 2016-11-02T21:54:24.877Z Reads: 957

```
Windoz plz
```

---
## \#19 Posted by: Ackmaniac Posted at: 2016-11-02T21:59:29.184Z Reads: 951

```
I am working on a windows version at the moment but i didn't get far. Maybe someone here in the forum can help.
```

---
## \#20 Posted by: Ackmaniac Posted at: 2016-11-03T00:24:11.663Z Reads: 962

```
I was able to get it running on Windows. But i need more testing to be sure that it works without issues. Didn't try the firmware upload yet because i don't have a spare VESC. 
If anybody has a bootloader (if it goes wrong terribly) and the balls to test it please let me know. Then i will send you the files for windows. The reading and writing of the settings and also the real time graphs work quite well.
```

---
## \#21 Posted by: solarcross Posted at: 2016-11-03T01:13:37.723Z Reads: 887

```
Wondering if you can figure this out and SAVE US !!
Some use 3-wire twist throttles on UART port..  
we need the ADC. 3.3V and GND from a different port..because UART port is needed for bluetooth ..
doesnt matter which one... which Im told would be a custom FW..
??
any ideas.. thnx
```

---
## \#22 Posted by: magnetvox Posted at: 2016-11-03T02:59:13.195Z Reads: 854

```
Why aren't people just using VM's, eg virtualbox and a ubuntu image (both free and simple, and will work on Win and OSX no dramas)? If people can build their own skateboard, inc tune the VESC and load modified firmware, then it's a walk in the park to spin up a VM and assign a USB port to it. Save's the smart bloke doing the BLDC-tool mods from wasting time/ energy with OS conversions, which could instead go into more testing/ improvements. Just a thought.
```

---
## \#23 Posted by: rpn314 Posted at: 2016-11-03T03:04:16.463Z Reads: 854

```
I've got Windows box around, a vesc, an st-linkv2 for flashing, and a pair. I'll give it a go. My base machine is Mac as well, so I can fiddle on that side too.
```

---
## \#25 Posted by: Ackmaniac Posted at: 2016-11-03T09:47:42.724Z Reads: 869

```
Finally got it running for windows and everything should work. 

If anybody wants to test you can download the files here.
[Windows BLDC-Tool, Modified Firmware and Ubuntu BLDC-Tool](https://www.dropbox.com/sh/t7dl90owz5ccbyl/AAANyC-yQCMeveA7errNRnYqa?dl=0)

**Here are some additional install instructions. Read them before please:**

Be aware that this is only for Hardware Version 4.10 or above.

Important: When you upload the Firmware then do **not** read the settings of the VESC.
Flash the Firmware **directly**. Otherwise this can cause trouble.

1. Open the downloaded BLDC-Tool 
2. Upload the new Firmware which is attached to this email.
3. Check the default values in the new BLDC Tool. When these are OK then you can use it. If the vaules are creazy then flash the firmware again.
4. Adjust the settings of your VESC. I would not recommend to use a saved config. It would be better and safer to set the values manually. So you should make screenshots of your old setup or write it down.

But please be careful when you test it. I don't want that anybody gets hurt.

If you have trouble then let me know. And i really would appreciate some **feedback**.
```

---
## \#26 Posted by: Ackmaniac Posted at: 2016-11-03T20:14:59.380Z Reads: 790

```
Did anybody give it a try yet? I did already around 500km on a single and dual drive with Watt Control Mode. All without issues.
But i would like to know what other people think about it.
```

---
## \#27 Posted by: Pimousse Posted at: 2016-11-03T20:33:05.499Z Reads: 786

```
It's terribly awesome !!!!
You rocks @Ackmaniac !

The feature I love the most is the center PPM parameter !
With custom mod, it's so difficult to keep a symetric curve of the throttle.
With your firmware, my dream come true ! 

I have a spare VESC, I'll try this asap. :wink:
```

---
## \#28 Posted by: XIII Posted at: 2016-11-03T20:58:18.250Z Reads: 791

```
<img src="/uploads/db1493/original/3X/c/1/c1b95be20b8c32f6f8e08224644c38860850ee8f.png" width="690" height="368">

What am I missing here ? :)
```

---
## \#29 Posted by: Ackmaniac Posted at: 2016-11-03T21:22:45.500Z Reads: 750

```
Which Windows are you using?
```

---
## \#30 Posted by: E-Boarding Posted at: 2016-11-03T21:26:18.628Z Reads: 741

```
had the same problem, googled for an hour and fixed it, some dll is missing:

Go to the folder 'release' where the .exe-file is and create a folder 'platforms' and put this file in there http://www.file-upload.net/download-12066170/qwindows.dll.html

hope this helps for now

(I've Win 10 64bit)
```

---
## \#31 Posted by: Ackmaniac Posted at: 2016-11-03T21:27:58.068Z Reads: 710

```
lol, also found that out 10 seconds ago. But help is abslolutely welcome. Will update this to the file folder
```

---
## \#32 Posted by: XIII Posted at: 2016-11-03T21:28:12.854Z Reads: 701

```
Works like a charm!
```

---
## \#33 Posted by: Ackmaniac Posted at: 2016-11-03T21:30:25.916Z Reads: 692

```
I updated the File. Please download the Version from the link again and try it. Want to know that it is fixed.
```

---
## \#34 Posted by: XIII Posted at: 2016-11-03T21:32:18.886Z Reads: 690

```
It works for me, with the new dropbox files
```

---
## \#35 Posted by: E-Boarding Posted at: 2016-11-03T21:37:52.281Z Reads: 685

```
worx for me too, going to test this out this weekend
```

---
## \#36 Posted by: Jinra Posted at: 2016-11-03T21:41:44.195Z Reads: 696

```
I'm having some trouble understanding how this is different from current control. How exactly does it feel different from CC at high speeds, and how do you "have more control"? Does hold a certain throttle position correlate to a certain RPM? What does the value in "ramp by current mode" represent?It sounds interesting for sure, I just don't understand the specifics. 

Also you making want to fix the wording to "braking" instead of "breaking" in the tool and instructions :stuck_out_tongue: At leats, that's what I'm assuming you meant.
```

---
## \#37 Posted by: Ackmaniac Posted at: 2016-11-03T22:06:28.640Z Reads: 706

```
The problem with the Current Control is that at high speeds you loose throttle range. Should mean for the most settings you only have 50 or 60 % of the throttle range left. Everything above that (for example 70% throttle) does not lead to more power. 
I guess you also realized that at high speeds 50% throttle is the same as 80% throttle. So you only have the possibility to control the power from 0% till 50% throttle. That makes it harder to carve because it isn't easy anymore to control the power. 
With the new Watt Control Mode 80% throttle is 80% of the power also at high speeds. So you feel more comfortable because you can control the power better.
At the beginning it feels like the board has less power. But after some time you just learn that you need to push the throttle a bit more than before. And you start to love it when you like carving at higher speeds.

And ramp by current mode means that it ramps with the current mode until the power is reached that you define by the throttle. This ramps the power by current control till around 25% duty cylce. After that the watt control takes over. this way  the motor starts softer at low speeds. I realized that problem when i had my board on the bench.
Because when the max watt setting is at 1000 Watts. then 10% throttle means 100 watts. But when the board trys to reach 100 watts at around 5% duty cycle then it kicks in really hard because it needs to use nearly maximum current for the motor. So the motor start up is very hard. When you stand on the board and use a kick push then it should be OK but on the bench it feels too hard. 
So i decided to add this parameter to have a smoother startup which really makes it nicer and i strongly recommend it.
```

---
## \#38 Posted by: SeanHacker Posted at: 2016-11-03T23:48:28.816Z Reads: 662

```
Hey guys using Ubuntu. @Ackmaniac Just uploaded the source in a zip file to his dropbox so that we can use it properly. Just download, extract, and install just like you install vedders BLDC_Tool.
```

---
## \#39 Posted by: Jinra Posted at: 2016-11-04T00:39:23.066Z Reads: 689

```
That's not entirely true though. Current control won't "lose" power at higher throttle. It just ramps to max speed, which will depend on load compared to where in the throttle you reach it. 

For example, i might reach full speed on flats with 30% throttle, in which 70% doesn't do anything, but if we're going up a slight incline it could take 60%throttle to ramp to full speed. You still have all the available power in CC mode, it just depends when it is that you fully overcome load.

Going up a steep incline you can feel a difference in power from 0 to 100% throttle.

That said, are you saying the the benefit of watt control is that you get more throttle range (not necessarily power) at high speeds compared to CC?
```

---
## \#40 Posted by: chinzw Posted at: 2016-11-04T00:46:16.199Z Reads: 670

```
Well, with wattage mode, lets say you have max 1000w, then throttle to 100% would try and push those 1000w.
```

---
## \#41 Posted by: SeanHacker Posted at: 2016-11-04T00:53:38.512Z Reads: 691

```
Alright guys. So I'm like a new born baby when it comes to all this stuff so far. Just got my first e-board (Enertion Raptor) 6 days ago. How do I know the wattage of my board? Do I need to set anything specific in "Define Max Watt" when using this? Or just leave it default? Thanks for any help you guys can offer. If there's anything else I need to know I'd greatly appreciate it.

<img src="/uploads/db1493/original/3X/6/0/6058ca1540e2b1d3a52bf29a12a0918178ac7609.png" width="690" height="125">
```

---
## \#42 Posted by: Jinra Posted at: 2016-11-04T00:55:15.124Z Reads: 659

```
Hm, yea i understand that much so far, but wouldn't suffice to say that current control already does a similar thing? You set motor max to 80a and 100%throttle will ramp the current up to 80 at the given battery voltage. How does watt control control the speed relative to throttle position?
```

---
## \#43 Posted by: Ackmaniac Posted at: 2016-11-04T00:59:29.400Z Reads: 660

```
I didn't say that CC looses power at higher speeds. It looses throttle range. It depends on the max Battery and max motor settings of your vesc but for most setups it starts at around 50% duty cycle that you loose throttle range. Because CC mode only controls the current of the motor. 

So lets say you have 80 Amps as max motor and a 50V Battery as example. So at 75% throttle at 20% duty it would be (80 A * 75%) * (50V * 20%) = 600Watt
At 80 % duty cycle it is (80 A * 75%) * (50V * 80%) = 2400 Watts

But when your Batt max is set to 30 A the maximum power output is 50V * 30A = 1500 Watts. So even when you give only 50% throttle at 80% duty cylce you don't get below 1500 Watts. 
(80 A * 50%) * (50V * 80%) = 1600 Watts

So a bit more than half of your throttle range is gone.
```

---
## \#44 Posted by: Jinra Posted at: 2016-11-04T01:02:28.711Z Reads: 627

```
I guess I'd have to try it to really understand, thanks for explanation!
```

---
## \#45 Posted by: Ackmaniac Posted at: 2016-11-04T01:15:33.635Z Reads: 636

```
CC mode would work like Watt mode when Battery max and Motor max are the same values. But you don't want to ride a 80A Motor max and 80A Battery max monster.. (80A * 50V) = 4000Watts. Dual drive 8000 Watts.
With watt mode you also have the advantage to set the settings values to it's max values fo the motor and battery and define the power by the watts.
So you could even set the settings for Battery max to 80A  (4000 possible watts) and set the max Watt value to 150 Watts and give it to your kids. And it will behave as soft and gentle as a teamed baby bunny.
And when you want to release the beast set it to 2500 watts.

BTW, if you want a softer rampup at low speeds i recommend to set the motor max a bit lower.
```

---
## \#46 Posted by: Ackmaniac Posted at: 2016-11-04T01:32:13.981Z Reads: 629

```
@SeanHacker You can set the max watt to your prefered settings. If you have a raptor with 60A max Battery output at 10S then at a load voltage of 3.7V per cell you can output around (3,7V * 10S) * 60A = 2220 Watts.
Devide that by 2 if you have a dual setup (2 motors). 2220 / 2 = 1110 Watts.
So you would have also in your VESC settings the Battery max at 30A in case of a dual raptor. I think that those are the default settings of the Raptors. But i don't know. (@onloop A sample of a Raptor could help me with that problem :joy:)
It depends what your previous settings were.

More simple, if you like the actual power of your board then get the actual max Battery Current value defined in the Vesc Setup and calculate the max watt like this
.
Max Battery Amps * 3,7V * Battery Cells = Max Watts

E.g 30A * 3,7V * 10S = 1110 Watts

If you want more power you also have to increase the max battery current because i don't allow to draw more amps from the battery then this value to prevent damage.
```

---
## \#47 Posted by: Ackmaniac Posted at: 2016-11-04T01:42:21.057Z Reads: 606

```
I added 2 videos to the dropbox link i made a while ago which shows how the system behaves at constant 50% throttle in current control mode and at 50% throttle in watt control mode. 
With watt control you can see that it ramps up like in current but then stays at around 680 Watts. Current control mode even reaches nearly 1200 watts.
But just give it a try. Then you will feel the difference. 
I recommend to do 2 test runs with carving shortly after another in CC mode and in Watt mode to really compare it.
```

---
## \#48 Posted by: shiro836 Posted at: 2016-11-04T05:09:05.033Z Reads: 587

```
Very cool! is it possible to implement watt control for the nunchuk as well?
```

---
## \#49 Posted by: The_Dude Posted at: 2016-11-04T08:39:37.680Z Reads: 580

```
Which app do you use for the realtime monitoring in the video? Thanks for your contribution!
```

---
## \#50 Posted by: Ackmaniac Posted at: 2016-11-04T08:53:01.328Z Reads: 624

```
That's my own app. Will also share that later. So this firmware also gives more possibilities. For example change control mode while you are driving via app or remote. And the change would update all VESCs in the can bus. But I don't have it working with Bluetooth yet. Only with WiFi. So my board is a access point at the same time. But I will publish that stuff at a later stage. And also for free. Still playing around with it.
At the moment it looks like this
<img src="/uploads/db1493/original/3X/c/0/c08fd4be233c07ce234d62251828d1d6a157f891.png" width="281" height="500">

But more important for me is what you think about the new firmware features after testing.
```

---
## \#51 Posted by: The_Dude Posted at: 2016-11-04T10:02:53.952Z Reads: 589

```
I'm not using PPM but the Nunchuk Kama for driving - most of all because I like the cruise control and I got used to the feeling of the nunchuk device in my hand. With PPM there is probably no chance to realize acceleration when in cruise control? 
So there is always the conflict of the already used UART port when driving with a Nunchuk :rage:
So: I'm VERY interested in testing the Watt-Mode, is it hard to implement it for Nunchuk Users?
```

---
## \#52 Posted by: Ackmaniac Posted at: 2016-11-04T11:27:52.992Z Reads: 582

```
First of all it would be doable to implement acceleration during cruise control. Also thought about that. And it would be doable to implement the watt mode to Nunchuk. Only problem it takes time. but i see what i can do. It's weekend now.
```

---
## \#53 Posted by: The_Dude Posted at: 2016-11-04T11:34:41.015Z Reads: 562

```
Sounds promising. When using the Nunchuk I have an additional (in fact two) button to set and hold the desired speed - how can this be realized when only a PPM signal is sent to the VESC?
```

---
## \#54 Posted by: Ackmaniac Posted at: 2016-11-04T11:37:50.533Z Reads: 555

```
Please explain me how it works for the Nunchuk. How can you control it in detail? i guess you slowly can set the speed a bit higher or lower.
I can aggree to set it lowly higher when the acceleration is pressed. But i don't think it is safe to slowly decelerate when you press the break. Because in a shock moment you want to break and maybe forget to release the cruise control (steering in my chase)
```

---
## \#55 Posted by: Ackmaniac Posted at: 2016-11-04T12:11:57.752Z Reads: 529

```
Have the coding for the nunchuk already done. Now the problem is to add all the settings to the bldc-tool. That takes most of the time.

But anyway, Is there anybody who made already a test ride and will share his thoughts.
```

---
## \#56 Posted by: The_Dude Posted at: 2016-11-04T12:29:14.874Z Reads: 529

```
Of course: works like a "Tempomat". When I want to "lock" a certain speed during driving, I press the C-Button. As long as I keep the button pressed the speed stays the same (Joystick in neutral position). Also, still the button is pressed, I can incement or decrement the speed using the joystick. The stepsize of the increments/decrements are set how far I move the joystick forward or backwards. When I release the C-Button I have the "normal" or so to say "direct" control, which is the same as in PPM-Mode I suppose.
Btw I didn't try what happens when decelerating hard in Cruise Control an suddenly release the C-Button ... full break :open_mouth:
```

---
## \#57 Posted by: Ackmaniac Posted at: 2016-11-04T12:33:38.349Z Reads: 533

```
That is where i see the safety risk. Also i see a risk when you have a shock moment and brake with cruise control activated. then you only decelerate slowly instead of do a hard brake. And when you then release it it would kick in too hard as you mentioned. Had that problem with the acceleration as well. that is the reason why i allow cruise control only when the throttle is not touched.

But if anybody has a better idea how it should behave and that it would be safe then feel free to share.

One thing i could imagine is to allow acceleration when you would request for more watts then cruise control is using in that moment. Because then you would feel it immediately when you accelerate and you can't get shocked when you release the cruise control. 
But for now i leave it as it is. That means it only is allowed to run when the throttle is not touched.

BTW for the Nunchuk i use the standard Nunchuk behavior do don't mix it.
```

---
## \#58 Posted by: ra.rend Posted at: 2016-11-04T12:44:18.059Z Reads: 516

```
@Jinra You have yours set to FOC, correct? Have you tried this? It shouldn't cause problems since you're uploading a new firmware?
```

---
## \#59 Posted by: Ackmaniac Posted at: 2016-11-04T13:03:18.310Z Reads: 528

```
I normally ride in BLDC mode. I haven't change the way FOC is handled. I calculate the current for the application in a different way but otherwise i don't change the internal Motor control. 
Only thing i have added additionally is the max watts for Cruise control in BLDC and FOC mode. That tells the Cruise control to don't use more Watts than the max Watt setting allowes.
But still all the other safety features of BLDC and FOC mode are there and have a higher priority.
```

---
## \#60 Posted by: The_Dude Posted at: 2016-11-04T13:12:19.210Z Reads: 536

```
It's not difficult to take care of this "risk". I implemented a cruise control two years ago when controlling my first Skateboard with a Teensy Controller and a Nunchuk. You simply only allow to go from cruise control to direct control when you are in the neutral position while the switching. Worked absolutely perfect. Using cruise control in this way was really no problem since then and it's really a pleasure using it this way. It's great to have cruise control and direct control at your fingertips available - you must try. When in panic mode you normally release the C-Button and the Joystick, so there won't happen anything worse.
To be honest, I have to check if Vedder did not already implemented some kind of safety feature in the firmware. I keep you updated.
```

---
## \#61 Posted by: Ackmaniac Posted at: 2016-11-04T13:24:53.764Z Reads: 565

```
Can you alos post a Screenshot of your actual Nunchuck settings in BLDC-Tool. Would help me to understand it a bit better.

I also had a look at the code and there is a safety feature when the new current is more than 5 Amps away then the previous current. But i think it still kicks in hard. But please test what happens when you release the cruise control button while you break hard and accelerate hard.

I think i have a better solution for it but maybe it handles nicely.
```

---
## \#62 Posted by: Pimousse Posted at: 2016-11-04T13:58:10.499Z Reads: 540

```
This is really impressive !
But it's a shame that so many genius build their own app instead putting effort together to build a very powerful and unique tool for smartphone.

I assume you modified the serialization of GET_VALUES command through UART ?
That means that other app using standard VESC communication protocl won't work anymore after flashing your firmware ?
I currently worked as beta tester on another app (VESC Monitor) so I can't use your firmware for that reason :frowning:
```

---
## \#63 Posted by: Jinra Posted at: 2016-11-04T14:08:48.053Z Reads: 514

```
I only use bldc, never messed with FOC.
```

---
## \#64 Posted by: Ackmaniac Posted at: 2016-11-04T14:14:00.815Z Reads: 522

```
@Pimousse I added my own commands. So the standard commands like GET_VALUES  are still working. Have fun. Wanted to make sure that it works with everything else which is existing.
```

---
## \#65 Posted by: Pimousse Posted at: 2016-11-04T15:48:32.618Z Reads: 508

```
I'll have a look at your code to understand !
Thanks ! :wink:
```

---
## \#66 Posted by: The_Dude Posted at: 2016-11-04T17:36:37.391Z Reads: 501

```
Made a dry test on the workbench: releasing the button when decelerating switches to direct braking. Don't know how hard it is. I will figure it out gradually when I'm on the board next time wearing protections :mask:
My Nunchuk settings are completely standard, I didn't change anything. Curious about your idea. 

Ackmaniac, where are you from? I also built a Nunchuk-NRF according to Vedder, so maybe you can give this one a try.

Can I compile your firmware for V4.7 or is it hooked only to newer HW versions? I thought it would be interesting how your power-controller performs on the Dual-Motor-Setup of my Dual-Motor eTrampa when trying a wheely ... there I need instant power and any time-lag is hard to handle.
```

---
## \#67 Posted by: Ackmaniac Posted at: 2016-11-04T17:54:11.343Z Reads: 492

```
I don't think it works below version 4.10. But i only know that normally for versions below 4.10 there is another firmware file available.
Maybe it works maybe it doesn't. Maybe somebody else knows what are the differences.
```

---
## \#68 Posted by: Pimousse Posted at: 2016-11-04T20:43:53.086Z Reads: 486

```
@Ackmaniac, do you have a tutorial for installing your BLDC Tool version on Ubuntu ?
I created a VM with latest version and follow Vedder website to install his version, but unsuccessfully.
I was planning to install yours after that.
```

---
## \#69 Posted by: SeanHacker Posted at: 2016-11-04T20:50:27.030Z Reads: 487

```
Download the source zip he has in his dropbox. Then just install it exactly like you would vedders. That's how I got it working.
```

---
## \#70 Posted by: Ackmaniac Posted at: 2016-11-04T20:52:55.414Z Reads: 497

```
For me it also didn't work the first time. only way that i could install it was with Ubuntu 14.04 with 32 Bit. A newer version or 64bit version didn't work for me. But i saw from SeanHacker that he got it working with version 16 in 64bit. So maybe he can help you out.
I am not really a linux expert. I am more into programming than system administration.
```

---
## \#71 Posted by: SeanHacker Posted at: 2016-11-04T21:00:47.738Z Reads: 501

```
@Pimousse What Ubuntu version are you using. What steps have you taken to get it working so far?

<img src="/uploads/db1493/original/3X/5/b/5be153e4aa6de932f5b08484b76aa2f4d94e25da.png" width="690" height="291">
```

---
## \#72 Posted by: Pimousse Posted at: 2016-11-04T21:07:44.259Z Reads: 485

```
I followed Vedder instructions : http://vedder.se/2015/01/vesc-open-source-esc/ (starting at the half of the page).
But I got some errors during the process.
```

---
## \#73 Posted by: Ackmaniac Posted at: 2016-11-04T21:08:22.071Z Reads: 473

```
Then i would recommend to post a screenshot of your errors.
```

---
## \#74 Posted by: Pimousse Posted at: 2016-11-04T21:28:40.770Z Reads: 479

```
<img src="/uploads/db1493/original/3X/9/0/90046125c0c8607afac6126d362f676a52b8cf3d.png" width="690" height="280">
I got this error at the first command line as well. :confused:
```

---
## \#75 Posted by: chinzw Posted at: 2016-11-04T21:31:21.101Z Reads: 451

```
Seems like your repo list is corrupt.
```

---
## \#76 Posted by: SeanHacker Posted at: 2016-11-04T21:31:50.763Z Reads: 458

```
Another process is using dpkg. You need to kill whatever it is or wait for it to finish. Also. What version of Ubuntu are you using. It's trying to install trusty packages and xenial?
```

---
## \#77 Posted by: Ackmaniac Posted at: 2016-11-04T21:32:42.169Z Reads: 459

```
That might help
http://askubuntu.com/questions/452638/how-can-i-solve-unable-to-lock-the-administration-directory-var-lib-dpkg
```

---
## \#78 Posted by: chinzw Posted at: 2016-11-04T21:33:47.082Z Reads: 450

```
Yeah, he has the pkg manager open probably. And he is trying to install trusty pkg on xenial, which is bad and wont work.

Do "sudo apt-get update" before downloading any packages.
```

---
## \#79 Posted by: Pimousse Posted at: 2016-11-04T21:36:20.512Z Reads: 463

```
Erff, it's (almost) the first time I use linux (just played a bit with a RaspPi). :smile:
 Thanks for the great support guys !
I'm using the latest version (download this evening (16.04.1 64 bits).
Should I download another one ?
```

---
## \#80 Posted by: Ackmaniac Posted at: 2016-11-04T21:41:41.312Z Reads: 452

```
Do you normally use windows?. Then you also can take the windows version in the dropbox folder.
```

---
## \#81 Posted by: Pimousse Posted at: 2016-11-04T21:42:09.142Z Reads: 465

```
No, I'm using OSX :/

Thanks to the link to your link @Ackmaniac I have no error anymore with the "lock" stuff :slight_smile:  
But now, it seems that my repos are not good, right ?
<img src="/uploads/db1493/original/3X/2/e/2e5f51d69697acde45a8c9105b47231f4c35111a.png" width="690" height="203">
```

---
## \#82 Posted by: chinzw Posted at: 2016-11-04T22:17:22.989Z Reads: 421

```
try replacing trusty by xenial in the sudo apt-get install command you're running
```

---
## \#83 Posted by: Pimousse Posted at: 2016-11-04T22:20:33.637Z Reads: 421

```
Not working (same error message).
```

---
## \#84 Posted by: chinzw Posted at: 2016-11-04T22:24:07.290Z Reads: 418

```
Hmm, seems that the repos are out of date, and also you need to enable untrusted repos
```

---
## \#85 Posted by: Pimousse Posted at: 2016-11-05T11:54:18.488Z Reads: 435

```
IT WORKS !!
As you guessed @chinzw, I has repos missing.
So I use gedit sources.list and uncomment universe and multiverse and follow again Vedder instruction, no it works.

I now try with @Ackmaniac github to install his version of BLDC-Tool
Thanks guys !
```

---
## \#86 Posted by: Ackmaniac Posted at: 2016-11-05T12:09:18.994Z Reads: 419

```
Glad to hear that you got it running. Tell me what you think about it after testing.
```

---
## \#87 Posted by: Pimousse Posted at: 2016-11-05T13:16:47.482Z Reads: 410

```
Vedder's BLDC Tool works but I can't compile yours, I got too many errors while typing "make".
I give up for today.
```

---
## \#88 Posted by: Ackmaniac Posted at: 2016-11-05T13:20:49.625Z Reads: 408

```
Which errors do you get? Screenshot helps.
```

---
## \#89 Posted by: Pimousse Posted at: 2016-11-05T13:50:32.063Z Reads: 438

```
I got thousands lines of errors.
Here's just the latest lines

<img src="/uploads/db1493/original/3X/2/2/22e1ea26c3a48708608eb80103ccc6e5eae410f0.png" width="690" height="453">
```

---
## \#90 Posted by: Ackmaniac Posted at: 2016-11-05T13:54:34.549Z Reads: 397

```
Did you unpack the zip file "bldc-tool ubuntu sources.zip" and run make inside the unpacked folder bldc-tool?
```

---
## \#91 Posted by: Pimousse Posted at: 2016-11-05T13:56:17.261Z Reads: 403

```
I guess I made some bullshits...
I deleted bldc-tool (Vedder's one) and unziped yours instead then ran the whole process with yours.
But i read I should have uninstall Vedder's one before compiling and install yours...
```

---
## \#92 Posted by: Ackmaniac Posted at: 2016-11-05T13:58:33.924Z Reads: 397

```
I have Vedders one and mine in different folders. So that is no issue for me.
maybe also try 
make clean && make
```

---
## \#93 Posted by: Pimousse Posted at: 2016-11-05T14:08:03.813Z Reads: 396

```
"make clean && make" was the magic command !
Now your version works !
Thanks so much Ackmaniac !

I let you know once I can test it in real (none of my builds are currently working...).
```

---
## \#94 Posted by: Ackmaniac Posted at: 2016-11-06T00:39:52.263Z Reads: 382

```
Currently i am implementing the watt control for the Nunchuk. Can somebody explain me for which remotes the ADC application is used for?
```

---
## \#95 Posted by: Ackmaniac Posted at: 2016-11-06T01:53:52.654Z Reads: 402

```
I implemented Watt control alss for the Nunchuk. But sadly i don't have one. So if anybody could be the beta tester you can download the firmware, windows and unix version from the Dropbox link in the folder "Beta_Watt_For_Nunchuk"

Would be great if somebody can give it a try. I checked it all 3 times and it should work. Finlly it uses the same code as for PPM, biggest problem was to implement the userinterface for bldc-tool.
```

---
## \#96 Posted by: Pimousse Posted at: 2016-11-06T07:54:39.202Z Reads: 382

```
As far as know, ADC is commonly used for ebike.
They used a wired wrist throttle made of a variable resistor.
```

---
## \#97 Posted by: Ackmaniac Posted at: 2016-11-06T14:47:05.336Z Reads: 425

```
I am currently working on a throttle curve implementation. Something like this.

<img src="/uploads/db1493/original/3X/5/8/5840698fe8ec0c307c62fb20374aaca24fdfffbe.png" width="480" height="289">

In this setup max watt is set to 1000 Watts. Trying to make it adjustable by 2 values. Benefit would be that you can define if you want to have more sensibility at lower watts.  

<img src="/uploads/db1493/original/3X/3/2/3211b3cdd078f5aa27e74c6ba4d95e177676b991.png" width="480" height="289">
Or more sensibility at higher watts.
```

---
## \#98 Posted by: Ackmaniac Posted at: 2016-11-07T00:23:01.191Z Reads: 414

```
Ok tried to find a good formula for the adjustable throttle curve. But everything i have so far is far too complicated to add this to the bldc-tool. Because to find the right curve you have to find a extreme curve and adjust it by a weird factor. That is  all not usable because people would need to experiment a lot to find the right settings.

Did anybody calculated already throttle curves and has a good formula which is easy adjustable by 2 or 3 parameters? Any help is welcome here.
```

---
## \#99 Posted by: chinzw Posted at: 2016-11-07T02:17:51.030Z Reads: 415

```
Why dont you just use bezier spline for this? Its pretty simple to implement, understand and map.
```

---
## \#100 Posted by: Pimousse Posted at: 2016-11-07T07:40:07.726Z Reads: 408

```
If it helps, I heard a lot of EXPO curve feature in car ESC.
I assume it's "exponential".
```

---
## \#101 Posted by: Ackmaniac Posted at: 2016-11-07T12:36:05.250Z Reads: 440

```
I think i go with something easier which is linear. Because i think in reality you don't feel the difference. And it would be easier to adjust it.

<img src="/uploads/db1493/original/3X/d/5/d5b7c7e67f7256ebb66a147768648e0ca3c76fd4.png" width="592" height="499">

The other question is is this really wanted by the community or not. Because it is a lot of work.

And did somebody give the new watt control and cruise control already a test run?
```

---
## \#102 Posted by: E-Boarding Posted at: 2016-11-07T12:54:23.403Z Reads: 410

```
I tested the speed control no accelaeration with 250W-limit but it felt weak, maybe it's not possible to make a law-confirm-board that is viable for commute, sadly.
It felt I pushed the board to about 20 km/h, pushed the button and the board slowed down a bit and I cruise at about 15 km/h or something.

Best thing, it slowed down downhill and kept the speed, that was nice.

I need to increase the watt-limit I think and test again.
```

---
## \#103 Posted by: Ackmaniac Posted at: 2016-11-07T13:03:00.201Z Reads: 427

```
So you tested the "PID speed control no acceleration". Be aware that this mode doesn't make the board legal in Germany. It was only a test and to be prepared if the law get's changed. And if you want to output 250 watts then you also can add the efficiency loss by calculating 250 / 0.90 = 277 Watts for 90 % efficieny of the brushless.

You should give the normal "Watt no reverse with brake" control also a try.
BTW i run my single drive board with 1600 Watts max and my dual drive with 1200 max Watt each, (so 2400 Watts total).

If you want to compare Watt control against Current control then set the max watt by the this calculation.

Your Max Battery Amps * 3,7V * Battery Cells = Max Watts
E.g 30A * 3,7V * 10S = 1110 Watts

But some more tips for "PID speed control no acceleration".
You said that you like that it slows down going downhill. I recommend to switch off breaking in cruise control. You can do that over the advanced tab. Because then it is really nice to carve at cruise control.
<img src="/uploads/db1493/original/3X/e/8/e87a745437f4373169d1ddb5ca907b78e559ef56.jpg" width="690" height="493">
```

---
## \#104 Posted by: E-Boarding Posted at: 2016-11-07T13:12:42.327Z Reads: 391

```
Maybe it's not legal but with no acceleration an the limits 250W at 25km/h it is not a KFZ and so they can't fuck me over with 1500 Eur and confiscate my board.

I'll test a few different setting the nect weeks, when the rain stops...

Does it make any difference if I set the watt-limit at "Define-Max-Watt" or at "Max Battery Amps * 3,7V"?
Because when the board is full charged it's about 41V and empty at 32V, so I guess the "Define-Max-Watt" is more accurate?
```

---
## \#105 Posted by: Ackmaniac Posted at: 2016-11-07T13:22:58.296Z Reads: 388

```
Yes it does make a huge difference.
Max Battery Current is the max amps the VESC can draw from the battery. So max watt can't go higher then the max watt which is allowed to draw from the battery. 
So if you have a 10 S battery and set max battery amps to 30 you are allowed to draw maximum 30A * 3,7V * 10S = 1110 Watts.
If you set the max watt value to 1500 Watts in this scenario you also would loose throttle range because when the throttle tells to provide more that 1110 watts the VESC does not allow that.
So i recommend to set a value for max watts below the result of that calculation and not higher than this.

For example on my single drive 10S i have set max battery amps to 50 A which would allow around 1850 watts (50A * 3,7V * 10S = 1850 Watts). But i set max watts to 1600.
```

---
## \#106 Posted by: Ackmaniac Posted at: 2016-11-07T15:03:29.405Z Reads: 370

```
Maybe i should share how Watt Control feels to me compared to Current Control.

With Watt Control it feels like i have have a direct connection between my finger and the boards power. And at higher speeds it is very controllable which makes carving nice, because i can use the full throttle range.

Current control feels to me like if there is some chewing gum between my finger and the trigger. And at higher speeds it brings you easily out of balance when you have a powerful setup because of the loss of throttle range.
```

---
## \#107 Posted by: The_Dude Posted at: 2016-11-07T21:59:25.781Z Reads: 373

```
I implemented a parametric mapping for my teensy controller. First I tried bezier splines because in fact you only have 2 parameters to choose, the normalized gradient at the beginning an at the end. I ended up using an exponential function because there is only one parameter left tho choose, the exponent:

    //Exponentialfunktion
    #define YAchseExpAccel (float)              2.0 // Beschleunigungsfunktion 1 linear, 2 quadratisch
    #define YAchseExpBrake (float)              1.0 // Bremsfunktion 1 linear, 2 quadratisch

But more important for the user experience was the possibility to choose different exponents for acceleration and braking. So you might consider this too.
```

---
## \#108 Posted by: Ackmaniac Posted at: 2016-11-08T00:01:14.082Z Reads: 381

```
First hard fight i have to do is adding a graph in BLDC-Tool which shows the throttle curve.
Took a while to understand the Framework. But finally i have the first results. Still far from finished but it seems i am getting there.

<img src="/uploads/db1493/original/3X/b/a/bac0c405ea9e1bddf1f96853254c145a791dbac0.png" width="690" height="371">
```

---
## \#109 Posted by: chinzw Posted at: 2016-11-08T00:06:32.781Z Reads: 361

```
@Ackmaniac quick question, will your 3 point PPM work with current control or does it only work in watt mode?
```

---
## \#110 Posted by: Ackmaniac Posted at: 2016-11-08T00:07:36.720Z Reads: 348

```
It could also work in Current control. But i think it would make it even less responsive. But i will try to implement it for both.
```

---
## \#111 Posted by: chinzw Posted at: 2016-11-08T00:09:32.531Z Reads: 350

```
Oh i mean, if the min max and center will work in currenbt control.
```

---
## \#112 Posted by: Ackmaniac Posted at: 2016-11-08T00:10:32.314Z Reads: 350

```
Yes it does. Works for every mode.
```

---
## \#113 Posted by: Ackmaniac Posted at: 2016-11-08T01:41:19.228Z Reads: 373

```
Enough work for today.

<img src="/uploads/db1493/original/3X/8/4/846c4e71f2f62ece9a00201a1d1d348ea959d259.png" width="690" height="372">
```

---
## \#114 Posted by: The_Dude Posted at: 2016-11-08T08:57:21.645Z Reads: 357

```
Coming back to the firmware 4.7 question. If you don't mind, I would like to compile your firmware extensions for my HW4.7 - are you willing to supply the sources? Would be great, even if I have the chance to spoil my HW once again :persevere:
```

---
## \#115 Posted by: Ackmaniac Posted at: 2016-11-08T09:19:37.545Z Reads: 350

```
Let me first finish my throttle curve adjustment and then i will make my code public so that you can compile your own firmware.
```

---
## \#116 Posted by: Hillso Posted at: 2016-11-08T09:44:08.810Z Reads: 354

```
Wow, great work.
now, who wants to make an PID acceleration control mode? :laughing:
```

---
## \#117 Posted by: Ackmaniac Posted at: 2016-11-08T10:06:13.487Z Reads: 374

```
The user interface to control the throttle curve got much better than expected and is really easy to understand. I am really surprised.
<img src="/uploads/db1493/original/3X/9/0/909258da6ed82f9f321fad677ae8da3a012d103b.png" width="690" height="459">
```

---
## \#118 Posted by: Pimousse Posted at: 2016-11-08T11:02:48.733Z Reads: 350

```
:astonished:
Ackmaniac, you're a genius !
What an amazing job !

You should definitely share it with Vedder.
It will be a shame to loose all this great job with VESC Tool and VESC 6. :wink:
```

---
## \#119 Posted by: Ackmaniac Posted at: 2016-11-08T11:58:28.546Z Reads: 354

```
And for that you guys need to test it. Because if the community likes it then i think Benjamin will think about it.
```

---
## \#120 Posted by: Maxid Posted at: 2016-11-08T12:02:00.039Z Reads: 365

```
I start to feel bad for not giving this a shot. Once my battery is finished I might try it - but that will take some time (and it's winter now :( )
```

---
## \#121 Posted by: Pimousse Posted at: 2016-11-08T12:33:18.830Z Reads: 390

```
Same for me mate !
I run from issue to issue with my builds.
Once it won't take fire anymore I'll be more than pleased to test your version ! :smile:
```

---
## \#122 Posted by: Ackmaniac Posted at: 2016-11-09T00:04:52.307Z Reads: 382

```
Got the software ready today for the adjustbale throtlle curve implementation. Hopefully i find the time to test it tomorrow. 
Finally It should work for all Control modes (Duty Cycle, Cruise Control, PID and Watt). But i think it really only makes sense for Watt Control because of the precise definition of the power output.

I really hope that it feels the same way as i think it would feel. It is highly adjustable, that means no predefined curves. So everybody can create it's own completely independent curve in a very easy way that everybody understands.

<img src="/uploads/db1493/original/3X/b/7/b7a7e4d99aae524134e2582b408793f8c726817b.png" width="690" height="419">
```

---
## \#123 Posted by: Pimousse Posted at: 2016-11-09T07:12:40.610Z Reads: 347

```
Amazing job ! Can't wait to test it !
There is a little typo in the legend of the chart "Costum".

Now, I can say I contributed to your project ! :smile: :smile:
```

---
## \#124 Posted by: Pimousse Posted at: 2016-11-09T21:27:17.736Z Reads: 339

```
@Ackmaniac, I want to upload your firmware but BLDC Tool says that the file name is not correct.
Any idea ?
```

---
## \#125 Posted by: E-Boarding Posted at: 2016-11-09T21:35:11.207Z Reads: 340

```
Had the same problem, I renamed the firmware to VESC_default or some shit and it worked somehow.
```

---
## \#126 Posted by: Ackmaniac Posted at: 2016-11-09T21:41:26.218Z Reads: 333

```
Thx for the info. I renamed it to VESC_default. Didn't know that, sorry. Maybe you can try if it works now with the updated dropbox files name.
```

---
## \#127 Posted by: Pimousse Posted at: 2016-11-09T21:48:51.701Z Reads: 343

```
I just finished a build a wanted to configure it through Vedder's BLDC but as always I was losing my hair with this fu**** PPM adjustment.
So I switched to your firmware and BLDC Tool and set the PPM in a heart beat.
This is so so so useful !!
I was crying about that on Vedder forum since a while and you made it.

Thanks so much @Ackmaniac.
You really deserve a couple of VESC-X for your test ! Isn't it @onloop ? :smile:
```

---
## \#128 Posted by: Ackmaniac Posted at: 2016-11-09T21:58:59.278Z Reads: 333

```
Now also try all the other stuff. Watt control and if you have a dual setup (2 VESCs) use the cruise control via the steering channel of your remote. And if you try cruise control then disable the breaking in cruise control to have really nice carving. 

And thanks for testing. Gives me the feeling that all those hours make sense.
```

---
## \#129 Posted by: Pimousse Posted at: 2016-11-09T22:29:46.224Z Reads: 343

```
Yes, for sure !
But for now it's snowing so it depends not only on my willing now.  :smile:
```

---
## \#130 Posted by: Ackmaniac Posted at: 2016-11-10T00:15:21.721Z Reads: 358

```
**VERY IMPORTANT****VERY IMPORTANT****VERY IMPORTANT****VERY IMPORTANT**

Don't use my modified Firmware and BLDC-Tool for FOC.  @Blasto figured out that there are issues which i have to solve first. It runs fine in BLDC but i need to find the issue for FOC. Strange thing is that i didn't change anything in the code how FOC is handled. But i will find out.

BTW: i made the first tests with the throttle curve adjustment and it works awesome.

**Update: Issue is already fixed**
```

---
## \#131 Posted by: Ackmaniac Posted at: 2016-11-10T01:05:44.483Z Reads: 343

```
Ok was analysing the code and checked my changes multiple times by comparing all my changes. And only the cruise control has a little change for FOC. But as long as cruise control is not activated it can't have any influence.

So i gave it another try. Made a FOC motor detection again. Then after changing from BLDC to FOC i rebooted the VESC. And then it worked. So it seems that those issues are also there with the normal BLDC tool.
So i recommend to always reboot the VESC after changes. Also please reboot the VESC when you change from FOC to BLDC again.

And I will try to release a new version with the throttle adjustment by tomorrow. So if there is anybody who wants to try it in  Foc then please wait for this version. Just because I checked the new one multiple times for mistakes and it was working on my bench.
```

---
## \#132 Posted by: Pimousse Posted at: 2016-11-10T05:08:03.789Z Reads: 323

```
Actually, some guys who fried their DRV advice to upload a fresh firmware each time  we change from a control mode to the other. It seems to keep some "ghost" values.

Do you have a Github repo for sharing your code easily ?
```

---
## \#133 Posted by: E-Boarding Posted at: 2016-11-10T08:17:03.910Z Reads: 322

```
This may be missleading as this is not the default-firmware, maybe something like VESC_ackmaniac would be better.
I used VESC_default because that was the name of the original firmware and I just wanted to make it work quickly.

And yes the original firmware do have issues with BLDC=>FOC but nobody found the failure code, maybe you get more lucky.
```

---
## \#134 Posted by: Pimousse Posted at: 2016-11-10T08:21:11.687Z Reads: 315

```
I renamed it "VESC_Ackmaniac" and it passed the name checking. :wink:
```

---
## \#135 Posted by: Ackmaniac Posted at: 2016-11-10T08:22:37.128Z Reads: 323

```
I think that Vedder will solve that stuff with the new Firmware for VESC 6 because he mentioned already that he found a lot of FOC issus which he fixed for the new firmware. So i think it would be the best to wait for that. And thanks for the check, i renamed it to VESC_Ackmaniac. And once the VESC-Tool is out then i will of course implement my changes and provide a modified Firmware again.
```

---
## \#136 Posted by: Pimousse Posted at: 2016-11-10T14:44:32.240Z Reads: 339

```
Just for my information, in case of cruise control PPM with dual VESC setup, could the cruise control be activated by the CH3 (ON/OFF momentary button) instead of steering pot ?

I see it working like a car : 
You ride at a certain speed with Watt control through the standard trigger (CH2).
Then you push one time the CH3 button. It activates cruise control so you can release the trigger it's keeping the same speed.
- If you need to accelerate, you pull the trigger. System takes into account the max of trigger or PID output. So if you release the trigger it comes back to the previous speed setpoint
- If you brake, cruise control is simply desactivated.

Could it work in this way ?
Actually, I use GT2B mods without steering pot but with CH3 button (like Mad Munkey mod) that's why I ask. :slight_smile:
Thanks !
```

---
## \#137 Posted by: Ackmaniac Posted at: 2016-11-10T15:55:24.413Z Reads: 315

```
Channel 3 would work  i think. You simply have to define the center pulsewith when the button is not pressed and the maximum pulsewidth with the value when the button is pressed. But i ma not sure if button 3 sends a signal at all when it is not pressed. You should try to find out.
And i like it more when you have to press a button or steer that cruise control keeps active. And when you release it it switches off.
Your described behavior would be possible but that only suites for buttons and not for the common steering wheel. Need to think about it in a free moment.
```

---
## \#138 Posted by: The_Dude Posted at: 2016-11-10T15:57:15.074Z Reads: 320

```
How/where do you read the Ch3? Using ADC?
```

---
## \#139 Posted by: Pimousse Posted at: 2016-11-10T17:18:09.401Z Reads: 327

```
Using PPM port of the slave VESC (onluly in dual setup).
```

---
## \#140 Posted by: Ackmaniac Posted at: 2016-11-10T18:12:52.576Z Reads: 355

```
**I am happy to announce that the new Firmware with Throttle-Curve adjustment is online now.** 

Was hard work over the last 4 days. I updated the description in the first post of this topic. Have fun.

<img src="/uploads/db1493/original/3X/2/d/2d7221846f2f810a3f2302c81c1f8ce1728631f2.JPG" width="690" height="411">

BTW i also fixed the issue with FOC in Watt Control. Problem was that the duty cycle (used for calculations) in FOC mode can be 0 and then the calculations also calculated 0 power output. This is fixed now.
```

---
## \#141 Posted by: Pimousse Posted at: 2016-11-10T19:41:44.783Z Reads: 327

```
I installed it. "Make clean && make"  !
However I got 2 warnings during compilation :

> mainwindow.cpp:2203:43: warning: unused parameter ‘clicked’ [-Wunused-parameter]
>  void MainWindow::updateThrottleCurve(bool clicked){
>                                            ^
> mainwindow.cpp:2207:45: warning: unused parameter ‘max_watts’ [-Wunused-parameter]

Oh and you should put version number to both BLDC Tool and firmware because you will release more version I guess ;)
```

---
## \#142 Posted by: Ackmaniac Posted at: 2016-11-10T19:47:45.048Z Reads: 298

```
I added the firmware version number. **It is Version 2.50 now**. 
And ignore those warnings. I know them and they are absolutely harmless. Can't avoid them. 
It is the function that creates the diagram. 
(Details: every time a value changes a listener is called to draw the diagram again. And the call always have to pass a parameter which i don't need for the diagram calculation. But i can't avoid it. So it is absolutely harmless)

BTW great that you try it.
```

---
## \#143 Posted by: Pimousse Posted at: 2016-11-10T19:58:47.725Z Reads: 292

```
I noticed some kind of bug when I played with the VESC.
When I rebooted it, BLDC Tool closed also by its own.
Is that normal ?
```

---
## \#144 Posted by: Ackmaniac Posted at: 2016-11-10T20:03:04.255Z Reads: 290

```
Does that happen every time? Doesn't happen on my computer. And if it happens every time then please restart your computer and check again.
```

---
## \#145 Posted by: Pimousse Posted at: 2016-11-10T20:19:04.809Z Reads: 292

```
I didn't try for a long time but IIRC, each time I rebooted the VESC through Reboot button.
```

---
## \#146 Posted by: Ackmaniac Posted at: 2016-11-10T20:27:49.558Z Reads: 294

```
Maybe do "make clean && make" again. Apart from the fact that this is annoying it can't have another bad effect. Does it also happen in the Vedder BLDC-Tool?
```

---
## \#147 Posted by: Pimousse Posted at: 2016-11-10T20:33:05.063Z Reads: 293

```
Never hqd this issue with Vedder's one.
I use Vedder's BLDC Tool directly on OSX.
I use yours on a Ubuntu virtual machine.
```

---
## \#148 Posted by: Ackmaniac Posted at: 2016-11-10T20:35:04.823Z Reads: 295

```
Maybe i you find the time you could give Vedders BLDC-Tool a go in Ubuntu to be sure.
And maybe you can start my BLDC-Tool via the Terminal. Maybe it gives a error message.
Could be that it is a issue with the USB device via your virtual machine when it looses connection to the VESC because of the reboot.

BTW, after you defined PPM in the general tab and rebooted you don't need to reboot again when you change the PPM specific settings. Only write and test directly.
So a reboot should only be nesessary when changing from BLDC to FOC or changing from PPM to Nunchuck or any other application.
```

---
## \#149 Posted by: SeanHacker Posted at: 2016-11-10T21:16:26.232Z Reads: 290

```
That's weird. I've been testing and haven't seen any reboots at all. Are you running this through a virtual machine by chance?
```

---
## \#150 Posted by: SeanHacker Posted at: 2016-11-10T21:17:55.280Z Reads: 282

```
@Ackmaniac You've done an awesome job on this so far. Thanks.
```

---
## \#151 Posted by: Pimousse Posted at: 2016-11-10T21:25:30.311Z Reads: 287

```
I had to configure UART for my bluetooth module so I needed to reboot several times.
I already launch your BLDC Tool via Terminal but don't have any errors on it when it closed.
Anyway, I'll see if it happens again and let you know. ;)
```

---
## \#152 Posted by: Ackmaniac Posted at: 2016-11-10T21:51:29.433Z Reads: 322

```
I must say that i am really proud on the throttle curve adjustment. It works exactly as expected. Had headaches about how to makes this easy accessible and understandable for everybody.  And i am really really happy with the result. 

Here is a example how i adjusted my throttle curve for my dual drive board with 1200 watts max at each VESC.
<img src="/uploads/db1493/original/3X/e/0/e015b24115627b58b707f649c4556d99a12d420b.jpg" width="650" height="500">

So for example the Power output at 30 % throttle is only 175 watts (2 VESCs 350 watts) instead of 350 watts (2 VESCs 700 Watts) with a linear throttle line.

So it is much easier to control the board at a constant speed while cruising around at around 30 km/h. Because the difference between 350 watts to 700 watts is much bigger (100%) then the difference of 1350 to 1700 watts (25%).

And with this mod it is possible to adjust more sensibility at lower throttle range.

And if you have a Mountain Board which needs more power because of the tires you can adjust the power above the linear line to have a higher power output and then more control for the usable power range.
```

---
## \#153 Posted by: onloop Posted at: 2016-11-10T22:20:44.660Z Reads: 284

```
This is such an important usability/ saftey advancement for very high power / high torqure boards.

Nearly everyone the first time they step on the raptors push the throttle to hard and land on arse.

This way we can tone it down but still have all the power at the top.

Congratulations
```

---
## \#154 Posted by: chinzw Posted at: 2016-11-11T00:00:58.739Z Reads: 288

```
You can fix those warnings by using:
(void)clicked;
(void)max_watts;
```

---
## \#155 Posted by: Ackmaniac Posted at: 2016-11-11T00:32:43.231Z Reads: 282

```
I will try that. Many thx.
```

---
## \#156 Posted by: yaca Posted at: 2016-11-11T12:05:29.948Z Reads: 291

```
Just saw this great news about watt control and other features and want to try this, because I also don't like it just to use 50% of the throttle range. Is the current windows version of the BLDC Tool and firmware ready to go or are there any bugs which will be fixed like this warnings? 

Btw. I have to unzip the bin file and put it into the platforms folder, right?
```

---
## \#157 Posted by: Ackmaniac Posted at: 2016-11-11T13:19:32.295Z Reads: 288

```
No, the bin file is the firmware file. Just select this one in the BLDC-Tool when you choose the firmware file.
```

---
## \#158 Posted by: Ackmaniac Posted at: 2016-11-11T20:01:34.233Z Reads: 318

```
Just wanted to let you know what i am currently working on. I am very happy with the actual throttle adjustment but i wanted to get it a bit more curvy. So i am trying some calculations.
Only Problem is that it is not as intuitive as the actual setup. So it would be nesessary to test a little bit. But you always could see the rsults in the Diagram so you know how the final result would look like. But you can really draw some nice curves by that.

Here are some examples
<img src="/uploads/db1493/original/3X/d/c/dcec5fde3025ee5eee6ba55a9a205974fbd50db1.png" width="690" height="422">

<img src="/uploads/db1493/original/3X/2/4/24f2be5fa6787562ffa4a18273b687e9862ccb3f.png" width="690" height="422">
```

---
## \#159 Posted by: yaca Posted at: 2016-11-11T20:08:57.092Z Reads: 279

```
Ok, when I wanted to choose the firmware file it just appears an empty "platforms" folder, so I thought I put the file into this folder. But I can also choose the file directly from the "Downloads" folder, so that's the same, right?
```

---
## \#160 Posted by: Ackmaniac Posted at: 2016-11-11T20:09:55.547Z Reads: 284

```
Yes , it's only a file. Doesn't matter in which folder. But please read the first post in this thread to understand the values.
```

---
## \#162 Posted by: Paulf Posted at: 2016-11-11T21:08:40.138Z Reads: 295

```
Do you think it could be possible for single motor setups to implement ppm cruise control through steering channel? 
By plugging the steering channel into the adc pin by example
Not sure it's doable, probably timer problems? 
Otherwise to bypass timer problems, maybe we could slightly modify receivers to only send all or nothing on the steering channel, then read this "all or nothing" signal through the adc pin (or an other pin) and enable or not cruise control depending on the state
```

---
## \#163 Posted by: CamBo Posted at: 2016-11-11T22:18:39.893Z Reads: 288

```
@Ackmaniac, this is AWESOME!  I setup my raptor dual this morning with your software and it's a tangible change in smoothness.  Thanks for all the hard work.  I'm pretty clueless, and I was able to get it going, so you must be doing the right thing.  

If you have a raptor, you may have had the same issue I had with an increase in acceleration (power band) that kicks in around 15-20 mph.  Ackmaniac's watt control and throttle curve have really improved this for me.  It wasn't that bad before, but it was noticeable.  On todays ride I didn't notice it once.

Now that my Throttle is Buttery Smooth, I wanted to ask you if the Braking curve could be changed the same way?  (The throttle curve is just so nice)
```

---
## \#164 Posted by: onloop Posted at: 2016-11-11T22:44:10.633Z Reads: 281

```
[quote="CamBo, post:163, topic:12286"]
Braking curve could be changed
[/quote]

That is such a good question.... I didn't even think about that.... this would be very useful. Because depending on wheel size. Reduction ratio. Rider weight, speed... etc etc the brakes strength varies greatly.
```

---
## \#165 Posted by: Ackmaniac Posted at: 2016-11-11T23:12:56.999Z Reads: 287

```
Great to hear the first impressions. Thx for testing.

Yes it would be possible to adjust the braking curve but i would need to make a lot of calculations and brainstorming to find a way that makes sense. And another problem is that i am running out of space on the PPM Screen. I think it would be necessary to add another screen like "advanced PPM" or "Throttle-Curve" (even more work). But first of all i need to understand the behavior in all situations. I should quickly study mathematics for that.

But first i will try to find a even nicer way to smooth the throttle curve a bit. (No sharp edges like in the last picture i posted). Because what i have right now works but it is a bit too confusing to adjust the curve exactly how you want it.

But for now the biggest impact on the brakes has the "Min Motor (regen)" value. For example -80 brakes harder than -60.
```

---
## \#166 Posted by: chinzw Posted at: 2016-11-12T01:54:40.483Z Reads: 275

```
I just tested this, haven't tried watt mode, but the ppm center and throttle curve work very nice!
```

---
## \#167 Posted by: Ackmaniac Posted at: 2016-11-12T02:23:45.526Z Reads: 275

```
Give the Watt Control Mode a try and you will gain even more throttle sensibility. But you have to test it on the road. On the bench you won't really see the difference.
```

---
## \#168 Posted by: chinzw Posted at: 2016-11-12T02:57:11.800Z Reads: 287

```
Yeah, i noticed no difference on the bench. Im waiting for a 3d print to finish so i can close back my enclosure and go for a test ride in watt mode.
```

---
## \#169 Posted by: chinzw Posted at: 2016-11-12T04:41:52.356Z Reads: 295

```
Just tried it, beautiful! Torque response all through the range, pretty impressive. Gotta set my rpm limits again tough, it was scary, im used to going full throttle all the time with my limits lol
```

---
## \#170 Posted by: Blasto Posted at: 2016-11-12T16:41:05.469Z Reads: 314

```
Tried it out in foc, liked it, i did not play with the throttle curve. I left it linear

http://www.youtube.com/watch?v=dYDolVNlVT0

Top speed was not affected

<img src="/uploads/db1493/original/3X/7/a/7a8a5340f91482cca6dd795205e4d1b1bc10a0cb.PNG" width="281" height="499">
```

---
## \#171 Posted by: Ackmaniac Posted at: 2016-11-12T17:17:47.243Z Reads: 317

```
A video. That was more than i expected. 
Just a hint to watt control. You will reach exactly the same top speed as with current control as long as adjusted max watt are enough to reach that speed. Watt control is more about to control the power. Full power is still full power as long as the watts allow it. Maybe share your Max Motor Amps and Max Batter Amps settings and then i can tell you which max watts you should set to reach the same power as in current control.

At the beginning of the video you said that it feels like less power. You only have to press the throttle a bit more than before. There is still the same power but over a wider throttle range. After an hour or so you get used to it.
I have a app with that i can change my control mode while i am riding and when i switch from Current Control to Watt Control it feels like switching from a "undefined digital" feeling to to a "direct analog" feeling.

Here in this example i try to explain the difference.

You can see in the table that with current control and 70% throttle you reach already at 0,55 duty cycle (half speed) the max power when the Battery Max is set to 22,5 A. at 44,4V (12S)  (22,5 * 44,4 = 1000 Watts) under load. That is the reason for the throttle range loss.
<img src="/uploads/db1493/original/3X/6/7/67f09e52b86de64fddd6468855040a9966e8bcb8.png" width="655" height="500">
Maybe all a bit too complicated but it works. You can see that in watt mode it stays to 700 Watts at 70 % Throttle and doesn't go above.

And here the same example at 40 % throttle. Watt mode stays at 400 watts and current goes up till full power of 1000 watts.
<img src="/uploads/db1493/original/3X/6/5/65f13eaabb40e29bcdbb727a1f406ee9ee9b9ec5.png" width="690" height="485">

But close to max speed (around 0,9 duty cycle) you will not really feel the difference because then you reach the efficiency border of the motor. I can't pull more watts than physically possible.
```

---
## \#172 Posted by: Ackmaniac Posted at: 2016-11-12T17:22:56.118Z Reads: 276

```
@Blasto And you sayed you have cruise control. Then switch off braking at Cruise Control and enjoy carving.
```

---
## \#173 Posted by: Blasto Posted at: 2016-11-12T17:35:37.505Z Reads: 309

```
I'm lazy, left everything default

<img src="/uploads/db1493/original/3X/d/3/d359a62846d5583acd132a358668cd933926bde2.png" width="639" height="500">

<img src="/uploads/db1493/original/3X/5/4/541eb096f9f53da4d09dda46a6654767d6eedf70.png" width="690" height="497">

Just realized that I should crank up this value


<img src="/uploads/db1493/original/3X/1/f/1fcb46e5a6364851964a0ee9fe05868c6fe88c77.png" width="690" height="497">
```

---
## \#174 Posted by: Blasto Posted at: 2016-11-12T17:37:45.280Z Reads: 277

```
look at me pretending to know watt i'm doing

<img src="/uploads/db1493/original/3X/5/0/507208dcf2fe2c58c2dfbe63647f0ab5d39a8501.png" width="690" height="490">
```

---
## \#175 Posted by: Ackmaniac Posted at: 2016-11-12T17:38:16.017Z Reads: 272

```
I guess you have a 10S Battery then set your max watt value to 10 * 3,6 * 60 = 2160 max watts. Then it will have the same power. But you see that even 1000 watts is enough for full speed because of the motor efficiency boarder.
```

---
## \#176 Posted by: SeanHacker Posted at: 2016-11-12T17:39:29.122Z Reads: 279

```
[quote="Ackmaniac, post:46, topic:12286"]
(3,7V * 10S) * 60A = 2220 Watts.Devide that by 2 if you have a dual setup (2 motors). 2220 / 2 = 1110 Watts
[/quote]

@Ackmaniac Because you know what you're talking about and I'm brand new to this stuff (only a couple weeks ago I got my first eboard) can you confirm something for me?

So if I've done the math right as you told me prior...
(3,7V * 10S) * 60A = 2220 Watts =Alright i got this part

So if I divide that by 2 because I have a Raptor dual motor (=2220) I would get = 1110 Watts

So would I set my max wattage to 1110 to get full power? Or to something less that that like the defaul 1000?
```

---
## \#177 Posted by: Ackmaniac Posted at: 2016-11-12T17:40:22.025Z Reads: 273

```
If you have a single drive then it is ok. But 2000 watts is already a lot for the belt (2000 / 740 = 2,7 hp). But if you always drive like this then have fun.
```

---
## \#178 Posted by: Blasto Posted at: 2016-11-12T17:51:57.457Z Reads: 266

```
Yes the belt will skip if i would punch it.

Don't get me wrong, i like it, but the difference is very suttle.

Time to try out some absurd settings, having the throttle curve almost flat and starting to ramp up 2/3 of the travel
```

---
## \#179 Posted by: Ackmaniac Posted at: 2016-11-12T17:56:58.750Z Reads: 271

```
At your setup you would feel the difference at 30 km/h during carving. Give it a try at watt control for 5 minutes at this speed with the throttle setup. And then shortly afterwards go back to current control without throttle adjustment (Vedder standard) and do the same. And then tell me the difference.

I can change in a second while i am riding with my app and then you really can compare. Your brain quickly gets used to watt control. But at the end of the day you realisethat you didn't have these moments when you get out of balance because of a throttle with indifferent response.
```

---
## \#180 Posted by: Blasto Posted at: 2016-11-12T18:00:24.406Z Reads: 294

```
this feels it will be pretty ridiculous

<img src="/uploads/db1493/original/3X/a/5/a57088b40b1716f072ca7e08aaa5d27ca3f4008d.png" width="690" height="445">

for science
```

---
## \#181 Posted by: Ackmaniac Posted at: 2016-11-12T18:03:50.088Z Reads: 287

```
Yes thats a bit ludacris but with my new curved edges that i will release soon it would look better. Example for same settings.
The black line.

<img src="/uploads/db1493/original/3X/8/5/8523ebd19094bc65c1b5e79900acb6e33cc17a9b.png" width="690" height="295">
```

---
## \#182 Posted by: Blasto Posted at: 2016-11-12T18:10:54.510Z Reads: 279

```
That felt actually very nice, plenty of low speed control. And i could still punch it to hit my top speed
```

---
## \#183 Posted by: Ackmaniac Posted at: 2016-11-12T18:15:55.249Z Reads: 272

```
The only problem with this modified firmware is that you will spent more time with it because of all the possibility's. You really can personalize how your boards should ride and feel.
```

---
## \#184 Posted by: chinzw Posted at: 2016-11-12T18:27:12.076Z Reads: 278

```
Yes, damn you! Now i have to go out and buy some panel mount usb connectors! hahaha, im tired of opening my enclosure to change firmware settings :S
```

---
## \#185 Posted by: Ackmaniac Posted at: 2016-11-12T18:29:43.829Z Reads: 286

```
When you do that then tape the USB-cable to the VESC so that it can't shake. Otherwise you might damage your USB plug on the VESC with the vibrations.
```

---
## \#186 Posted by: Blasto Posted at: 2016-11-12T18:32:25.964Z Reads: 297

```
Don't be hating ;)

<img src="/uploads/db1493/original/3X/4/8/488a4c3e88ebb181683eec869b1ec0b9e4ba5ee2.JPG" width="375" height="500">
```

---
## \#187 Posted by: chinzw Posted at: 2016-11-12T18:32:41.602Z Reads: 286

```
I already destroyed my vesc's usb port while drilling an enclosure :S
Might as well just solder the wires to the board lol
```

---
## \#188 Posted by: Ackmaniac Posted at: 2016-11-12T18:35:22.397Z Reads: 288

```
Just put some duck-tape around the plug and put some foam below the cable close to the VESC so that the vibrations get damped.
```

---
## \#189 Posted by: yaca Posted at: 2016-11-12T20:36:41.387Z Reads: 287

```
In current mode I used "Soft RPM Limit" to limit the top speed and for to have slower acceleration in higher speeds. I set the values at "Start" 20.000 and at "End" 25.000. Do I have to set the same value (RPM Limit End) in Watt mode for to get the same top speed? And because of the wider trigger range do I still need to set a lower value in " RPM Limit Start"? Because of rain I could not test this.

I have Motor Max 30 and Battery Max 25 for each VESC (dual hubs). 10s Lipo.  In Watt mode I will have to set max Watt to 925 or 1850 for the Master? Slave VESC ppm is disabled if I use can bus?
```

---
## \#190 Posted by: CamBo Posted at: 2016-11-12T20:53:22.658Z Reads: 288

```
@Blasto did you test with the Nano X?
I'm looking for feedback on if the Accel curve and watt control help with the short throw on this style of remote.  I have the Steez, and Ackmaniac's mods worked magic on its smoothness.
```

---
## \#191 Posted by: Ackmaniac Posted at: 2016-11-12T20:59:58.738Z Reads: 295

```
A motor max of 30 is quite low but that is personal taste. For my dual i have it at 60 with Enertion R-SPEC 6355. 
You should set it to 925 max watts. And i think you can raise the "Start ERPM" to 23000 with watt mode. It is always good to have a start and end limit if you want to set the speed limit. 
Because in that range the calculated current gets regulated. Means when set to Start 20000 and End 25000 then 10A are at 20000 ERPM 10A, 22500 ERPM 5A and at 25000 and above 0A.
And if you want to restrict your top speed to 25000 ERPM then you should also do that in Watt mode.
But just try it first with your old settings and Watt mode with 925 Watts and also adjust the throttle curve to give less power at the lower throttle range like @Blasto did. And then you can start to fine adjust it from there.
if you want more power at very low speeds then set your Motor max higher.

And if you have a steering wheel on your remote like on the mini remote and you want cruise conrol the set at the slave VESC the "Cruise Conrol via second channel" mode and connect the steering ppm to that VESC. Also don't forget to adjust the minimum, center and maximum pulsewidth on the slave.
```

---
## \#192 Posted by: Ackmaniac Posted at: 2016-11-12T21:04:59.433Z Reads: 286

```
If anybody has issues with his board and don't know how to get the settings right then please always post a screenshot of the general motor and ppm settings.

And if it helped you making your board more enjoyable and you want to donate something for the many hours and the ongoing process then feel free :grin:
[Donations](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=4R86CGGZDVE9W)
```

---
## \#193 Posted by: yaca Posted at: 2016-11-12T21:28:00.305Z Reads: 277

```
Thank you! I use Jacob's hubs and he recommends Motor Max 40 for each Vesc/Motor. 40 is really strong acceleration and for flat land 30 I like. Maybe now in Watt mode I will try to go higher, because of you now I am able to adjust the throttle curve. 925 max watts is all together or for each motor?
```

---
## \#194 Posted by: Ackmaniac Posted at: 2016-11-12T21:32:51.498Z Reads: 275

```
925 for each. 
And i don't know about hubs. When he recommends it then it should be fine. It always depends on your personal taste. But i always thought that hubs need more Amps, so i am a bit surprised. But that is stuff for another topic.
```

---
## \#195 Posted by: Blasto Posted at: 2016-11-12T21:45:56.606Z Reads: 279

```
[quote="CamBo, post:190, topic:12286"]
@Blasto did you test with the Nano X?
[/quote]

No i have the winnning
```

---
## \#196 Posted by: Ackmaniac Posted at: 2016-11-12T21:49:26.601Z Reads: 276

```
How does the winnings cruise control work. Does it simply keep the actual throttle value or does it hold the exact speed? i have a modded GT2B and a Mini remote. And the Mini remote is perfect with the steering channel to activate the cruise control. Easy controllable via one hand.
```

---
## \#197 Posted by: Blasto Posted at: 2016-11-12T22:03:16.293Z Reads: 270

```
There's no cruise on the winning. I know i said cruise in the video, what i meant is "cruising along" at a constant speed. To which it is easier to do
```

---
## \#198 Posted by: Ackmaniac Posted at: 2016-11-12T22:04:33.045Z Reads: 267

```
Oh sorry, think what i meant is the steeze remote.
```

---
## \#199 Posted by: yaca Posted at: 2016-11-13T00:19:29.166Z Reads: 287

```
I tried to configure "Soft RPM Limit". End is set to 25000 but in Realtime Data - RPM still get about 32000 RPM. I think that should not be or I'm wrong? 

<img src="/uploads/db1493/original/3X/5/b/5b8753133a91d198aa884f63d157210b4d0c7ede.png" width="650" height="500">
```

---
## \#200 Posted by: Ackmaniac Posted at: 2016-11-13T01:53:33.298Z Reads: 291

```
Actually what i said was not completely right. Checked the code (same a Vedder) and when the ERPM's are higher than the "ERPM limit end" value then the current is restricted to the value marked in yellow. So when you stand on it the wind and roll resistance is much higher then when your board is on the bench. So everything is fine. And don't set this value lower than 1A (Vedder mentioned that once).
<img src="/uploads/db1493/original/3X/4/2/42054baf716defa01060ebbd613f325d64e9eae0.png" width="690" height="412">
So if you have a 10 S fully charged battery then 1A is already 42V * 1A  = 42 watts. And i think a hub motor has even less resistance on the bench than a belt drive.
```

---
## \#201 Posted by: chinzw Posted at: 2016-11-13T06:32:16.869Z Reads: 301

```
Why use standard USB when you can over engineer some aviation connectors lol!
<img src="/uploads/db1493/original/3X/b/7/b7bae9d859c1bcb5107920480b79fd3febc47e07.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/b/6/b63ed23d25e21ac7f6646b4f74b5a7375c10263a.jpg" width="666" height="500">
```

---
## \#202 Posted by: yaca Posted at: 2016-11-13T12:53:30.267Z Reads: 291

```
Today I tested "Watt no reverse with brake" in real. I was surprised, that still just about 50% of throttle trigger range is working. In lower speed it is smoother but the rest feels almost the same as current mode. I thought I can use the whole trigger range. 
When I came home I thought maybe I'm still in current mode, but I'm not. Did I do something wrong or is it like it is? One screenshot is above. Do you need others?
```

---
## \#203 Posted by: Ackmaniac Posted at: 2016-11-13T13:14:16.963Z Reads: 276

```
Then set your "ERPM limit start" to 24000 and give that a try. Because i think it is fighting against that restriction. Please also post your General Motor settings.
But why do you restrict your max speed at all?
```

---
## \#204 Posted by: yaca Posted at: 2016-11-13T13:18:48.746Z Reads: 276

```
The max speed with 25000 is 30km/h with full charged batt. I'm using the Winning remote and had some drop outs, so till I get a new remote I stay at this top speed. 
Now my family ic calling, later I show you the screenshots.
```

---
## \#205 Posted by: yaca Posted at: 2016-11-13T14:43:45.439Z Reads: 292

```
Here are my motor settings. Both VESCs have the same values:

<img src="/uploads/db1493/original/3X/8/d/8df83b7e52e073e9c7ab08b4a07c00f05254a9e3.png" width="650" height="500">

<img src="/uploads/db1493/original/3X/5/4/5409c38d667c2c369d7fcd530605faade2cd038a.png" width="650" height="500">

<img src="/uploads/db1493/original/3X/7/1/71852307c9575a8dcc5e958480d0a4ccdc173b68.png" width="650" height="500">

I changed to 24000 and now I'll test it.
```

---
## \#206 Posted by: Ackmaniac Posted at: 2016-11-13T14:50:25.139Z Reads: 254

```
With your settings you won't feel such a big difference because the motor and battery max is very close to each other. And the moment you would feel a slight difference the ERPM limits kick in already. But you still could customize the throttle-curve.
```

---
## \#207 Posted by: yaca Posted at: 2016-11-13T18:50:32.689Z Reads: 250

```
The ERPM Limit Start at 24000 didn't change the throttle trigger range. What will be the result if I lower the value for Batt max?
```

---
## \#208 Posted by: Ackmaniac Posted at: 2016-11-13T19:55:33.283Z Reads: 261

```
Then you would have less power. Because Battery max * batter volts at load = max power output.
But what exactly would you expect? Because the power output must be already different over the entire throttle range. So do you feel a difference between 80 % throttle and 100 % throttle at 25 km/h?
Because at 30 km/h you won't feel a difference because you hit the max ERPM border. There is not much i could do about it. But you would feel it when you remove the ERPM limit.
```

---
## \#209 Posted by: yaca Posted at: 2016-11-13T21:14:44.622Z Reads: 260

```
I just try to understand the different settings of the VESC. It would be nice to set a speed limit for different situations or maybe for to give the board to other people and always could use the entire throttle trigger range like it is possible with an rc-car ESC. But it seems that is not possible in current or watt mode.
```

---
## \#210 Posted by: Ackmaniac Posted at: 2016-11-13T21:55:18.018Z Reads: 262

```
You can do that by reducing the max watt. Then the board has less power over the entire throttle range. Set it simply to 250 watts and try it. Then 100 %Throttle will be 250 watts for each vesc. So 500 watts in total for a dual drive.
```

---
## \#211 Posted by: yaca Posted at: 2016-11-14T14:50:50.530Z Reads: 256

```
Just tried that. 250 x 2 watts is really good for to give the board in other hands. Still reached about 30 km/h but it's only for flatland.
```

---
## \#212 Posted by: Ackmaniac Posted at: 2016-11-14T15:06:53.578Z Reads: 274

```
Yes for 30 km/h you need roughly 300 till 350 watts in total. Depends on the efficiency of the drive train. Glad that you got it sorted finally. 

I also reduce the power when i give it to somebody else the first time. Because everybody underestimates the power when they see the small motors.

I once made the mistake to give the board to a boy who was like 30kg. And the board acted like it's doing a test run on the bench. Told him multiple times to be extremely careful but it din't help. So he was flying. Actually he didn't even ride a single meter, felt down at the exact spot where he started. 
Afterwards i decided to reduce the power drastically when i give it to somebody new.

It's really funny when my colleagues drive the first time with 250 Watts and tell me that it is very impressive and a nice toy. And then i ask them if they want to try it with 10 times the power (2500 Watts). 
Always funny to see the WTF face they make then. And there was only one guy wanted to give it a try.
```

---
## \#213 Posted by: SirDiff Posted at: 2016-11-14T15:17:23.669Z Reads: 263

```
How do you switch settings so fast?
```

---
## \#214 Posted by: Ackmaniac Posted at: 2016-11-14T15:26:09.975Z Reads: 298

```
I also programmed a android app with that i can save multiple modes and simply switch while i am riding. 
But it only works with my modded firmware. Because i don't want the board to keep the settings. Means when i switch the board on and off again it is back to default. It only sets it as default when i want it. That has some advantages when the cops stop me.
And the Vedder firmware can't do that.

Also it only works with Wifi via a ESP8266. Because i need this module to be smart to keep the max and min values by itself. Otherwise the smartphone needs to be connected all the time. This way i check the stats at the end of my run. But that app is something for another topic. 
But if somebody has a Wemos Mini D1 (ESP8266) then pm me and i can send the code and the app.

App looks like this, but i don't want to publish it yet because when i change the firmware i might have to adopt also this app. So i will do that when it is the time.
<img src="/uploads/db1493/original/3X/c/8/c8b0dd14f876d4bf38621a67bb88b683f5a8b366.png" width="281" height="500">
```

---
## \#215 Posted by: yaca Posted at: 2016-11-14T15:46:37.614Z Reads: 268

```
Maybe it was a bit less than 30km/h with 2x250 watts, I forgot my phone to take with. 
Now I tested with 2 x 500 watts and changed the Soft RPM Limit to 30.000. I only got 32km/h. Next I will try to give more Max watt and see if this will give higher speed. If not I go higher with Soft RPM Limit to see where is the top.
```

---
## \#216 Posted by: Ackmaniac Posted at: 2016-11-14T15:48:28.987Z Reads: 263

```
Forgot that you have hub motors. So i can't tell you how they perform. But keep on sharing your experiences.
```

---
## \#217 Posted by: Ackmaniac Posted at: 2016-11-14T16:42:05.621Z Reads: 273

```
Currently i ma still working on the softened edges for the throttle-curve implementation which i will implement hopefully today.

But afterwards i think about it to add watt control also to the brakes. Because there we have the same issue like with the acceleration in current control. When i go full speed then 40% braking-throttle is already enough to brake 100%. So also there the throttle range is lost. Will be interesting to test this and see how it feels. But i guess it will make the brake much more controllable. Even more than the acceleration.
I keep you updated.
```

---
## \#218 Posted by: Ackmaniac Posted at: 2016-11-14T23:07:13.188Z Reads: 287

```
I added the new feature to soften the throttle curve edges. this way the throttle curve feels very natural. But i still left the possibility to keep the hard edges. the smoothness of the curve is now adjustable via the red marked number box in the second picture. Just try it out. Also the calculations in 10% steps are now visible in the diagram.
By adjusting how curve the edges should be it is still possible to adjust very extreme curves. So with the box you can adjust how curve it should be to fit your needs.

**Hard edges**
<img src="/uploads/db1493/original/3X/0/2/02b6e8e50c23fb6128e7d51d361a26e94841a08d.png" width="690" height="411">

**Soft edges**
<img src="/uploads/db1493/original/3X/8/6/864717ea30ea0edab57438e3a0786fe675077001.png" width="690" height="410">

This is version 2.51.
```

---
## \#219 Posted by: chinzw Posted at: 2016-11-15T01:40:02.497Z Reads: 257

```
@Ackmaniac great work dude! I've been using watt mode for about 2 days, and between that and the ppm center im loving it.  Its very predictable and responsive.
```

---
## \#220 Posted by: Ackmaniac Posted at: 2016-11-15T13:16:47.389Z Reads: 257

```
Great to hear that. Did you also try the throttle curve adjustment?
```

---
## \#221 Posted by: chinzw Posted at: 2016-11-15T17:00:40.609Z Reads: 258

```
I haven't. I like my linear throttle curve :slight_smile:
```

---
## \#222 Posted by: Ackmaniac Posted at: 2016-11-16T01:00:20.518Z Reads: 279

```
You should give it a try.  It is really nice to reduce the power at the low throttle range till 50 %.  Makes carving at mid to higher really nice and smooth. If you only go full speed all the time then you don't need it. My board for example does 50 km/h max and carving at 30 till 35 is the best for me. And at those speeds the reduced power output from the throttle is really nice.

Right now I work on the implementation that watt control also works for braking. I am really interested how it would feel. But if it is good I still will leave the possibility to switch it off so that it works like it does right now. Actually braking is the same as in current control.
And If it is great then I might also implement the throttle curve adjustment for braking. Oh and also for the nunchuk. 

What would be another feature the community wants. Maybe you have some great ideas? 

And can anybody tell me if it would be OK for a single drive to connect one channel of the remote to the servo connector and the other one to the adc channel inclusive the GND and TV or 3.3 volt pin. Or could that create a short? And on how many volts do the remote channels run? Because this way the cruise control also could  be activated for a single drive.
```

---
## \#223 Posted by: chinzw Posted at: 2016-11-16T01:07:07.910Z Reads: 253

```
I have my board limited to 15km/h so im pretty much full throttle all the time. And i do like the torque at startup that i have, i can get to full speed in a few meters :slight_smile:
```

---
## \#224 Posted by: SeanHacker Posted at: 2016-11-19T19:18:40.575Z Reads: 248

```
Bumping this thread up because this BLDC_Tool is awesome. More people need to see this.
```

---
## \#225 Posted by: Ackmaniac Posted at: 2016-11-19T19:57:49.980Z Reads: 255

```
Just a update. Currently I am working on watt control for braking. But we had a huge thunder storm 2 days ago and the roads are still whet and full of dirt. And with the next release throttle curve adjustment will also be available for nunchuk.
```

---
## \#226 Posted by: chinzw Posted at: 2016-11-20T16:58:02.107Z Reads: 245

```
1st week report: Flawless! Been using watt mode, with linear curve throttle and 1000w, just perfect!
```

---
## \#227 Posted by: Pimousse Posted at: 2016-11-20T19:12:54.206Z Reads: 245

```
Hey @Ackmaniac, I uploaded the VESC firmware and had the crash I mentioned before with BLDC Tool.
But this time I double checked the terminal, and here is the message after a crash (happened at the end of the firmware upload).

> Segmentation fault (core dumped)
```

---
## \#228 Posted by: Ackmaniac Posted at: 2016-11-20T19:16:40.585Z Reads: 245

```
Then it must be related to the fact that you use the Ubuntu version via a virtual machine. But just restart it and it should be fine. Bit annoying but i also don't have a better idea at the moment. When i find the time i will try to get it running for Mac. Maybe i need your help for that to test it because i don't have a Mac.
```

---
## \#229 Posted by: Pimousse Posted at: 2016-11-20T19:40:31.891Z Reads: 263

```
I rebooted the VESC via Reboot button and it did the same.
Restarting my VM doesn't fix the issue either.

Anyway, I don't reboot so much time, so it's not so annoying.
I now play with your curve "softener". I put your values (forked in the screenshot of the first post) and put 0,4 coeff for softening. It looks great.
Now, I have to try ! :slight_smile: 

Just some feedbacks : you can lock chart scales because we don't have to move it.
And dealing the the screen resizing to see status bar or parameters is a pain ! :neutral_face:

<img src="/uploads/db1493/original/3X/f/3/f334e546af634aa327cf969f8c41e7f9f32a4e08.png" width="689" height="453">

EDIT : of course, I'm your man for Mac testing ;)
```

---
## \#230 Posted by: shiro836 Posted at: 2016-11-22T07:33:03.150Z Reads: 248

```
Loving the watt control mode! Could you also include the throttle curve for nunchuk as well?
```

---
## \#231 Posted by: Ackmaniac Posted at: 2016-11-22T09:39:19.542Z Reads: 254

```
That feature comes with the next release
```

---
## \#232 Posted by: gaetjen Posted at: 2016-11-22T21:13:43.257Z Reads: 263

```
Hey, just tested your new bldc tool with watt control mode and it works flawlessly. I have a dual 190kv motor setup with a 10s battery and a winning remote. Since the change; I have a lot more throttle range than before and that makes for a much smoother ride. Thanks for the great work. I set the define max watt to 1600 and the erpm limit end to 60000. Hope that's right. 
Does the cruise control without accerlation work? I live in Germany and it would be nice to have that option since it's still illegal. Even better if you have that app of yours where you can switch to that mode in an instant.
```

---
## \#233 Posted by: E-Boarding Posted at: 2016-11-22T21:56:46.092Z Reads: 264

```
> Does the cruise control without accerlation work?
It works but it's no fun to ride that way, I'm not able to push to a decent speed that is usefull for commuting.
Best use is for a police-switch, not for regular usage imho.
```

---
## \#234 Posted by: yaca Posted at: 2016-11-29T20:25:38.345Z Reads: 260

```
Are you going to make your source code public? I ordered a bluetooth module from @rpasichnyk and now I realized I can not use his mobile apps with your firmware. He says he could support your firmware if you make the source code public. This would be great.
```

---
## \#235 Posted by: Ackmaniac Posted at: 2016-11-29T20:29:18.108Z Reads: 261

```
I will make it public soon. Working on the last bit.Found out that watt control for braking doesn't make sence because it seems that the VESC doesn't detect the watts correctly during braking, so i leave it as it is. But i will introduce throttle curves for braking.
```

---
## \#236 Posted by: jmasta Posted at: 2016-11-29T21:46:38.698Z Reads: 255

```
Great progress, @Ackmaniac! I'm going to have to give this a shot.  My board has way too much torque on the low end
```

---
## \#237 Posted by: Ackmaniac Posted at: 2016-11-29T22:02:58.193Z Reads: 257

```
Please post your motor settings. Because if it is at the very low end then maybeyour motor max are too high. But by adjusting the throttle curve you could also improve that.
```

---
## \#238 Posted by: Ackmaniac Posted at: 2016-12-02T10:43:11.413Z Reads: 288

```
I provided a new version of the modified firmware. Now it is possible to adjust the throttle curve for braking. 
And throttle curves are also available for Nunchuk's.
The setup is now in an own tab in the application configuration to have a bit more space, because some users had problems with the screen resolution.

<img src="/uploads/db1493/original/3X/2/c/2c34c8e926be61b11a4e4a54a1d52665492f0ef0.png" width="690" height="443">

If you want to honor my work you can use the donations link on top of this page.
Or if you want to buy a raptor 2 you can also use this link ([Raptor 2](http://www.enertionboards.com/raptor-2-direct-drive-electric-skateboard/?setCurrencyId=2&afmc=6q)) to get 100 $ discount and i would get the same as well. So it would be a win win.
```

---
## \#239 Posted by: rmrf Posted at: 2016-12-02T17:56:35.897Z Reads: 266

```
Are you working for enertion now? Noticed the screenshot at his kickstarter campaign https://www.kickstarter.com/projects/668913678/most-powerful-direct-drive-electric-skateboard-rap?ref=nav_search looks almost exactly like the one you attached.
```

---
## \#240 Posted by: Pimousse Posted at: 2016-12-02T20:18:46.063Z Reads: 274

```
Glad to see that you could take benefit from your great work being a partner of Raptor 2 project.

I uploaded your latest version and customed my throttle curve.
Let's play with it ! :smiley: 

<img src="/uploads/db1493/original/3X/4/2/4256bb23114283866eca5e9f78d957041b34c27c.png" width="655" height="500">
```

---
## \#241 Posted by: CamBo Posted at: 2016-12-03T00:07:54.554Z Reads: 268

```
@Ackmaniac Braking curve is SWEET!  Lots of hills where I live, and there was no way to have proper braking before.  Either too grabby or too weak.  Now I have a soft initial brake with plenty of power later in the stroke.  AWESOME WORK!
```

---
## \#242 Posted by: CamBo Posted at: 2016-12-03T00:12:04.956Z Reads: 277

```
An installation question:
If I have a dual motor system running over CAN, Do I have to update the slave every time I update the master?  I went from 2.51 to 2.52 without updating the slave.  Is this ok?  It seems to run fine.  Or should I update the slave?
```

---
## \#243 Posted by: Ackmaniac Posted at: 2016-12-03T00:14:54.420Z Reads: 271

```
It would be better to update the slave. The can bus commands are still the same so it should be fine, but just to be sure it would be better.
```

---
## \#244 Posted by: gaetjen Posted at: 2016-12-03T12:23:31.788Z Reads: 270

```
@Ackmaniac really like your work. Is it possible for you to work with @rpasichnyk, so you can combine both features. It would be awesome to adjust the throttle curve whilst riding via his bluetooth app
```

---
## \#245 Posted by: SeanHacker Posted at: 2016-12-03T21:22:59.117Z Reads: 300

```
@Ackmaniac

You're the pro here. I've still gotta lot to learn. Here's what I'm working with. I have a dual Raptor. I just put 100mm wheels on because the streets where I live are crazy with cracks, potholes, ect... I noticed after doing that I lost a little bit of torque (normal) and gained some top speed (also normal). One thing I noticed is that I lost a bit of braking which I'd like to get back. Here are my settings. Any advice? Also. Does it look like I have the right settings set as far as my battery, ERPM, ect...?

<img src="/uploads/db1493/original/3X/5/c/5c8232b54da0a5bae80361a7e609cff786a892fc.png" width="689" height="462">
<img src="/uploads/db1493/original/3X/8/6/860c52e5d4e2d6d539727e8359914d3e62d0613a.png" width="690" height="461">
```

---
## \#246 Posted by: Ackmaniac Posted at: 2016-12-03T21:26:04.097Z Reads: 270

```
Raise the motor min to -60. For the battery that is no issue but your belts might don't like that.
```

---
## \#247 Posted by: SeanHacker Posted at: 2016-12-03T21:37:52.368Z Reads: 285

```
Thanks a lot. I'm not worried about belts. :slight_smile:

<img src="/uploads/db1493/original/3X/b/e/be526027718fd31a5a0382c1a60d23b3414e0ba3.jpg" width="375" height="500">
```

---
## \#248 Posted by: Ackmaniac Posted at: 2016-12-03T22:00:18.755Z Reads: 264

```
The problem is that the belts can slip because the stress for the belts is higher at braking. But just try it.
```

---
## \#249 Posted by: ninja Posted at: 2016-12-03T22:14:51.508Z Reads: 265

```
What max. wattage i should put for my throttle curve? I have 8s 8000mah battery with SK3 245kv motor. At the moment i have 1000w max. watt!
```

---
## \#250 Posted by: SeanHacker Posted at: 2016-12-03T22:20:28.033Z Reads: 259

```
-60 was a bit too much. -50 seems just about right for me. Thanks!
```

---
## \#251 Posted by: Ackmaniac Posted at: 2016-12-03T22:20:54.916Z Reads: 262

```
Just calculate your battery max amps * 3,6 * 8 cells
EG.  30A * 3,6 ' * 8 = 864
```

---
## \#252 Posted by: ninja Posted at: 2016-12-03T22:22:31.575Z Reads: 256

```
I'ts lipo battery so the numbers the same?
```

---
## \#253 Posted by: Ackmaniac Posted at: 2016-12-03T22:26:46.130Z Reads: 253

```
Just raise your battery max if you want more.
```

---
## \#254 Posted by: ninja Posted at: 2016-12-03T22:46:00.741Z Reads: 259

```
What is max. for my battery, for now it's 40A in bldc tool.
```

---
## \#255 Posted by: Ackmaniac Posted at: 2016-12-03T22:47:44.258Z Reads: 258

```
Then 40A * 3,6V * 8S = 1152 watts
```

---
## \#256 Posted by: ninja Posted at: 2016-12-03T22:57:48.754Z Reads: 261

```
O.K. thanks! But that 3.6v for lipo should be 3.7v?
```

---
## \#257 Posted by: Ackmaniac Posted at: 2016-12-03T23:03:11.319Z Reads: 272

```
That's true. In watt control I set the maximum my battery can handle and then set the max watts lower so that I never have an issue with it. This way I have the same power output even when the battery gets lower. You could even set the battery max extremely high and then set the max watts to 250 watts and it would drive very gentle. Max battery in watt mode is only there to protect the battery if somebody enters crazy max watts values.
```

---
## \#258 Posted by: ninja Posted at: 2016-12-03T23:06:10.455Z Reads: 275

```
I see, so i'll put those 1152 watts with my battery max. set at 40A and i'll be on safe side isn't it?
```

---
## \#259 Posted by: Ackmaniac Posted at: 2016-12-04T00:33:00.083Z Reads: 315

```
Lets say you put it to 2000 watts. In this case the calculation for the throttle would tell the VESC to draw 2000 watts which it tries. But the max battery value forbids that. So you would feel that more than 60% throttle doesn't give more power. So you should not set it higher than my calculation to don't loose throttle range.
```

---
## \#260 Posted by: Ackmaniac Posted at: 2016-12-05T13:01:54.875Z Reads: 334

```
I created a Android app that works together with my modded firmware to watch the actual motor values and to quickly change the motor settings. You need a standard HM-10 Bluetooth low energy device for that. 
https://de.aliexpress.com/item/HM-10-BLE-Bluetooth-4-0-CC2540-CC2541-Serial-Wireless-Module/32516357718.html?spm=2114.13010608.0.0.cbyTeS&detailNewVersion=&categoryId=400103

So you need the latest version of my firmware and a standard HM-10. If you are interested to test the app then send me your email via pm and i will send you the file. 

But it really only works together with the HM-10. Otherwise you can't see anything in the app because the connection to the module is the starting point. You also can then host multiple boards with different setups because each bluetooth module is handled individually.

The cool thing is that you can record the screen while you are riding with another app to analyse your ride later on. that also lets you understand much better how the VESC works.

The app looks like this (not a actual picture)
Have to make a video this evening. I think you will love the features.

<img src="/uploads/db1493/original/3X/8/5/8535fc5bab7a8b567d744f6a1480fa0ff2d0b99f.png" width="281" height="500">
```

---
## \#261 Posted by: Ackmaniac Posted at: 2016-12-05T13:52:45.032Z Reads: 305

```
I decided to do it in another way. Currently i am adding the app as a beta version to my google play store account. So i will share the link here later so that anybody can try it.

My aim with this app is give it for free and count on donations. **(I know that is a bloody stupid idea :joy:)**

Because of that i add here the donation link again.
[Donations](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=4R86CGGZDVE9W)
Or if you want to buy a Raptor 2 and want to save 100$ and support me with 100$.
[Raptor 2](http://www.enertionboards.com/raptor-2-direct-drive-electric-skateboard/?setCurrencyId=2&afmc=6q)
```

---
## \#262 Posted by: Ackmaniac Posted at: 2016-12-05T15:54:57.497Z Reads: 298

```
And here is the link for the app

[VESC Monitor App](https://play.google.com/apps/testing/ackmaniac.vescmonitor/join?hl=de)
```

---
## \#263 Posted by: SageTX Posted at: 2016-12-05T16:09:14.146Z Reads: 298

```
Does the app support dual vesc?
```

---
## \#264 Posted by: rmrf Posted at: 2016-12-05T16:28:07.551Z Reads: 296

```
How about pushing the firmware and BLDC-tool code to github? They both are licensed under GPL, you are bound by this license. Please do it as soon as possible as you are violating our right (the end users) to 
> "study, share and modify the software"

https://www.gnu.org/licenses/gpl-3.0.en.html
```

---
## \#265 Posted by: ninja Posted at: 2016-12-05T17:49:42.550Z Reads: 288

```
How can i know how much A my battery can handle?
```

---
## \#266 Posted by: Ackmaniac Posted at: 2016-12-05T18:15:17.896Z Reads: 285

```
@SageTX The app doesn't really support dual VESC. It does update the slave vesc with the settings when the motor settings have been changed via the app. And it just doubles the realtime data values if you have 2 vescs. But it doesn't detect the values of the second one individually.

@rmrf Do i have to share my code via Github or is it enough when i provide the code at my dropbox account? Never used Github before.

@ninja just take the C rating of the batery and multiply it by the amp hours and the bateries in parallel.
A 10S4P with Samsung 25R cells (2500mah = 2.5ah) would be 2.5 * 8C * 4P = 80 amps.
```

---
## \#267 Posted by: SageTX Posted at: 2016-12-05T18:34:31.968Z Reads: 275

```
Great! Was wanting the ability to change modes so that'll do!
```

---
## \#268 Posted by: rmrf Posted at: 2016-12-05T19:03:04.600Z Reads: 283

```
[quote="Ackmaniac, post:266, topic:12286"]
Never used Github before
[/quote]

How did you get BLDC-tool source code then? :smirk: GitHub is the best and recommended way to do it. Dropbox is kinda OK in a sense that you will at least stop violating the license. The downside of Dropbox is that it's not easy to see the updates that you are making each time and contribute.
```

---
## \#269 Posted by: ninja Posted at: 2016-12-05T19:58:18.789Z Reads: 279

```
I got crazy number that way, so 8S1P 30c 8000mah = 30 * 8 * 1 = 240 A can i put this value like battery max.?
```

---
## \#270 Posted by: SeanHacker Posted at: 2016-12-05T20:07:50.843Z Reads: 290

```
@Ackmaniac You don't have to upload to git or any other source repository legally because you've already done that by releasing the zip with the source in your dropbox. It's just easier if you upload to git so we will be able to see the changes you've made and we can submit code back to you. You'll probably be receiving a ton of help if you do upload to git. It's the spirit of opensource. :)

Samsung does exactly what you did and release in one huge blob in your dropbox. They are forced by law (under gpl) to release source for their kernel. So what they do is release in a tar ball which is a mess and we can't see their changes made. It's a diffs worst nightmare most of the time.
```

---
## \#271 Posted by: Ackmaniac Posted at: 2016-12-05T20:22:28.772Z Reads: 294

```
Honestly it isn't my aim to protect my source code. Just don't find the time to deal with github. Tried once but failed. And i wanted to finish my changes and features before people begin to discuss about my code. And at the moment i am working in the app integration when i find the time.

All of the stuff from me is for free. Even the app. 
The people who complained that i didn't make it public are those who want to integrate it to their stuff where they charge money for it.
Till now i got 20 Euros of donations. Which is like 10 cent the hour or so. But i still continue for the fame :joy:
But money makes the world go round.

What makes me happy is that Benjamin Vedder took over a lot of my features to the new VESC tool. So everybody can profit by that. Sadly he never mentioned it before i pointed on it. Little thanks would have been cool. But on the other side i have to thank him for his amazing work that became my most beloved hobby.
```

---
## \#272 Posted by: rmrf Posted at: 2016-12-05T20:43:00.508Z Reads: 292

```
[quote="SeanHacker, post:270, topic:12286"]
you've already done that by releasing the zip with the source in your dropbox
[/quote]

The source code for firmware is missing. I would not write it here if the code was public. It is not.

[quote="Ackmaniac, post:271, topic:12286"]
All of the stuff from me is for free
[/quote]

This is not about free / non-free. This is about licensing and doing things right. Please let's stay on topic. The source code for firmware must be published because of GPL.
```

---
## \#273 Posted by: gaetjen Posted at: 2016-12-05T20:50:50.140Z Reads: 289

```
I'm definity going to donate when I get the module and tested everything. But because I ordered from aliexpress, it could take awhile
```

---
## \#274 Posted by: Ackmaniac Posted at: 2016-12-05T22:40:49.818Z Reads: 298

```
Here is a quick video of the app.

https://youtu.be/nuX9tiKtcVY
```

---
## \#275 Posted by: Brad Posted at: 2016-12-05T23:38:53.911Z Reads: 284

```
The work you are doing is wonderful.

Much appreciated, will donate some dough once I do get around to using it for real.
```

---
## \#276 Posted by: SageTX Posted at: 2016-12-06T01:27:44.787Z Reads: 277

```
That looks so cool. Will try to set up mine this weekend. Thanks for your time and effort into this project.
```

---
## \#277 Posted by: Ackmaniac Posted at: 2016-12-06T01:29:32.718Z Reads: 280

```
Just have to say that the app still has some bugs but I am working on it when I find the time. For example disconnect and connecting again seems to have a problem. But as long as you stay connected it is fine.
```

---
## \#278 Posted by: Ackmaniac Posted at: 2016-12-07T19:41:15.134Z Reads: 283

```
Did anybody test the app yet? Some feedback would be cool.
```

---
## \#279 Posted by: Pimousse Posted at: 2016-12-08T18:16:28.869Z Reads: 302

```
Hey,

I'm giving it a try.
First inputs :
- I had a couple of crashes especially when I want to go back to board selection
- Battery setup : replace capacity in Wh by mAh (more useful)
- Add datalogging feature
- Let user able to select baudrate (maybe in a Advanced menu). I often use VESC Connect for datalogging, it uses 115200 baudrate.
So switching from an app to the other forces me to re-parameter the VESC via BLDC Tool.
- "Max ERPM" unit is "A" in mode setup
- Disconnect then connect again is not working (as you mentioned)
- Wider pop-up menu for selecting the drive mode. Parameter are also unreadable.

Otherwise, it's a fuc@#% good job !!
I create a beginner drive mode limited to 2000 ERPM (for testing), it works very well !
This will bring me peace of mind when I'll give my board a try to begineers. :slight_smile:
Just add datalogging and I'll definitely use it as my new ride companion !
```

---
## \#280 Posted by: Ackmaniac Posted at: 2016-12-08T18:34:48.836Z Reads: 294

```
Thanks for the very detailed feedback. To video record the data while you ride I can recommend the "record master"  app. Works very well for me. As far as i know it isn't possible to switch to 115200 baud rate via Bluetooth (smartphone). You have to connect via serial and Programm the hm-10. And I want that they work out of the box so that people can simply order them anywhere and connect it. Or do you use the same hm-10 module without reconfiguring?

https://m.apkpure.com/record-master-screen-recorder/com.duapps.screen.recorder
```

---
## \#281 Posted by: Pimousse Posted at: 2016-12-08T18:38:17.508Z Reads: 291

```
Well I'd rather use a .csv or .txt file to be exploited in Excel sheet.
I made a spreadsheet with macros to exploit VESC Monitor datalog (from Solarturtle), it's very useful.
I'm hoping to do the same with yours ;)
```

---
## \#282 Posted by: E-Boarding Posted at: 2016-12-08T20:35:22.174Z Reads: 303

```
do this work with Dual-Setup, can I setup ride-modes and change both VESCs?

btw. great work
```

---
## \#283 Posted by: Ackmaniac Posted at: 2016-12-08T20:47:39.525Z Reads: 302

```
You have to connect it to the master vesc. Then the updates are done to both automatically when they are connected via CAN.
```

---
## \#284 Posted by: SeanHacker Posted at: 2016-12-11T03:58:54.056Z Reads: 314

```
Hey @Ackmaniac I just tried your app but I couldn't get it to work properly. I just got the balls to do my first solder job ever and connect this bluetooth module I bought a while back http://miamielectricboards.com/shop-1/vesc-bluetooth-adapter. The app connects to it no problem but I can't get it to changes modes or anything. Here's a vid if it helps. I'm thinking I might be missing something in BLDC_Tool or something. Do I need to be in UART/PPM mode for it to work? Or is just PPM mode good?

 https://www.youtube.com/watch?v=tZAG3zThfV4&feature=youtu.be

Hopefully I hooked this up right. I see it when I connect to bluetooth and it connects. Like I said. My first ever solder job.
<img src="/uploads/db1493/original/3X/c/9/c9755f50fcd3207896d98d004580cf197cc30caf.jpg" width="375" height="500">
```

---
## \#285 Posted by: lox897 Posted at: 2016-12-11T04:45:02.645Z Reads: 284

```
You need to be in PPM and UART
```

---
## \#286 Posted by: SeanHacker Posted at: 2016-12-11T04:48:10.339Z Reads: 282

```
Thanks. That's why it's not working.
```

---
## \#287 Posted by: thirdorange Posted at: 2016-12-11T15:48:42.309Z Reads: 285

```
Can you upload the apk somewhere? I don't have google play on my phone :confused:
```

---
## \#288 Posted by: Ackmaniac Posted at: 2016-12-11T16:34:48.926Z Reads: 285

```
I placed it to my Dropbox folder. You can find the link in the first post of this thread.
```

---
## \#289 Posted by: Maxid Posted at: 2016-12-12T13:05:35.669Z Reads: 293

```
Can you change the app to allow for baud rate settings? I have a HM10 set to 115200 and my VESC is set to the same - tried hooking it up and it connected but did not see anything from the VESC (not even the lab power supply voltage I used for the setup).
```

---
## \#290 Posted by: Ackmaniac Posted at: 2016-12-12T14:59:35.547Z Reads: 294

```
As far as i know it is not handled by the app. The communication between the Bluetooth module and the smartphone has no baudrate. It is only needed between the module and the VESC. So maybe check if the bluetooth module is really setup to a baudrate of 115200.
```

---
## \#291 Posted by: Maxid Posted at: 2016-12-12T15:27:24.568Z Reads: 289

```
Just checked - it is a cheap clone so BAUD is set to 8 which should mean 115200 according to the data sheet. Any other settings I need to change/reset?
I set the VESC to UART and 115200 Baud and the HM10 to a new name and Baud 8. Connected are 3.3V GND TX and RX (crossed so that RX on the module is connected to TX on the VESC and so on).
```

---
## \#292 Posted by: Ackmaniac Posted at: 2016-12-12T16:10:01.151Z Reads: 290

```
After you changed it to 8 please try if it works when you change the baudrate at the VESC to 9600. If that is the case then the change to 8 (115200) didn't work.
Anyway it isn't necessary to set the baudrate higher because it works fine with 9600. The amount of requests are handled by the app. So there won't be more data requests if the baudrate is higher.
```

---
## \#293 Posted by: Maxid Posted at: 2016-12-12T16:37:03.243Z Reads: 282

```
Nope still nothing. I changed it to factory settings (even though the 115200 settings were saved - otherwise my arduino softwareserial would have not been able to work properly) - and set the VESC to PPM+UART plus the baud rate to 9600. The App detects the module but displays only 0s - even for voltage.
```

---
## \#294 Posted by: Pimousse Posted at: 2016-12-12T20:11:39.708Z Reads: 291

```
I was wondering about the same feature (to choose the baudrate), but you're right, it's only for UART communication, not bluetooth.
And you're also right, the lower baudrate is, the better.
So I lower the HC05 baudrate so now both BT module are on the same baudrate ;)
```

---
## \#295 Posted by: Maxid Posted at: 2016-12-13T07:26:34.498Z Reads: 287

```
Anything else that I can try?
```

---
## \#296 Posted by: Ackmaniac Posted at: 2016-12-13T08:19:03.419Z Reads: 288

```
Can you post a picture of your module. Frontside and Backside? And you can download a Bluetooth characteristics analyse app and check which UUID you have for the Sierial (RX TX) communication.
The standard one is "0000ffe1-0000-1000-8000-00805f9b34fb"
```

---
## \#297 Posted by: Maxid Posted at: 2016-12-13T09:19:27.072Z Reads: 300

```
<img src="/uploads/db1493/original/3X/7/9/79aefcbddc9a4f311a439c55e6b9c284962ce093.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/5/3/539103bddc7f30d0a40c0b62376853690af317c8.png" width="281" height="500"><img src="/uploads/db1493/original/3X/b/6/b69b31ec164b5053c960241e3bd30b317e7a2817.jpg" width="375" height="500">
```

---
## \#298 Posted by: Maxid Posted at: 2016-12-13T09:28:43.597Z Reads: 283

```
Now it works - I changed the Power to 5V instead of 3.3V on the VESC after seeing the 3.6-6V on the back of the module. Seems like that fixed it. Thanks for the help and for the App :thumbsup:
```

---
## \#299 Posted by: Ackmaniac Posted at: 2016-12-13T09:48:15.766Z Reads: 280

```
Great. Thanks for the info. That's good to know. Because i never tried it with the 3.3V pin.
```

---
## \#300 Posted by: Maxid Posted at: 2016-12-13T09:49:21.296Z Reads: 284

```
Well not 100% sure if that actually was the culprit - but since I did not change anything else it is the  obvious conclusion.
```

---
## \#301 Posted by: SeanHacker Posted at: 2016-12-13T16:05:12.054Z Reads: 288

```
Can you tell me where exactly you changed the power to? I'm having the same issue.
```

---
## \#302 Posted by: Ackmaniac Posted at: 2016-12-13T16:05:53.316Z Reads: 299

```
The Vesc has a 3.3V and a 5V pin. Just connect VCC to the 5V pin.
```

---
## \#303 Posted by: SeanHacker Posted at: 2016-12-13T16:25:06.711Z Reads: 296

```
This might be out of my league. Is the 5v pin supposed to be labeled on the vesc or something? I just don't want to be plugging into something that will break anything. I'm a super noob.

<img src="/uploads/db1493/original/3X/6/6/6617825c6c4d1a2e327beb21056dbe78144401a5.jpg" width="281" height="499">
```

---
## \#304 Posted by: Ackmaniac Posted at: 2016-12-13T16:32:31.872Z Reads: 303

```
<img src="http://www.electric-skateboard.builders/uploads/db1493/original/2X/e/ea43a13722c878c33a812a3d20fb2efbba59af28.PNG">
Not so easy to add a picture via smartphone
```

---
## \#305 Posted by: Maxid Posted at: 2016-12-13T16:38:39.875Z Reads: 290

```
it is labelled on the other side.
From your view in the image on the bottom right (in the white plug) the leftmost pin is 5V, then 3.3V GND ADC TX RX ADC2
```

---
## \#306 Posted by: SeanHacker Posted at: 2016-12-13T16:43:52.058Z Reads: 299

```
Thanks guys. I have the pin switched. The problem for me still is nothing shows in the app. I can't select my modes and no info show. I was hoping this would fix it. Any ideas? 

<img src="/uploads/db1493/original/3X/f/0/f06ce6265a1d8fd83bd16f3b106e73db716be70a.jpg" width="281" height="499"> 
<img src="/uploads/db1493/original/3X/1/0/10d5218e1dfb7e81255f04dec96e3ccf880d097e.png" width="281" height="500">
```

---
## \#307 Posted by: Ackmaniac Posted at: 2016-12-13T16:48:38.858Z Reads: 271

```
Please make a screen shot of the general application setup and the uart setup of the vesc.  It needs to be ppm+uart and 9600. And the cable which is plugged to RX at the vesc needs to be in TX at the Bluetooth module. And TX vesc is RX module.
```

---
## \#308 Posted by: SeanHacker Posted at: 2016-12-13T16:54:18.078Z Reads: 287

```
Alright. So I need to switch another wire. I'll try that now. 

<img src="/uploads/db1493/original/3X/8/3/8304a283a0cbaaad8403b73d575d9fe3dab28f7c.png" width="690" height="459"><img src="/uploads/db1493/original/3X/2/b/2b589914b3237a03a003afc8e83652cc3720bc68.png" width="690" height="462">
```

---
## \#309 Posted by: Ackmaniac Posted at: 2016-12-13T16:55:53.457Z Reads: 256

```
Baud rate needs to be 9600 and not 96000.
```

---
## \#310 Posted by: SeanHacker Posted at: 2016-12-13T16:59:50.163Z Reads: 258

```
Works now! Thanks for being so patient and helping me out. Really cool of you.
```

---
## \#311 Posted by: SeanHacker Posted at: 2016-12-13T17:01:36.422Z Reads: 255

```
Last question. When I change modes will it apply it to both vesc's?
```

---
## \#312 Posted by: Ackmaniac Posted at: 2016-12-13T17:04:17.235Z Reads: 263

```
When you connected the Bluetooth module to the master and the VESCs are connected via CAN then yes.
```

---
## \#313 Posted by: SeanHacker Posted at: 2016-12-13T17:07:04.465Z Reads: 266

```
Awesome. Thanks again. Sent a donation your way. X-Mas, kids, and life has drained me lately. But I wanted to show my support. Your link was in another language and it kept giving and error so I just sent through my friends & family account. Let me know if you received it. Otherwise I will get crazy on PayPal. lol.
```

---
## \#314 Posted by: Maxid Posted at: 2016-12-13T17:07:17.271Z Reads: 270

```
so not possible with a nunchuck right?
```

---
## \#315 Posted by: Ackmaniac Posted at: 2016-12-13T17:11:09.022Z Reads: 268

```
No not really. It will show the values but the mode change won't work this way. Maybe I will provide a solution in the future. I know how to solve it but I need to find the time.
```

---
## \#316 Posted by: SeanHacker Posted at: 2016-12-14T06:08:23.964Z Reads: 260

```
I really hope you guys donate to @Ackmaniac. He's spent a ton of time on this project. We need to keep these kind of guys motivated and appreciated here. Wattage control has been a godsend!
```

---
## \#317 Posted by: Maxid Posted at: 2016-12-14T06:38:31.374Z Reads: 262

```
Understood - would be awesome. Also Android Wear support would get the App to the next level. Seeing the battery status for example on the watch would be the best battery indicator ever.
```

---
## \#318 Posted by: SeanHacker Posted at: 2016-12-14T06:41:16.417Z Reads: 288

```
If I had the source (because I wouldn't have the time to start from scratch) I would make that happen. You're definitely on to something there dude. :)

I'm pretty much stuck with raw source from the app. But If I can help in anyway i will asap! He's done an awesome job so far!

<img src="/uploads/db1493/original/3X/f/0/f046e9ce8284bc10157f5b04dffe64ddb72e79bc.png" width="690" height="291">
```

---
## \#319 Posted by: Ackmaniac Posted at: 2016-12-14T07:23:29.215Z Reads: 272

```
I think the next thing will be camera and video support. So you can record your ride. My aim is to help to understand how the vesc behaves. Maybe graphs will be added but I like the idea to minimize the actual screen in the video.
```

---
## \#320 Posted by: SeanHacker Posted at: 2016-12-14T07:46:26.813Z Reads: 275

```
That would be awesome dude.

P.S- One thing I like about what you do is that you don't force others to buy a product prior to using your work. That shows a lot. Keep doing your thing man. It'll pay off.
```

---
## \#321 Posted by: Pimousse Posted at: 2016-12-14T07:57:23.316Z Reads: 276

```
Awesome feature for sure !
But at least a feature that logs data into a .csv or .txt file (with gps data for real speed) would be a very useful tool to diagnosis the VESC behaviour.
As I said,  I'm using a lot this feature with solarturtle's VESC Monitor. it helps a lot to configure properly the VESC ;)
```

---
## \#322 Posted by: Ackmaniac Posted at: 2016-12-14T08:44:53.832Z Reads: 273

```
I made it for a XML file. But i also think a CSV file would be more useful and easier.
```

---
## \#323 Posted by: Ackmaniac Posted at: 2016-12-15T01:19:33.132Z Reads: 291

```
Nice update about the app. 
It is possible now to create videos with the VESC relatime data as overlay in the video. 
So it would be much easier to analyse the behavior of the vesc in different situations. 

At the moment only the main camera can be used for that. The video can then be found in the folder VESCMonitor on the device (not on the storage card). 
Please test it and let my know if there are problems. It will take a couple of hours for google to uplaod the new application file. If you can't wait get the file from my dropbox folder. 

Still some bugs, so please check when you start the video that the values get updated. Otherwise start the app again.

https://youtu.be/0y_CKa4OoKY

Please post some videos of your rides with the data. Would be nice to compare different boards with each other.
```

---
## \#324 Posted by: chinzw Posted at: 2016-12-15T04:47:00.117Z Reads: 272

```
Keep up the good work dude, this is just perfect :slight_smile:
```

---
## \#325 Posted by: onloop Posted at: 2016-12-15T04:59:33.454Z Reads: 279

```
WELL DONE.........

So much knowledge can be gained from this.
```

---
## \#326 Posted by: Kaden56 Posted at: 2016-12-15T05:10:16.642Z Reads: 275

```
Forgive me as I haven't been very good in keeping up with this thread and there are 324 comments now so I don't want to spend time to read all of them but can someone give me a general update on how this is going and who can use it? For example is it limited to any versions of Vesc? Is it a whole separate program or is it some kind of a plug in to the bldc tool I already have? Can I download it on my mac? What are the main advantages of it? Thank to anyone who takes the time to answer these questions.
```

---
## \#327 Posted by: Maxid Posted at: 2016-12-15T08:15:09.306Z Reads: 274

```
Why is the app called VESC Monitor in the play store but on device it is VESC Scanner?
```

---
## \#328 Posted by: Ackmaniac Posted at: 2016-12-15T08:30:35.611Z Reads: 276

```
@Maxid thanks for the info. I corrected that.

@Kaden56 For the Firmware and the BLDC-Tool the information can be found in the first post of this thread. But i have not created a MAC version yet. But as far as i know you can get the linux souces running on MAC.
The app is made for Android and needs a HM-10 Bluetooth module which you have to connect with your VESC.
You can buy it here.

https://de.aliexpress.com/item/HM-10-BLE-Bluetooth-4-0-CC2540-CC2541-Serial-Wireless-Module/32516357718.html?spm=2114.13010608.0.0.cbyTeS&detailNewVersion=&categoryId=400103
```

---
## \#329 Posted by: Pimousse Posted at: 2016-12-15T08:34:44.417Z Reads: 260

```
VESC Monitor already exists !
It's Solarturtle's one.
```

---
## \#330 Posted by: Maxid Posted at: 2016-12-15T08:57:12.460Z Reads: 260

```
So? I doubt there is a copyright on that name.
```

---
## \#331 Posted by: Ackmaniac Posted at: 2016-12-15T09:28:24.684Z Reads: 255

```
Wasn't my intention to copy his name. I can give it another name. But i also think it doesn't really matter.
```

---
## \#332 Posted by: Pimousse Posted at: 2016-12-15T10:16:35.138Z Reads: 264

```
@Maxid : Why talking copyright, patent and so on ?
There are just billion of different names possible for an app.
This is just to avoid being mistaken between several app (lot's of talented app dev on this forum resulting in so many app).

@Ackmaniac, Cool ! Your app is even more than a simple monitor as you also offer driving modes. ;)
```

---
## \#333 Posted by: The_Dude Posted at: 2016-12-15T10:29:23.027Z Reads: 259

```
So cool! Any chance to go for an iPhone Version (I'm suffering more and more the further you develop things)?
```

---
## \#334 Posted by: Maxid Posted at: 2016-12-15T10:31:42.649Z Reads: 266

```
VESC Monitor in Google play will only show @Ackmaniac's App.
The other one is called Vedder ESC Monitor - so there is already a distinction there.
Don't see a reason to change the name (I also like VESC Monitor).
```

---
## \#335 Posted by: Maxid Posted at: 2016-12-15T10:34:54.767Z Reads: 268

```
[quote="The_Dude, post:333, topic:12286, full:true"]
I'm suffering more and more the further you develop things
[/quote]

And you should for using an iPhone :stuck_out_tongue_winking_eye:
```

---
## \#336 Posted by: Pimousse Posted at: 2016-12-15T10:38:26.134Z Reads: 268

```
VESC Monitor
Vedder ESC Monitor

Completely different names :smile:
The point is Solarturtle's name is "VESC Monitor" once installed.
Anyway, it doesn't matter.
```

---
## \#337 Posted by: Ackmaniac Posted at: 2016-12-15T11:12:13.144Z Reads: 267

```
Sadly i never developed a app for a IPhone. And to do so you need a MAC and a IPhone which i don't have. Also the fees for a developer account are high. Around 100$ a year. Maybe in the future. 
But i think there are better IPhone programmers here in the forum which get inspired by the apps that are already available.
```

---
## \#338 Posted by: lox897 Posted at: 2016-12-15T11:50:35.196Z Reads: 262

```
Why is it saying that the app isn't compatible with my android?
```

---
## \#339 Posted by: Maxid Posted at: 2016-12-15T11:58:38.565Z Reads: 266

```
maybe OS version is too old?
```

---
## \#340 Posted by: lox897 Posted at: 2016-12-15T12:10:25.814Z Reads: 268

```
That could be it. It's a shitty $99 android anyway, I'll just use my iphone with another app
```

---
## \#341 Posted by: Ackmaniac Posted at: 2016-12-15T12:22:53.007Z Reads: 273

```
Video support is only given with Android 5.0 (Lollipop). I changed the software so that it can run from Android 4.3 (KitKat) where you could see the VESC realtime data.
But to make videos you need Android 5.0.

Google needs a while again for the updated Version. If you can't wait then use the file in the Dropbox link of the first post of this thread.
```

---
## \#342 Posted by: SeanHacker Posted at: 2016-12-15T14:07:43.341Z Reads: 331

```
You guys need to update your android OS. No need to stick to the old stuffs. Let me know if you need any help.  ;)

<img src="/uploads/db1493/original/3X/5/f/5f9982e5da26452730fc5cb0fa713b77b688bbaa.png" width="281" height="500">
```

---
## \#343 Posted by: mortorojo Posted at: 2016-12-16T21:59:03.420Z Reads: 305

```
Off topic request is there anyway you could get the LED's working as show in Vedder's video, [ESC nunchuk and ws2812 LEDs](https://www.youtube.com/watch?v=G8f0xg7DNmM) in conjunction with your Watt-Control?
```

---
## \#344 Posted by: Ackmaniac Posted at: 2016-12-17T19:47:11.153Z Reads: 312

```
Realized that i didn't post a link for the Google Play Store for the app. So here it is

[App in Google Play Store](https://play.google.com/store/apps/details?id=ackmaniac.vescmonitor&hl=de)
```

---
## \#345 Posted by: Ackmaniac Posted at: 2016-12-17T19:48:43.174Z Reads: 314

```
I don't have a Nunchuk and i don't have lights on my board. Of course it would be interesting to add light support but i didn't spent time on that. In Germany you try to be as stealth as possible.
```

---
## \#346 Posted by: Eboosted Posted at: 2016-12-18T06:28:26.295Z Reads: 315

```
@Ackmaniac your tool is amazing, thanks for your colaboration with the community.

I'm still on the build process, waiting impaciently on my battery pack and remote, but would like to know if there is anyway I could flash the firmware and tinker with you modded BLDC tool as I already got the VESCs and motors without risking the VESCs hardware or DRV chip

OTOH, is this the correct bluetooth hardware to connect the datalogging android app or it has to be exactly the one you pointed on Aliexpress?

https://www.amazon.com/Industry-Park-Bluetooth-Transceiver-Central/dp/B01LYFXIAE/ref=sr_1_3?ie=UTF8&qid=1482035472&sr=8-3&keywords=HM-10+BLE+Bluetooth+4%2C0+CC2540+CC2541
```

---
## \#347 Posted by: Ackmaniac Posted at: 2016-12-18T09:53:37.479Z Reads: 289

```

The linked module has no pins. So it would be a tough soldering task. 

Better would be this module if you want to order it in the states. But i don't know for 100% if it works. But it should do the job. 
https://www.amazon.com/Qunqi-Bluetooth-HM-10-Module-Conversion/dp/B0140R8DGQ/ref=sr_1_4?ie=UTF8&qid=1482054708&sr=8-4&keywords=bluetooth+hm-10

But i still recommend this here. The price is hardly beatable.
https://de.aliexpress.com/item/HM-10-BLE-Bluetooth-4-0-CC2540-CC2541-Serial-Wireless-Module/32516357718.html?spm=2114.13010608.0.0.cbyTeS&detailNewVersion=&categoryId=400103
```

---
## \#348 Posted by: Ackmaniac Posted at: 2016-12-18T17:07:29.587Z Reads: 272

```
I provided a update of the actual Android app. Now it is possible to adjust the video and sound quality and the realtime data size in the video is also adjustable.
Made some changes to the code so that the connection should be more stable now and the connect button should also work now.
In the background a CSV file of the realtime data ad GPS position and altitude gets created each time the app is connected to the VESC. This can be found on our device in the folder VESCMonitor.

And as always Google Play Store needs a while or this version 11. So if you can't wait you can download the app in the dropbox link in the first post of this thread.
```

---
## \#349 Posted by: DreadBiscuit Posted at: 2016-12-19T18:35:46.328Z Reads: 274

```
[quote="Ackmaniac, post:1, topic:12286"]
Here are some additional install instructions. Read them before please:

Be aware that this is only for Hardware Version 4.10 or above.

Important: You have to flash the Firmware with this modified BLDC-Tool.Flash the Firmware directly. Otherwise this can cause trouble. 


Open the downloaded BLDC-Tool 
Upload the new Firmware which is attached to this email.
Check the default values in the new BLDC Tool. When these are OK then you can use it. If the vaules are creazy then flash the firmware again.
Adjust the settings of your VESC. I would not recommend to use a saved config. It would be better and safer to set the values manually. So you should make screenshots of your old setup or write it down.
[/quote]

I have some questions about this.  The firmware needs to be **uploaded to the VESC upon first connection before reading VESC settings or before reading Firmware version?**

What does "Flash firmware directly" mean? 
What does default values do I need to make sure are ok?  How will I know if they are crazy?

Any help would be appreciated. Edit: I am using a TB VESC 4.12 on Windows 10.  I have already downloaded your BLDCtool and 2.52 firmware Here is a screenshot of what I am waiting to do.  All I need to do is power up, plug in USB and upload firmware to board after I hit 'Connect'?  
<img src="/uploads/db1493/original/3X/b/2/b23047d233753fc45aadf39c5ef477450ed6b6c8.JPG" width="690" height="387">
```

---
## \#350 Posted by: Ackmaniac Posted at: 2016-12-19T18:36:32.461Z Reads: 272

```
Made a little modification. When the VESC has a fault it will be shown  in the area of the red rectangle shown in the picture. Good thing is that even if the VESC shuts down and reboots it should be shown here.
<img src="/uploads/db1493/original/3X/2/2/22b3a06a224174d10c18731307ac9e5482c3d0b0.png" width="281" height="500">
```

---
## \#351 Posted by: Ackmaniac Posted at: 2016-12-19T18:38:41.087Z Reads: 250

```
by changing the Firmware version these problems are gone. So if the firmware version doesn't fit to the BLDC-tool version you have no other chance than flashing the firmware. So there is no chance anymore to do it the wrong way.
And yes you can upload after the connect. You can go back to the original firmware as long as you have the file at any time if you have the file of the original firmware.
```

---
## \#352 Posted by: DreadBiscuit Posted at: 2016-12-19T18:41:02.733Z Reads: 248

```
How do I save the original firmware before flashing yours?
```

---
## \#353 Posted by: Ackmaniac Posted at: 2016-12-19T18:42:23.428Z Reads: 244

```
You can't save it. But i guess they use the original firmware anyway.
```

---
## \#354 Posted by: DreadBiscuit Posted at: 2016-12-19T18:43:32.102Z Reads: 242

```
Thanks!  I can't wait to get this up and running! Ok, I got it uploaded.  Now I can go through like normal under motor configuration and read configuration from the VESC, and then configure as I want, right?
```

---
## \#355 Posted by: SeanHacker Posted at: 2016-12-19T19:10:31.637Z Reads: 240

```
@Ackmaniac Just a suggestion for the app if you get the time or want to. Maybe making an option for MPH (Speed) and miles (Distance & Range). That way those of us in the US don't have to do the math (for dummies like me).  :slight_smile:

Great job dude!
```

---
## \#356 Posted by: DreadBiscuit Posted at: 2016-12-19T21:03:47.587Z Reads: 242

```
I haven't configured everything, I have to re-read parts of this thread to make sure to do it right.  But @Ackmaniac, YOU ARE THE MAN!!  Thanks for the quick response on my questions.  I now have your version of BLDC setup on my board as well as the bluetooth working with the app right out of the box!  Just sent a donation - it's not much, but I know every little bit helps.  Your support is much appreciated!
```

---
## \#357 Posted by: Ackmaniac Posted at: 2016-12-19T21:12:36.868Z Reads: 250

```
Just added distance unit which can be adjusted in the drive setup. Thanks for the hint SeanHacker. Had this in a previous version but then completely modified it and forgot about it.
As always Google needs a while for the update. Who can't wait go to my Dropbox link and install it from there.

Thx DreadBiscuit for the Donation.
```

---
## \#358 Posted by: Ackmaniac Posted at: 2016-12-19T23:02:08.815Z Reads: 246

```
Ups, calculated Miles the wrong way accidentally in the app. That's fixed now.
```

---
## \#359 Posted by: jacobbloy Posted at: 2016-12-20T00:46:07.216Z Reads: 266

```
windows .exe installer
https://drive.google.com/file/d/0Bym9XrdeViekenJEZVdEb2pyelU/view?usp=sharing

OS X DMG
https://drive.google.com/file/d/0Bym9XrdeViekZ2xMeERmSjVWRkU/view?usp=sharing

the firmware has been added to the installers, in windows you will have to delete the old firmware folder in program files before the new firmware will replace it (small bug)

This is a great MOD to BLDC TOOL and the vesc FIRMWARE. through testing vesc tool with benjamin vedder he has added similar features for the vesc 6 and back dated but still using duty cycle. i thing current control is a lot better method for use with ppm.
 with @Ackmaniac i will put this up on my website with credit to @Ackmaniac but not untill he gives permission. thanks guys.
```

---
## \#361 Posted by: Ackmaniac Posted at: 2016-12-20T01:17:56.298Z Reads: 250

```
With the last version I also fixes a issue with the drive setup in the app. So if anybody experienced issues when you changed the values these should be fixed now as well.
```

---
## \#362 Posted by: Eboosted Posted at: 2016-12-20T06:36:41.662Z Reads: 251

```
In your BLDC TOOL have you modified the code where the max current ramp multiples by 10 when writting advanced settings? 

http://www.electric-skateboard.builders/t/psa-remember-to-reset-your-max-current-ramp-step-when-programming-your-vesc/6262
```

---
## \#363 Posted by: SeanHacker Posted at: 2016-12-20T06:39:25.691Z Reads: 249

```
That was a bug in the firmware quite a while ago. Not the tool. This firmware doesn't have that issue.
```

---
## \#364 Posted by: Maxid Posted at: 2016-12-20T14:26:05.483Z Reads: 234

```
Just donated - you might want to change that text from "Ackmaniac E-Longboard Developent" to Development ;)
```

---
## \#365 Posted by: Ackmaniac Posted at: 2016-12-20T14:37:40.581Z Reads: 233

```
Thx for the hint and for the donation.
```

---
## \#366 Posted by: onloop Posted at: 2016-12-20T21:29:24.597Z Reads: 230

```
Nice work @jacobbloy
```

---
## \#367 Posted by: SeanHacker Posted at: 2016-12-20T22:31:09.204Z Reads: 248

```
Gotta question. I read somewhere in the forum the other day about having to split up Motor Max when running dual vesc's/motors. So instead of having 60A for both vesc's in BLDC_Tool should they both be at 30A? I just don't want anything to break. Although I've been running this setup for months now. Just making sure. ;)

<img src="/uploads/db1493/original/3X/d/9/d97572192aa9e2f432b2a5b9aafd59446b6d97e9.png" width="690" height="448">
```

---
## \#368 Posted by: rpn314 Posted at: 2016-12-20T22:43:43.510Z Reads: 226

```
Eh, to be honest I would just worry about battery max (which I would split if you have a dual setup), because (in my opinion) it's easier to figure out what the limit should be since you just need to know what your pack can output. So for a dual setup, if your battery pack can output 50 Amps, put 25 Amps on the batt max to each VESC, and if can max charge (think regen) at 10 Amps, then put the batt min at 5 amps on each.
```

---
## \#369 Posted by: SeanHacker Posted at: 2016-12-20T22:46:34.538Z Reads: 226

```
Awesome. Thanks. I have a Raptor dual so it looks like I have everything set right for my board then.
```

---
## \#370 Posted by: Ackmaniac Posted at: 2016-12-20T22:47:02.470Z Reads: 230

```
60A is fine.  You can enter the max value your motor can handle for each vesc. 
For the max battery amps it is the opposite. You have to split the maximum the battery can handle by the amount of vescs.
```

---
## \#371 Posted by: SeanHacker Posted at: 2016-12-20T22:48:18.913Z Reads: 228

```
Thanks. I think I got the two (Batt Max & Motor Max) mixed up when I read that the other day. :dizzy_face:
```

---
## \#372 Posted by: Ackmaniac Posted at: 2016-12-20T22:59:44.773Z Reads: 222

```
And you should set the maximum input voltage to 57.
```

---
## \#373 Posted by: SeanHacker Posted at: 2016-12-21T00:42:15.004Z Reads: 231

```
@Ackmaniac Changed it. What does Maximum Input Voltage do?
```

---
## \#374 Posted by: Eboosted Posted at: 2016-12-21T07:36:30.972Z Reads: 231

```
What's the formula to calculate the maximum output in amps for a 10s4p with Samsung 25R?
```

---
## \#375 Posted by: Pimousse Posted at: 2016-12-21T07:46:44.544Z Reads: 234

```
4 x Nominal Amp of a Samsung 25R
```

---
## \#376 Posted by: Maxid Posted at: 2016-12-21T07:50:06.447Z Reads: 232

```
current is: 4 * 20A = 80A
```

---
## \#377 Posted by: Pimousse Posted at: 2016-12-21T09:46:53.919Z Reads: 230

```
As far as I know, VESC's are rated to 50A max continous (battery), aren't they ?
```

---
## \#378 Posted by: Ackmaniac Posted at: 2016-12-21T10:06:11.860Z Reads: 244

```
No it can't because it will overheat. But that is no issue because it reduces the power automatically when it gets too hot. For a belt driven dual drive you normally don't get issues. For a single drive it can happen that it gets too hot.
Simply set it to the value your battery can handle and you will be fine. So a 10S4P Samsung 25R can do 80Amps. But also check how much your fuse can handle. Maybe that is lower then the battery.

I also have a Vedder switch with a 40A fuse and I go up to 80A with no issues. But that is not recommended and at your own risk. But I never had issues and never blew a fuse. Because mostly you only draw high amps for a couple of seconds. When you go full speed on the flats then you are not even close to max amps.
```

---
## \#379 Posted by: marc Posted at: 2016-12-21T12:48:58.724Z Reads: 243

```
So I downloaded the Windows version from the OP, and my VESC is on 2.18 firmware. When I try to upload the 2.52 firmware, I can't find it. Is it a separate download? Sorry if this is obvious, I'm a bit of a newb.
```

---
## \#380 Posted by: DreadBiscuit Posted at: 2016-12-21T13:31:15.127Z Reads: 249

```
Yes, it's a separate download.  It's the file named "VESC_Ackmaniac.bin" on the download page from the first post.  I had this issue as well.  When you go to choose firmware, link to the location of this file once it is downloaded.

Here is a screenshot of what it should look like ('......' is hiding my path names as it has personal information from my laptop on it)
<img src="/uploads/db1493/original/3X/b/2/b23047d233753fc45aadf39c5ef477450ed6b6c8.JPG" width="690" height="387">
```

---
## \#381 Posted by: SageTX Posted at: 2016-12-22T01:09:27.926Z Reads: 237

```
Donated 20 euros.
Thanks for the work you put into this app and firmware, and the ongoing help and contribution to the community.  
Merry Christmas! 🎅🎅🎅
```

---
## \#382 Posted by: SageTX Posted at: 2016-12-22T04:53:01.859Z Reads: 238

```
OK.  Got the BT to connect.  

Only glitch I'm having is changing modes.  

I set up the modes,  but when selecting a mode, it won't change it like in the video.  I have to select it, disconnect, then reconnect before it changes settings.

Also locks up sometimes, requiring reset of the app. (dump from memory and restart)  That might be my phone though.  Samsung Note 3 running Android 5.0 Using the HM10 BTLE with resistors on the RX bt side.
```

---
## \#383 Posted by: DreadBiscuit Posted at: 2016-12-22T11:51:49.683Z Reads: 230

```
@SageTX - Why the resistors on the RX BT side?  What values?  I have used my BT once, and it worked but I haven't done any extensive testing or changing modes yet.
```

---
## \#384 Posted by: Maxid Posted at: 2016-12-22T12:05:47.828Z Reads: 229

```
he might have a HM10 without the breakout board. Then you need a voltage divider:
See http://www.hangar42.nl/hm10
http://i0.wp.com/www.hangar42.nl/wp-content/uploads/2015/08/voltagedividerhm10.png
```

---
## \#385 Posted by: DreadBiscuit Posted at: 2016-12-22T13:51:59.691Z Reads: 219

```
Oh, ok- makes perfect sense.  Yeah, mine has the breakout board.  Making sure I wasn't missing something.  I've read this whole topic twice now, working on the third time through and I'm still finding new information I missed the previous times.  There's so much good knowledge here.  Thanks!
```

---
## \#386 Posted by: SageTX Posted at: 2016-12-22T15:00:19.889Z Reads: 217

```
Yes. This.
```

---
## \#387 Posted by: Ackmaniac Posted at: 2016-12-22T18:40:30.016Z Reads: 245

```
I worked on my app and now there are some new features.
It is possible to choose the resolution of the video. Maximum allowed size is the size of your display.
<img src="/uploads/db1493/original/3X/5/8/5830632e3ec69286e10e466f7c053298a08cfdee.png" width="281" height="500">

I added a explorer with that you can have a look at your created video and CSV files
<img src="/uploads/db1493/original/3X/6/5/657cb90ffe5b9d7543137513da05450d6a13778f.png" width="281" height="500">

And it is possible to watch the Realtime data of the CSV files in Graphs.
<img src="/uploads/db1493/original/3X/f/7/f707a4eaf454e876f87e3d95cf617338b6e782b6.png" width="281" height="500">

As always google needs a little time for the upload. If you can't wait the apk file is avaliable at my dropbox link in the first thread.

Merry Christmas everybody.
```

---
## \#388 Posted by: Ackmaniac Posted at: 2016-12-22T19:12:40.015Z Reads: 213

```
I also forced the App to request the actual mode if unknown. So i think that should fix your problem that you couldn't see the mode changes.
```

---
## \#389 Posted by: SageTX Posted at: 2016-12-22T20:21:33.105Z Reads: 212

```
Yes. Works as expected now. Thanks!!!!
```

---
## \#390 Posted by: Ackmaniac Posted at: 2016-12-22T20:33:38.134Z Reads: 213

```
Awesome. Thanks again for the info.
```

---
## \#391 Posted by: Pimousse Posted at: 2016-12-22T21:54:13.581Z Reads: 210

```
No need of resistors with VESC because its Rx/Tx level is 3,3V and not 5V like Arduino.
;)

@Ackmaniac, thanks so much for the work on the CSV part !
Better than I could expect !
```

---
## \#392 Posted by: Maxid Posted at: 2016-12-22T21:55:16.624Z Reads: 212

```
Don't tell that to me but @SageTX ;)
```

---
## \#393 Posted by: SageTX Posted at: 2016-12-22T21:57:20.307Z Reads: 214

```
Well that would've been easier. Should I take them off?
```

---
## \#394 Posted by: Pimousse Posted at: 2016-12-22T22:08:59.466Z Reads: 221

```
@Maxid : oh sorry, wrong reply.
@SageTX : it works with (I'm in this case).
```

---
## \#395 Posted by: SeanHacker Posted at: 2016-12-23T00:06:27.664Z Reads: 234

```
@Ackmaniac I'm only asking here because I know you know your stuff. Only thing I changed in BLDC_Tool yesterday was Max input voltage from 50.0v to 57.0v as suggested. I was just cruising today and all the sudden I lost power. So I walked the board back home and ran the faults. This is what read out. I'm screwed now aren't I? Slave vecs still works. 

The following faults were registered since start:

Fault            : FAULT_CODE_DRV8302
Current          : 0.4
Current filtered : 0.2
Voltage          : 41.80
Duty             : 0.00
RPM              : 2.4
Tacho            : 3
Cycles running   : 1
TIM duty         : 263
TIM val samp     : 10
TIM current samp : 26384
TIM top          : 52747
Comm step        : 1
Temperature      : 21.06

https://youtu.be/g6qap-Id11k
```

---
## \#396 Posted by: Ackmaniac Posted at: 2016-12-23T00:53:20.657Z Reads: 226

```
Sorry to tell you that I don't have experience with drive faults. On like 2000 km I never fried a vesc. But the 57 can't be the issue. Did you run in FOC or BLDC? Does the vesc still run or is it dead? Maybe it helps when you post Screenshots of all the motor tabs again.
```

---
## \#397 Posted by: Eboosted Posted at: 2016-12-23T03:49:14.286Z Reads: 224

```
Does your VESC light the blue led and the 3 consecutive pinks ones? Where you on FOC?
```

---
## \#398 Posted by: SeanHacker Posted at: 2016-12-23T04:05:33.035Z Reads: 221

```
Yes. 

No FOC. I posted all my settings here http://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286/367?u=seanhacker . Only thing different was I changed the Maximum input voltage to 57v.
```

---
## \#399 Posted by: Eboosted Posted at: 2016-12-23T04:07:21.906Z Reads: 218

```
Damn! I see you did not do anything wrong, what VESC are you runing, DIYs?
```

---
## \#400 Posted by: SeanHacker Posted at: 2016-12-23T04:19:26.141Z Reads: 218

```
Enertion vesc. @onloop actually contacted me minutes after the post and told me that I will get a replacement after I email support. I bought a Raptor 1 and it falls under the 12 month warranty which is pretty cool. He said that he will replace it with a vesc-x. 

I already have two vesc-x's on order so I will probably just keep a spare one for my new build. I just ordered a vesc from @chaka (Ollinboards) tonight so I will just use that one for the Raptor. 

I'm just really glad it's winter right now!!! I really wish I could figure out what happened. It's been riding in that same setup for 2 months and I've had no issues with any part of that Raptor.
```

---
## \#401 Posted by: Eboosted Posted at: 2016-12-23T06:25:12.638Z Reads: 215

```
Wow that's really kind from @onloop

Did you see what was your max current ramp?
```

---
## \#402 Posted by: SeanHacker Posted at: 2016-12-23T06:51:48.804Z Reads: 214

```
I'm super new at this stuff. Do you mean when looking at the Realtime Data?
```

---
## \#403 Posted by: Eboosted Posted at: 2016-12-23T07:37:51.025Z Reads: 216

```
There were a lot of burnt VESC because this number was not set correctly, some versions of VESCs firmwares even multiplied this number by 10 and if you riden the  board the vesc would die. 

Check this number on your BLDC tool VESC settings
```

---
## \#404 Posted by: Ackmaniac Posted at: 2016-12-23T07:58:12.109Z Reads: 204

```
He used my firmware mod which never had that problem.
```

---
## \#405 Posted by: Maxid Posted at: 2016-12-23T07:58:15.464Z Reads: 214

```
according to @chaka this bug never actually affected any VESCs.
Not sure where you got the information from that "there were a lot of burnt VESC"
http://www.electric-skateboard.builders/t/why-does-my-slave-vesc-keep-blowing/14943/22
```

---
## \#406 Posted by: raxell Posted at: 2016-12-23T11:03:17.560Z Reads: 211

```
I have been riding my board with nunchuck and default VESC firm for 3 months and it has worked perfectly every day. But a few days ago I have a lot of random cutoff continuously. It is impossible to ride it now.
I have changed all the wires and still with the same issue. I have not fault code in VESC.

I am going to try your mod firm and BLDC and see if still the same issue using your watt mode. I think I read in your 400 replies that your watt mode works with nunchuck too, really?

Anyway, I am going to change my controller for PPM.

Thanks, your mod is an awesome idea!! good job!!
```

---
## \#407 Posted by: Ackmaniac Posted at: 2016-12-23T11:18:13.383Z Reads: 206

```
I changed the firmware to work with a nunchuk as well. But I don't have one so please test if everything works as expected. I guess others also use it already with a nunchuk but I don't know for sure. But your problems sound like remote connection issues so I also would recommend to change the remote.
```

---
## \#408 Posted by: Maxid Posted at: 2016-12-23T11:21:22.036Z Reads: 201

```
yep - I am using it with a nunchuck and with FOC
```

---
## \#409 Posted by: Ackmaniac Posted at: 2016-12-23T11:23:38.022Z Reads: 201

```
Thx for the info.
```

---
## \#410 Posted by: raxell Posted at: 2016-12-23T11:27:43.127Z Reads: 205

```
Thank you guys, I am going to try it. Let me read a little more before. I am a newbie :grin:
```

---
## \#411 Posted by: raxell Posted at: 2016-12-23T13:00:43.509Z Reads: 206

```
Installing your firmware I think I have found my problem. I'm going to solder the nunchuck receiver direct to the VESC. I have it now conected with JST plug.
I have now installed your mod. Do I have to do motor detection again before config all parameters?
```

---
## \#412 Posted by: Ackmaniac Posted at: 2016-12-23T13:09:48.146Z Reads: 210

```
You have to do the whole configuration again including motor detection.
```

---
## \#413 Posted by: raxell Posted at: 2016-12-23T20:59:37.372Z Reads: 208

```
Thanks @Ackmaniac i have fixed my issue with nunchuck soldering it to the VESC. I tried your watt mode just two minutes and i can say it feels good. Tomorrow i will give it a try long time.
```

---
## \#414 Posted by: yaca Posted at: 2016-12-23T21:30:11.668Z Reads: 208

```
Is there a reason to make motor detection again? I just took the values I had before with 2.18.
```

---
## \#415 Posted by: chaka Posted at: 2016-12-23T21:50:25.287Z Reads: 209

```
@Ackmaniac 

I am ashamed to say I haven't tried your app until today. Excellent work! Sent you a little token of appreciation, If I can help you in any other way please let me know. :+1:
```

---
## \#416 Posted by: Ackmaniac Posted at: 2016-12-24T00:27:49.139Z Reads: 205

```
Thank you very much for the donation. Much appreciated.
@yaca you can take the same values as in the original bldc-tool. But I don't recommend to load saved xml files of the original version. Because I haven't tested it.
It is better to save a new xml file of the new setup just to be safe.
```

---
## \#417 Posted by: Ackmaniac Posted at: 2016-12-24T00:41:29.486Z Reads: 211

```
One feature of the app I should mention is that when you switch the mode then the vesc doesn't store that mode. So if you switch the board off and on it will be back to the original mode. If you want the new mode as default mode you first have to select the mode via the app by pressing on the little mode window box. When the the vesc runs in the new mode you have to press the mode window box a bit longer and a window will appear which asks you if you want to use this mode as the default mode.

So why don't I always store the new mode as default mode. Because this is great if you want to make sure that when your kids take your board that it isn't in Ludacris mode. You only can activate it by the app. Also helpful for police if you want to pretend that your board is not more than a toy if you understand :wink:
```

---
## \#418 Posted by: SageTX Posted at: 2016-12-24T06:49:56.337Z Reads: 205

```
That's cool.  I was wondering why it felt like it reverted to slow mode.  This actually helps in several situations.  Thanks!

quick edit-- What if you disconnect the app, but not turn off the board?
```

---
## \#419 Posted by: Ackmaniac Posted at: 2016-12-24T09:45:11.357Z Reads: 200

```
One you selected a mode you don't need to stay connected. It keeps the selected mode also without the app.
```

---
## \#420 Posted by: Ackmaniac Posted at: 2016-12-24T10:09:32.093Z Reads: 209

```
Thanks to the info of chaka i fixed a bug where distance and range was calculated the wrong way when Miles were  selected as distance unit. Can take a little while until it is available in the apps store.

Merry Christmas everybody.
```

---
## \#421 Posted by: raxell Posted at: 2016-12-25T13:21:16.225Z Reads: 214

```
I was riding 1 hour in watt mode. I like it!. I love the idea of remaping the throttle my way. Works perfect with nunchuck. I have to set Deadband, sometimes still accelerating a little bit without touching the stick.

What is not working is cruise control. When I press C button motor makes weird noise and brake. Maybe I have to set some parameters. I have all parameters by default in cruise control because I don't understand what each parameter does.

Anyway, I am waiting my GT2B to ride in PPM and use a blutooth module with your app.

Amazing!!
```

---
## \#422 Posted by: Ackmaniac Posted at: 2016-12-26T20:57:56.207Z Reads: 214

```
Here is a little video of a demo test run. Not very cool but it shows a little how the VESC works. Roads were slippy so no real carving was possible. So i did alot of hill climbing and full speed runs. It is my single drive. I will try tomorow to make a video in the daylight. Then it should be of a better quality. And i think i need a selfie stick (what went wrong in my life that i need a selfie stick).
https://youtu.be/3zMGm0apBoQ
```

---
## \#423 Posted by: mmaner Posted at: 2016-12-26T22:27:39.758Z Reads: 210

```
I installed the firmware, did the basic config, put it in the road.  I still have some research to do before I do any heavy configs, still trying to understand VESC parameters and the learning this modded firmware on top of it.  It seems smooth, but it also felt smooth before.
```

---
## \#424 Posted by: Ackmaniac Posted at: 2016-12-27T00:09:18.629Z Reads: 208

```
If you need help then please also post Screenshots of your actual setup. That makes it easier. You could also send a pm message if you don't want to share it with the rest of the world.
```

---
## \#425 Posted by: mmaner Posted at: 2016-12-27T04:14:30.320Z Reads: 207

```
Be glad to, just been a busy day.  I'll do it in the morning. Thanks for being so responsive.  

I do have a question.  How difficult would it be to make the 'tiles' configurable? As in placement and size?

Also, I'll be donating when I get back to work.  PayPal has gone nuts on my phone.  I thjnkjits in Cyrillic 😁.
```

---
## \#426 Posted by: Ackmaniac Posted at: 2016-12-27T14:34:40.579Z Reads: 211

```
I think this one is a better video. At the end of the video you can see how the VESC overheats. But it regulates itself.

https://youtu.be/eaLUqa4avyA
```

---
## \#427 Posted by: TarzanHBK Posted at: 2016-12-27T14:55:39.454Z Reads: 208

```
There you have some good realtime data. It´s interesting to see the actual amps beeing drawn. People often underestimate how much our boards need when it comes to a small hill and leave their limits too low. You´re often cruising with 15 - 20A and reach 40A batt and 75A motor a few times.
So always good to think about that and build a board with hardware capable of higher amps, if you want something with 50 km/h.
Well done Ack ;)
I´ll have a few boards running your software next year!
```

---
## \#428 Posted by: Maxid Posted at: 2016-12-27T16:51:16.801Z Reads: 205

```
Just came back from my first "longer" run and want to give some constructive feedback:

The data columns in the csv seem a bit weird:
1) time column would probably be clearer when split into date and time
2) How can I start with WattHours already consumed? First row already shows data for AmpHours, AmpHours charged, WattHours and WattHours charged.
3) Why does the tachometer values not use the gear ratio and poles to give me actual speed in km/h?
4) GPS data columns have only zeros filled in - even though location data is allowed.

Some graphs would also be nice so that I don't have to transfer the csv to my PC every time.
And I am still rooting for android wear support - would be awesome to see the battery voltage on my wrist ;)
```

---
## \#429 Posted by: Ackmaniac Posted at: 2016-12-27T17:47:52.905Z Reads: 201

```
**1) time column would probably be clearer when split into date and time**
When you use the charts inside the app you don't have to worry about it. But i will give it a thought.
**2) How can I start with WattHours already consumed? First row already shows data for AmpHours, AmpHours charged, WattHours and WattHours charged.**
I think you mean to start with fresh data. In this case you have to switch the board off and on. This way the data starts from 0 again.
**3) Why does the tachometer values not use the gear ratio and poles to give me actual speed in km/h?**
Because if you change your gearing ration you will have the correct data. But i will give that also a thought. Because you might want to compare different gearing setups. So it would make more sense to save the speed.
**4) GPS data columns have only zeros filled in - even though location data is allowed.**
That is strange. Please check if you switched on your GPS and that it locates your GPS position by the GPS symbol in the smartphones status bar.
```

---
## \#430 Posted by: Maxid Posted at: 2016-12-27T18:53:26.845Z Reads: 194

```
How do I use the charts inside the app? I can only find the button to change the default folder.
```

---
## \#431 Posted by: Ackmaniac Posted at: 2016-12-27T18:54:04.361Z Reads: 196

```
Just click on a CSV file.
```

---
## \#432 Posted by: Maxid Posted at: 2016-12-27T19:22:24.905Z Reads: 207

```
I don't see any files inside the folder.<img src="/uploads/db1493/original/3X/6/7/671b16c088b9c675bf79ea913ef6038523214dfb.png" width="281" height="500">
```

---
## \#433 Posted by: Ackmaniac Posted at: 2016-12-27T19:23:36.371Z Reads: 189

```
Then please press the disk icon to set this folder as the default folder. it should be the VESCMonitor folder on your device. And did you give the app the rights to write on the disk or did you disallow it.
```

---
## \#434 Posted by: Maxid Posted at: 2016-12-27T20:13:10.195Z Reads: 205

```
but that is the folder I have set as default - and it appears to be empty even though there are csv files inside.
<img src="/uploads/db1493/original/3X/e/1/e1024f3e8953a67b8821e1ea77bade48d214df3b.png" width="281" height="500">
What am I doing wrong?
Permissions are set
<img src="/uploads/db1493/original/3X/d/3/d38e9d820b4edb403c74855ada75d956b606439b.png" width="281" height="500">
it is also weird that the OSX android file transfer app does not see the newly created files the file explorer app on my phone can see (look at the files from today 27th of december)
<img src="/uploads/db1493/original/3X/a/d/adc4391b3e8113ce0f40409bf52a601409395ed6.png" width="638" height="500">
```

---
## \#435 Posted by: Ackmaniac Posted at: 2016-12-27T20:50:19.050Z Reads: 184

```
I just reeased a new version. Please install this one and create a new csv file by logging some data and ry it again. the upload at google takes a while but i made it also available at my dropbox link. I also added the change for the speed in the CSV file so that the speed is logged instead of the rpm. And also instead of the tachoABS data the distance is now available.
```

---
## \#436 Posted by: Maxid Posted at: 2016-12-27T20:56:13.595Z Reads: 180

```
was it a bug or did I do something stupid? Will test it tomorrow. Thanks for the quick update :thumbsup:
```

---
## \#437 Posted by: Ackmaniac Posted at: 2016-12-27T20:57:16.895Z Reads: 179

```
I am not sure if you had the latest version. At my phone it works without issues. I hope it was a old version.
```

---
## \#438 Posted by: SageTX Posted at: 2016-12-27T21:51:52.910Z Reads: 211

```
I don't think the ERPM is being changed by the app.  Screenshots of the mode settings, and ss of three modes all topping at exactly 21.4 mph.  Is there something overriding it or is it not affected by the app?

I do believe the watts are being set, as it "feels" more powerful, and the watts go up on the monitor, although higher than set. Probably just a quick spike though, nothing sustained.
I would like to be able to set the ERPM so I could actually hand it to a beginner and limit top speed. 

<img src="/uploads/db1493/original/3X/2/d/2dbdb9a1561200a21da73079fac4593289ef0ed6.jpg" width="281" height="500"><img src="/uploads/db1493/original/3X/1/4/14b42e3e513ec65122278c0ae324f7d6c0d9a121.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/1/f/1fe9a6b5a647b803dcf59f5b566ff2912dc893f0.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/f/7/f7da3e9650a662906088bfb9e986a86442829afc.jpg" width="690" height="388">
```

---
## \#439 Posted by: Ackmaniac Posted at: 2016-12-27T21:56:02.617Z Reads: 187

```
I will have a look at it
```

---
## \#440 Posted by: Ackmaniac Posted at: 2016-12-27T22:16:32.498Z Reads: 190

```
I have good and bad news for you. Good thing is that the speed get's limited. You can test that by setting extreme values and test it on the bench.
So what happens.
I set a soft ERPM limit in the PPM setup. But when i read the values to display it in the APP i read the Motor Max ERPM which i don't change. So finally it is working but you see the wrong value in the app. Will change that in the future but sadly you need a new Firmware file for that.
So i hope you can live with that bug. But you can be sure that when you see that the new selected mode is activated that also the speed limit is set.
```

---
## \#441 Posted by: SageTX Posted at: 2016-12-27T22:32:37.867Z Reads: 198

```


OK, so the ERPM setting in the modes changes the soft ERPM  on the PPM tab   

I have it set on the tab as ERPM limit start 35000 and ERPM limit end 36000. {for the basic turn it on and go setup} 

Does the app change both, or should the limit end be set to 60000? (I feel like I'm soing something wrong here)
<img src="/uploads/db1493/original/3X/c/d/cd6bf712861ee9cab392e3a92f4813cabfc23e3b.png" width="690" height="387">

oh and the bug is fine, not sure where it shows in the app anyway, just so i know what i am changing.
```

---
## \#442 Posted by: Ackmaniac Posted at: 2016-12-27T22:36:28.064Z Reads: 194

```
The app changes 3 values. It sets the ERPM limit end to the selected ERPM from the app. Then it sets the ERPM limit start to 4 % less than then the value from the app. And it sets the PID max ERPM value to the same value as in the App so that the cruise control is also working at the same max speed.

So if you set for example 25000 ERPM in the app then the values will be
ERPM limit end 25000
ERPM limit start 24000
PID max ERPM 25000

The motor settings max ERPM will stay as default becasue it is already limited by the PPM settings.
```

---
## \#443 Posted by: SageTX Posted at: 2016-12-27T22:38:51.234Z Reads: 188

```
Awesome, thanks.  Now that I have the BLDC tool connected, I can see the values change.
```

---
## \#444 Posted by: Ackmaniac Posted at: 2016-12-27T22:43:14.504Z Reads: 186

```
And you also should install the latest version of the app. I can see that not all the values are correct which are already fixed. And do me a favor and publish a video of your ride. Would love to see the values of some other boards for comparison.
```

---
## \#445 Posted by: SageTX Posted at: 2016-12-27T23:46:27.369Z Reads: 203

```
App updated.

These are original videos those screenshots came from.  If you want a longer ride I can do that, but they are jumpy, as my ride safety takes priority in my brain over videoing.  :head_bandage::-1:

Longest video - Beginner Plus Settings
https://youtu.be/TZT6F-VPvH8

Advanced Settings
https://youtu.be/rEBhqeEML_g

and Fastest Settings
https://youtu.be/M8pQazLWt9Y
```

---
## \#446 Posted by: Ackmaniac Posted at: 2016-12-28T00:07:32.836Z Reads: 185

```
Awesome, thx for the videos. So you really should get the latest version of the app because the max and min battery values are fixed and the distance and range when miles are active is calculated the right way.

Oh and you asked the question why the max watts are exceeded. that is because you have  VESCs. So it summarized the values. Means when you have 2 VESCs the values which make sense are doubled then like watts, motor amps, battery amps Wh and Ah.
```

---
## \#447 Posted by: SageTX Posted at: 2016-12-28T00:20:05.312Z Reads: 185

```
I updated.

Oh, so If I set max watts to lets say 1000,  The monitor would show up to 2000 because Double the VESCs, Double the power.

I haven't even come close to hitting max power!!!
```

---
## \#448 Posted by: Ackmaniac Posted at: 2016-12-28T01:20:37.169Z Reads: 191

```
Seems that you don't give full power. And your gearing is quite short. Because at 21 miles you reach max speed already.
So you also see that you only need like 450 watts for 21 mi/h (34 km/h). Most people think they draw full amps.
```

---
## \#449 Posted by: Ackmaniac Posted at: 2016-12-28T01:24:38.313Z Reads: 195

```
I also added a new feature which shows the average speed. You can see it in the speed box.

**Ø T = Average Total** 
Average speed over the entire time, also when the board doesn't move (starts counting once 1 km/h is reached)
**Ø R = Average Riding**
Average speed over the entire ride time. Only measures the speed when the board is moving. So if you make a short stop it doesn't count it.

As always google play store needs a little time for it, if you can't wait you can find it in my dropbox link.
```

---
## \#450 Posted by: Ackmaniac Posted at: 2016-12-29T14:56:16.501Z Reads: 203

```
Added the GPS speed as additional info to the speed box. This is to verify the speed. It only updates the values when GPS is activated in the apps setting.

<img src="/uploads/db1493/original/3X/1/4/14d21c8a4b3279d7efa440f1a2416b9bae062da1.jpg" width="280" height="500"><img src="/uploads/db1493/original/3X/2/c/2c71b2bda581c9fc1fed7f5fbeee41068cbdc231.png" width="319" height="500">
```

---
## \#451 Posted by: Pimousse Posted at: 2016-12-29T15:49:42.530Z Reads: 192

```
Nice feature !
I was waiting for so long for update of the app through Play Store but I didn't know that the app changed :smile:
So I downloaded the new one and gone for a ride.
I noticed a bug with mode switching.
I set a beginner mode limiting amps and ERPM. When I switch to it, power is limited, top speed too.
Perfect.
But when I switch back to "default", I recover the initial power but I'm still limited by the beginner ERPM limit.
The only way to fully recover default settings is to reboot the VESC.
Any idea why it acts like this ?

EDIT : for recording video I have to hold my phone upside/down...
Not so easy for the mind to reverse while riding. :smile:
```

---
## \#452 Posted by: Ackmaniac Posted at: 2016-12-29T16:09:30.507Z Reads: 189

```
Thank you very much for that info. I checked it and found already the bug. But i only can fix it by a new firmware update which will take a while.

But you can avoid it by creating a mode which represents the default mode. And before switching to default you can select that mode. Problem is that i don't initialise the values again. I only initialised the motor max ERPM but then switched to the PPM limitation. But i forgot to also initialise the ppm values again.
```

---
## \#453 Posted by: Ackmaniac Posted at: 2016-12-29T18:23:28.416Z Reads: 188

```
I was working again on my app and found some bugs which i fixed. For example the distance was not 100% correct.
I recommend for everybody to get the latest version of the app. The current Version is 29.
Also the range and battery % value will only be calculated when there is no power to calculate the correct value. This way you get a relatively precise reading.
And it would be awesome if some of you can post videos which are made with the app to compare different boards.

As always google needs a while for the update, if you can't wait you can find the file at my Dropbox link.
I think the app needs to be updated manually because it is in beta status at the Google Play store.
```

---
## \#454 Posted by: Pimousse Posted at: 2016-12-29T18:24:44.565Z Reads: 174

```
Nice !
Do Play Store need to validate even if it's in beta ?
```

---
## \#455 Posted by: Ackmaniac Posted at: 2016-12-29T18:27:06.106Z Reads: 176

```
I think it's because they have multiple servers and millions of apps. So they need to synchronize it between all the other servers, check if there are no viruses or hurt policys and then they can publish it. Normally it takes between 3 till 12 hours.
```

---
## \#456 Posted by: Pimousse Posted at: 2016-12-29T18:38:04.023Z Reads: 186

```
I just updated mine.
Could you add a "About" menu to check the version (and add credits to you with Paypal donation link or something ;) ).
I didn't donate yet, I correct that mistake immediately ! :slight_smile:
```

---
## \#457 Posted by: Maxid Posted at: 2016-12-29T18:42:49.585Z Reads: 183

```
Will try to record one as soon as the weather allows it.
```

---
## \#458 Posted by: Pimousse Posted at: 2016-12-29T18:53:09.618Z Reads: 197

```
Mine (short) :
https://www.youtube.com/watch?v=R8FO4BkfFZ4

Note for myself : put the flight mode during recording :smile:
```

---
## \#459 Posted by: Ackmaniac Posted at: 2016-12-29T19:05:00.228Z Reads: 191

```
Thank you very much for the video. 

I can see that you don't have the latest version with GPS speed and correct distance and range calculation.

I think google is 4 updates behind. Please try it tomorrow again or download it from my Dropbox link and install it manually. Made a couple of updates today for every little bug, feature or improvement i found or made.
```

---
## \#460 Posted by: gaetjen Posted at: 2016-12-29T19:18:59.679Z Reads: 187

```
Hey, just connected the bluetooth modul and it connects to the app, but the default settings stay at 0. When I hit the throttle the motor spins normally, but nothing happens in the app. I created other profiles like beginner and pro, but I can't select them. It stays in default. The modul  is connected rx on vesc to TX on modul an the other way around. Any ideas?
```

---
## \#461 Posted by: Ackmaniac Posted at: 2016-12-29T19:20:45.839Z Reads: 195

```
please post a screenshot of your applications General tab and the UART Tab.
```

---
## \#462 Posted by: Pimousse Posted at: 2016-12-29T19:52:13.159Z Reads: 200

```
I updated after the video, now I can see GPS speed.
```

---
## \#463 Posted by: Ackmaniac Posted at: 2016-12-29T20:35:11.966Z Reads: 221

```
This picture here shows a good basic setup for a Li-Ion battery (**not** LiPo). Of yourse your cells can differ a bit but i think it is a good starting point. These values are used for batterys voltage when there is no load on the cells. Because of that you will see that the battery percent changes only when the board is in idle (no acceleration and no braking).
For the VESC itself in BLDC-Tool you can set the cutoff start to 3.0 and cutoff end to 2.8 for each cell. So for a 8S you have to multiply these values by 8. If you want to treat your cells a bit nicer you can set the values to 3.2 for cutoff start and 3.0 for cutoff end. For LiPo batterys it is another story. There i would set the values to 3.6V for cutoff start and 3.4 for cutoff end.
But as already mentioned, this is only a recommendation. Each battery behaves a bit different.
<img src="/uploads/db1493/original/3X/2/8/28ba7f8f27357f29b55e4321e3875596c35fdc2c.png" width="281" height="500">
```

---
## \#464 Posted by: Ackmaniac Posted at: 2016-12-29T20:50:51.953Z Reads: 219

```
And i found a picture where they explain the no load voltage in relation to the capacity for a LiPo battery. 
So it is not very different to a Li-Ion battery for no load. But the voltage cutoffs are different under load situations. So please read the post above.
<img src="/uploads/db1493/original/3X/6/0/60d3e3102f6a56bc33ad21709afa7caa98237cad.jpg" width="666" height="500">
```

---
## \#465 Posted by: gaetjen Posted at: 2016-12-29T21:09:10.965Z Reads: 203

```
When I did the screenshot I realised that I hadn't changed the ppm settings to ppm+uart. I corrected that and now it works like a charm. Will be doing some testing tomorrow and then some donations :-)
```

---
## \#466 Posted by: Esrapp21 Posted at: 2016-12-29T21:10:58.030Z Reads: 197

```
Hey, cool app! Do you ever see releasing it for iOS in the future?
```

---
## \#467 Posted by: Ackmaniac Posted at: 2016-12-29T21:17:33.505Z Reads: 203

```
I never programmed a IPhone app and I don't even have a Mac or IPhone. Maybe I will start in the future but @evoheyax also has a app for IPhones.
```

---
## \#468 Posted by: PXSS Posted at: 2016-12-30T05:35:57.481Z Reads: 203

```
Why not go by an actual discharge curve?
You can find them at Lygte.info. I would use Samsung 25r as a base since that's what most use
```

---
## \#469 Posted by: Maxid Posted at: 2016-12-30T10:52:31.985Z Reads: 203

```
I went for a short ride - couldn't hold my phone in hand (too cold) to make a video.
However the csv files are still not listed in the app - the file explorer shows them though.
Used the new version with GPS speed settings.
Not sure why it is only me having this problem. I am on a Nexus 5 with custom rom Pure Nexus 6.0.1
```

---
## \#470 Posted by: gaetjen Posted at: 2016-12-30T12:03:30.926Z Reads: 199

```
Do I need a nunchuck reciever to use PID speed control no acceleration or does it work with a winning remote as well?
```

---
## \#471 Posted by: Ackmaniac Posted at: 2016-12-30T12:08:45.562Z Reads: 204

```
At the moment it only works with a ppm remote. So the Nunchuck will not work. If you want cruise control then this would be the wrong mode. But if you want a mode that doesn't accelerate and only keeps the current speed then this is the way to go. It feels like a mix of normal skateboarding and e-skateboarding because you have to push to your speed and then it can keep it. Mainly i did that to try to create a legal mode for Germany.
@Maxid I am working on a update which hopefully fixes the problem you have. But i can't promisse. Will inform you in the next hours.
```

---
## \#472 Posted by: Maxid Posted at: 2016-12-30T14:19:59.197Z Reads: 214

```
The android file transfer app was again also not able to "see" the files inside the folder.
I cleared the database (Settings->Apps->Show System Processes->Media Storage->Clear Data) following this post
http://android.stackexchange.com/questions/46315/not-all-files-are-visible-over-mtp
It helped - I can now transfer the files to my Mac.
However your App does still not list any of the csv files.
I hope you can solve this :thumbsup:

Plus I have another recommendation:
Instead of date as a column in the csv could you add a elapsed time in seconds column? That way one could easily plot the charts with time on the x-axis instead of doing calculations to extract this information from the timestamp.
Also one question: I set the number of VESCs in the settings to two. Are the values doubled now or does the csv still show just one VESC?
```

---
## \#473 Posted by: Ackmaniac Posted at: 2016-12-30T14:22:13.397Z Reads: 206

```
It doubles the amp and watt values automatically.
```

---
## \#474 Posted by: Maxid Posted at: 2016-12-30T14:27:43.916Z Reads: 205

```
So is battery current also doubled? You should probably give some indication in the csv file which columns are actually doubled.
```

---
## \#475 Posted by: Ackmaniac Posted at: 2016-12-30T14:39:10.755Z Reads: 209

```
All the marked marked values are multiplied by the amount of VESCs (Motors). So if you have 4 Wheel drive then the values would be multiplied by 4. This way you are able to see the real currents and watt that count for the battery.

<img src="/uploads/db1493/original/3X/a/f/afe45af8634c6f189d50f6910475d630497b13a9.png" width="281" height="500">
```

---
## \#476 Posted by: Maxid Posted at: 2016-12-30T16:34:24.792Z Reads: 192

```
I just did a test on my bench with no load. When I use the cruise control button on the nunchuck the battery current and motor current become negative values even though I am not braking but still basically use full throttle. Seems odd, no?
<img src="/uploads/db1493/original/3X/4/7/4745f184db264204fbdd3687c8bc9bd43a865235.png" width="690" height="410">
```

---
## \#477 Posted by: Ackmaniac Posted at: 2016-12-30T17:07:04.689Z Reads: 181

```
Can you please check the CSV files if the value is wrong there. Because i have no answer for that. Maybe something went wrong in your graph calculation. Will show you a video of my cruise control in a couple of minutes. there you can see that it is working.
```

---
## \#478 Posted by: Maxid Posted at: 2016-12-30T17:09:52.650Z Reads: 182

```
I noticed the negative values in the app while "riding" the board on the bench not just afterwards in the csv. The charts I just posted to show you what was going on. Maybe it has to do with FOC and no load? Just wanted to let you know.
And cruise control does also work in my case - under load and no load.
```

---
## \#479 Posted by: Ackmaniac Posted at: 2016-12-30T17:14:45.264Z Reads: 181

```
Do you use my firmware. Because the standard firmware also brakes in cruise control. In my firmware you can disable the braking in cruise control in the advanced tab.
```

---
## \#480 Posted by: Maxid Posted at: 2016-12-30T17:17:59.374Z Reads: 188

```
Of course I am using your firmware and BLDC Tool.
Not sure what you mean with braking on the standard firmware. I have never experienced this on the standard one. The Nunchuck cruise control is supposed to hold your speed when pressing the C-Button and allows adjusting the speed via the trigger.
It behaves the same way in your firmware.
```

---
## \#481 Posted by: Ackmaniac Posted at: 2016-12-30T17:23:06.070Z Reads: 201

```
I mean this checkbox in my firmware. When you carve havily in cruise control then you feel that the VESC brakes because it always trys to keep the speed. Because of that i added the feature to disable braking in cruise control. Because it is very disturbing during carving. if you want to disable braking in cruise control it it should **not** be checked like in the picture.

<img src="/uploads/db1493/original/3X/7/9/798226f15897eadefee957530728192af8e26199.png" width="690" height="419">
```

---
## \#482 Posted by: Ackmaniac Posted at: 2016-12-30T17:26:31.518Z Reads: 199

```
**New Android App Update**

I have changed a couple of things in the app. As you can see in the video it shows now green and red bars for power, motor current, battery current and duty cycle. When one of those bars reached the end then it means that this is the actual limiting factor for the power output. For example when maximum motor amps are reached you will see that immediately by the bars. Watch the video then you will understand what i mean.

You can also see that i rearranged the boxes because i wanted to have all the limiting factors below each other to easily see which one is limiting right now.

And i also show in the video how the nicely the cruise control works with a PPM remote.
https://youtu.be/2fd8sIHi9sM

I also changed the code for the file explorer so @maxis please check if you can see the CSV files now. First please store the default folder again by pressing the disc icon.

As always google needs half a day for to publish the new Version in the Play store. If you can't wait you can find the apk file in my Dropbox link in the first post of this thread.
```

---
## \#483 Posted by: Maxid Posted at: 2016-12-30T17:28:03.083Z Reads: 194

```
But I am not using PWM mode.
```

---
## \#484 Posted by: Ackmaniac Posted at: 2016-12-30T17:31:13.726Z Reads: 190

```
This is not for PWM. The Speed control works for FOC and BLDC mode.
```

---
## \#485 Posted by: Maxid Posted at: 2016-12-30T17:35:51.830Z Reads: 195

```
oh - I always thought the entire page is only used in BLDC mode. Guess that applies only to the first groupbox then - Sorry...
```

---
## \#486 Posted by: Ackmaniac Posted at: 2016-12-31T00:59:02.192Z Reads: 195

```
**New Android App Update**
I changed the request frequency a bit so that the values are more close to the actual situation. The app is now like 0.2 seconds delayed to what happens in reality. You can hardly even tell that there is a delay now.

As always google needs half a day for to publish the new Version in the Play store. If you can't wait you can find the apk file in my Dropbox link in the first post of this thread.
```

---
## \#487 Posted by: Maxid Posted at: 2016-12-31T08:49:05.026Z Reads: 193

```
Everytime I install the apk or get an update in the play store the version number is 1.0
It is really hard to keep track of the new versions. Would you mind setting the numbers correctly? Will test it today again...
```

---
## \#488 Posted by: gaetjen Posted at: 2016-12-31T09:11:13.869Z Reads: 182

```
I want to use the no acceleration mode the same way as you. So that it is maybe half legal in Germany. I tried the mode, but I have too much motor stuttering. I have a dual vesc setup. I just changed the ppm setting to PID no acceleration and kept all the others values the same. Is there anything else I have to change?
```

---
## \#489 Posted by: Ackmaniac Posted at: 2016-12-31T09:41:57.703Z Reads: 187

```
Please post a Screenshot of the Motor Advanced Tab.  And you have to test it while you are riding on it. Because on the bench it is hard spin both wheels at the same time with a decent speed for the cruise control. And when you are very slow on the bench it feels like stutter.
```

---
## \#490 Posted by: gaetjen Posted at: 2016-12-31T10:33:15.840Z Reads: 193

```
<img src="/uploads/db1493/original/3X/7/3/738b392fdba7f7b545908dd96141b03f5c560bdd.png" width="690" height="387">
```

---
## \#491 Posted by: Ackmaniac Posted at: 2016-12-31T11:49:20.763Z Reads: 197

```
You should disable braking for cruise control.And then try on the street and not on the bench.

<img src="/uploads/db1493/original/3X/7/9/798226f15897eadefee957530728192af8e26199.png" width="690" height="419">
```

---
## \#492 Posted by: raxell Posted at: 2017-01-01T13:10:01.668Z Reads: 190

```
I have solved my issue with nunchuck cruise control changing KP and KI "Speed control" parameters. I have used the default firmware 2.18 settings.

KP:0.00010 instead of 0.00400 and KI:0.01500 instead of 0.00400
```

---
## \#493 Posted by: Eboosted Posted at: 2017-01-01T19:05:18.490Z Reads: 188

```
@Ackmaniac

Does your firmware needs to be uploaded when switching from FOC to BLDC in order to avoid blowing the DRV chip?
```

---
## \#494 Posted by: Ackmaniac Posted at: 2017-01-01T19:11:54.664Z Reads: 192

```
You should reboot the VESC after switching from one to the other. Flashing the firmware again doesn't make any sense to me. But when you do the motor detection you should disable the remote application first. Then do the motor detection. And then enable the remote application again. I think that a lot of errors in Foc resulted from that mistake. Because if you don't disable it,  then the remote signal would interfere the motor detection.
```

---
## \#495 Posted by: Eboosted Posted at: 2017-01-01T22:43:36.833Z Reads: 187

```
What do you mean by disabling the remote application?
```

---
## \#496 Posted by: Ackmaniac Posted at: 2017-01-01T22:54:15.922Z Reads: 189

```
You can configure the motor and the remote. And the remote setup is called application in the bldc-tool. For example in the ppm setup set the ppm control mode to disabled,  write the configuration and then do the motor detection. Afterwards enable it again.
```

---
## \#497 Posted by: SageTX Posted at: 2017-01-02T01:34:05.028Z Reads: 183

```
Since newest update, can't get App to connect to BT.  Shows module on the "scanning" page, but wont fully connect after pressing correct one.  

Anyone else?
```

---
## \#498 Posted by: Ackmaniac Posted at: 2017-01-02T08:08:55.525Z Reads: 185

```
Just switch off the board,  wait a couple of seconds and switch it back on. And also kill the app in the background and restart it. Sometimes the modules have a problem. If this doesn't help then let me know and I will revert the latest changes that make the communication a bit faster.
```

---
## \#499 Posted by: Pimousse Posted at: 2017-01-02T11:49:26.653Z Reads: 189

```
I just had a ride, it works for me.

Some inputs to improve the app :
For each build, could you create variables memorized for odometer and average energy consumption (Ah/km or Wh/km for comparision with any build) ?

I didn't try the bars feature because I'm not confident to hold my phone while riding :smile:
```

---
## \#500 Posted by: Ackmaniac Posted at: 2017-01-02T19:20:40.482Z Reads: 197

```
@SageTx I made a little change to the app which hopefully fixes your connection problems. If you see the the text disconnect at the top right on the screen after you selected the Bluetooth module then it should be fine. If you see "connect" text then please click on it so that it tries to reconnect. Please let me know after the update of it works now.

@Pimousse You can also record a video of the app while you are riding. This way you can analyse it later. And you don't have to hold it in your hand. Even if you don't record your ride the realtime data in the video is still helpful. Otherwise you can also have a look at the graphs. They are always recorded even without the video. Just go to the file explorer inside the app (click the galarie icon) and select the last CSV file to see the last recorded data. 
I also could add the feature to save and summarize the average values of each ride but it would be necessary to connect to the Bluetooth module via app after each ride to save the data. Sadly the Bluetooth modules have no memory on their own. I had it once with a ESP8266 and WIFI which could sava data on their own but the cheap HM-10 can't store any data.
But i think about a nice solution. 

As always google needs half a day for to publish the new Version in the Play store. If you can't wait you can find the apk file in my Dropbox link in the first post of this thread.
```

---
## \#501 Posted by: Maxid Posted at: 2017-01-02T21:39:03.860Z Reads: 188

```
I appreciate the v1.1 identification ;)
Play store has already let me download the new version.
```

---
## \#502 Posted by: Pimousse Posted at: 2017-01-02T22:22:20.009Z Reads: 191

```
I think it's mostly for the odometer that connecting to the board each time is required.
For average comsuption I was mainly thinking to "average the average". So if you forget/don't want to connect the app, you just loose an average in your calculation but it doesn't really matter, right ?

I often think about adding the arduino nano I planned to use at the beginning (before discoring the power of bluetooth and app) as a gateway between HM10 and VESC to perform some other feature (memorize variables, LCD, leds and lights managament...).
Is it something you already worked on ?
```

---
## \#503 Posted by: DeathCookies Posted at: 2017-01-02T23:26:47.804Z Reads: 197

```
HM10 Module
Watt Controll Firmware 2.52
PPM + Uart
9600 Baudrate

HM10 to VESC
RX to TX
TX to RX
VCC to 5V
GND to GND

The chip is blinking but the app wont find it... Does anybody have an idea what i could have done wrong?
```

---
## \#504 Posted by: Ackmaniac Posted at: 2017-01-02T23:57:28.814Z Reads: 195

```
Is Bluetooth enabled on your device? I never had a issue to see the Bluetooth modules. Can you please make a picture of the module. Could it be that you purchased them from evoheyax or is it a standard HM-10 module?
```

---
## \#505 Posted by: Maxid Posted at: 2017-01-03T00:06:46.404Z Reads: 189

```
is it the breakout board version or only the true HM-10 PCB?
The HM10 needs 3.3V and not 5V
```

---
## \#506 Posted by: SageTX Posted at: 2017-01-03T05:46:20.063Z Reads: 198

```
I'm not sure what happened, the update didn't help, but I completely uninstalled the app-  deleted the VESC folder, reset my phone, reinstalled the app and now connects fine. 

Thanks for looking into it though, not sure what the problem was, maybe just my phone, or something funky in the installation.
```

---
## \#507 Posted by: DeathCookies Posted at: 2017-01-03T09:19:23.677Z Reads: 211

```
[quote="Ackmaniac, post:504, topic:12286"]
Is Bluetooth enabled on your device?
[/quote]

yes ;)

I just bought this HM10 module some time ago. Even if i change from 5V to 3.3V it does not work...
<img src="/uploads/db1493/original/3X/c/2/c25e914739792ec14a03585df0edc56df7155433.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/6/8/687c3069c07cf06bfa9df5d67b3fa57282290abc.jpg" width="666" height="500">
```

---
## \#508 Posted by: Maxid Posted at: 2017-01-03T09:20:50.634Z Reads: 190

```
that looks different to mine - you sure it is a HM10?

Edit: looks like a HC05
http://www.martyncurrey.com/bluetooth-modules/

that is the wrong module!
```

---
## \#509 Posted by: DeathCookies Posted at: 2017-01-03T09:28:01.188Z Reads: 190

```
Well you are right :D it seems as i have soldered my HC05 instead of HM10 :frowning:

I will change the module and report back. Sorry for the dumbness and thanks for the help :D
```

---
## \#510 Posted by: Ackmaniac Posted at: 2017-01-03T09:37:25.405Z Reads: 191

```
It's very easy to get them mixed up because they all look very similar. But pictures or Screenshots help in most cases. So if somebody has issues and a picture might help then please take the time and add them to your post.
```

---
## \#511 Posted by: DeathCookies Posted at: 2017-01-03T09:50:24.150Z Reads: 188

```
Now it is working with the right Module :smiley:
Thanks @Maxid and especially to @Ackmaniac
```

---
## \#512 Posted by: Pimousse Posted at: 2017-01-03T14:12:21.803Z Reads: 191

```
@Ackmaniac, would it be possible to add persistent notifications on lock screen when the app is connected and recording ? With some important values as well :slight_smile: 
And, is it possible to add a button to toggle csv recording or not (in the case you just want to check some values likes bat. voltage without creating a new csv file) ? 

Let me know if you need someone to test it ! :wink:
```

---
## \#513 Posted by: Ackmaniac Posted at: 2017-01-03T14:58:58.790Z Reads: 188

```
The lock screen would be very difficult. At the moment the screen will always stay on when the app is active. You onl can switch off the screen manually.
A button to activate the CSV logging whenever you want would be possible. But it also would be a pity of you want to analyse your ride and forgot to press the button. I think a option to be asked or that it will always be active wold be nice.
```

---
## \#514 Posted by: DeathCookies Posted at: 2017-01-04T11:14:25.340Z Reads: 183

```
I would love to See the Feature to connect a gopro for Video recording because i do not want to record the video with a Smartphone camera... 
I May have overseen it: is it possible to See when which error occured?
```

---
## \#515 Posted by: Ackmaniac Posted at: 2017-01-04T11:22:36.863Z Reads: 188

```
Yes you can see when errors occurred. It shows them at the bottom of the screen below the stats. As long as there is no error you won't see anything.
```

---
## \#516 Posted by: leroy Posted at: 2017-01-05T19:44:54.507Z Reads: 184

```
Wow, what a long thread, 
where is the code repo please? 
I would love to take a look.
```

---
## \#517 Posted by: leroy Posted at: 2017-01-05T20:04:09.867Z Reads: 183

```
I hope that doesn't come across badly, 
it sounds like you've done a great job.
I write code myself, and I am just interested.
```

---
## \#518 Posted by: SageTX Posted at: 2017-01-06T20:58:53.470Z Reads: 189

```
[quote="SageTX, post:506, topic:12286"]
I'm not sure what happened, the update didn't help, but I completely uninstalled the app-  deleted the VESC folder, reset my phone, reinstalled the app and now connects fine.
[/quote]

I found out my problem with the Bluetooth connection. It was my Tile (lost keys) app taking over the Bluetooth connection. Just thought I'd follow up if anyone else was having problems connecting.

tl:dr check your background apps.
```

---
## \#519 Posted by: Ackmaniac Posted at: 2017-01-06T21:22:58.447Z Reads: 188

```
Thank you very much for the info.
```

---
## \#520 Posted by: Ackmaniac Posted at: 2017-01-10T00:23:11.932Z Reads: 188

```
Is anybody interested in changing the throttle curve via the app? I can imagine the situation that you want a throttle curve that reduces the power at the low throttle positions when the total power output is high.
But if you change then to a setup with a low total power output then you do't want the power reduced in the low throttle positions.
I am implementing a total visual overview of all the parameters which might reduce the power output. This way it should be easy for everybody to understand why the VESC is reducing the power in some situations. You also could see if you even touch the limits so that you might can adjust the settings for more control.
```

---
## \#521 Posted by: SageTX Posted at: 2017-01-10T00:26:51.834Z Reads: 183

```
YES.  Mostly because I would like to refine my throttle curve - WITHOUT dismantling my board each configuration to do so.  Probably matching curves with modes would be helpful too.
```

---
## \#528 Posted by: Ackmaniac Posted at: 2017-01-10T07:08:18.963Z Reads: 175

```
Please try the 200 amps first before you continue to  advertise your motor here.
```

---
## \#534 Posted by: Maxid Posted at: 2017-01-10T07:48:26.715Z Reads: 182

```
Guys please stay on-topic. Feature requests should be fine IMO but the Amp discussion should move somewhere else.
Otherwise I am flagging the shit out of this.
```

---
## \#535 Posted by: Hummie Posted at: 2017-01-10T07:49:45.412Z Reads: 181

```
 @Ackmaniac said I should try 200 amps and I'm asking why not.  seems fair.  There's no one else around who seems to have a clue.  and I never advertised in this thread.  Just wondering what wattage his program will do at low duty cycle slow speeds
```

---
## \#537 Posted by: Maxid Posted at: 2017-01-10T08:00:14.134Z Reads: 183

```
was also me - not a moderator or "staff"
```

---
## \#539 Posted by: Ackmaniac Posted at: 2017-01-10T08:06:46.424Z Reads: 184

```
Keep it in this thread and in hummies. No need to high-jack others. And try 200 amps first.
http://www.electric-skateboard.builders/t/programmer-w-understanding-of-vesc-pc-side-software-language/15832
```

---
## \#541 Posted by: Ackmaniac Posted at: 2017-01-10T08:09:12.124Z Reads: 183

```
And i replied in your thread already yesterday. Can some of the admins delete all of that unnecessary conversation.
```

---
## \#544 Posted by: Smithster Posted at: 2017-01-10T08:49:42.789Z Reads: 184

```
Possible conflict of interest?
Everyone reads the flagged posts anyway :)
```

---
## \#545 Posted by: Ackmaniac Posted at: 2017-01-12T13:41:53.840Z Reads: 189

```
Just to give a little update. 
I am working currently on new Features which will be available soon.

* Full Nunchuk support
So you can conect the Bluetooth module to the slave VESC when you have a dual drive and still change ride modes and the settings.

* Power output limit visualisation
That should mean if the VESCs output power is limited by the low voltage or the VESCs Temperatur you will be able to see it in the app and in the Videos.

And i fix the bug with the speed limit in the firmware. So also a new Firmware file will be necessary.
```

---
## \#546 Posted by: Ackmaniac Posted at: 2017-01-12T22:59:27.738Z Reads: 181

```
And another new feature will be to adjust the throttle curve via the app. So each mode can have its own throttle curve or it simply uses the default one.
```

---
## \#547 Posted by: Pimousse Posted at: 2017-01-13T05:04:15.009Z Reads: 177

```
Really great job ! Many thanks.
The feature of odometer and memorisef average didn't convinced you ?
```

---
## \#548 Posted by: Ackmaniac Posted at: 2017-01-13T07:39:46.455Z Reads: 181

```
The problem with that are the bench tests. Because they would ruin the average values. And it's not so easy to identify a bench test. Especially if somebody starts with a bench test and then takes the board for a ride. If I implement something like that then I want that the numbers are correct. But I did not find a way yet to achieve that. Maybe you have ideas. 

I already delete the CSV files when the motor doesn't spin so that a simple voltage and temperature check can be done.
```

---
## \#549 Posted by: Maxid Posted at: 2017-01-13T07:43:03.866Z Reads: 180

```
can't you just use like a amp/speed ratio or acceleration threshold to detect a bench test?
On a bench you will reach top speed very quickly and the drawn amps will be low since there is almost no load.
Or time - only keep csv files when the run takes longer than a couple of minutes. Benchtests usually don't last that long.

maybe we can ask VW for some help with this ;)
```

---
## \#550 Posted by: Ackmaniac Posted at: 2017-01-13T07:48:55.814Z Reads: 183

```
[quote="Maxid, post:549, topic:12286"]
maybe we can ask VW for some help with this :wink:
[/quote]

Awesome :joy: ,  they have a factory 20km away from my hometown. If they can't help who can?
```

---
## \#551 Posted by: Pimousse Posted at: 2017-01-13T08:29:44.671Z Reads: 183

```
In order to separate bench test (or just checking voltage and so on), you should add a mode like in sport app (endomundo, runtastic...).
I see the app like this :
You open the app, connect to your board by taping its name.
The scrren with all the values appears and is in standby mode (no csv recording, monitoring only).
Then if you go for a ride that will be taken into account in the average and odometer calculation, you just tap the triangle (like "Play"button) and the app starts to log datas.
You can pause then stop your ride (like in Endumundo). That will save distance and average in the memorized variable.
Otherwise, your could also cancel your ride, it won't save anything.

For test bench, another button for that could be great to avoid corrupt the memorized values.

What do you think about that ?
```

---
## \#552 Posted by: Ackmaniac Posted at: 2017-01-14T01:03:25.213Z Reads: 176

```
Best would be to identify it automatically instead of switching buttons on off.
```

---
## \#553 Posted by: mmaner Posted at: 2017-01-14T02:07:15.638Z Reads: 175

```
@Ackmaniac Ive got the FOC itch, is it OK to use your firmware to run FOC mode?
```

---
## \#554 Posted by: Ackmaniac Posted at: 2017-01-14T02:12:46.672Z Reads: 173

```
Sure, the FOC is the same as in Vedders Firmware.
```

---
## \#555 Posted by: mmaner Posted at: 2017-01-14T02:17:36.280Z Reads: 175

```
cool, thank you sir
```

---
## \#556 Posted by: Ackmaniac Posted at: 2017-01-14T02:20:13.756Z Reads: 178

```
Why does everybody call me "Sir". Is that the new "Dude" or does everybody think that i am that old.
```

---
## \#557 Posted by: mmaner Posted at: 2017-01-14T03:26:07.383Z Reads: 184

```
[quote="Ackmaniac, post:556, topic:12286"]
does everybody think that i am that old.
[/quote]

I am old, and nobody calls me sir.  I guess Im just being polite, which is rare, so count your blessings :wink:
```

---
## \#558 Posted by: Okami Posted at: 2017-01-15T16:15:56.362Z Reads: 186

```
Hi there! Been reading this topic and I wonder - where is the rest (more of) the vesc log videos?

I understand it is not always conveniant to upload recorded videos, but would be great if it was possible to share just the stats/logs even without video.

Is this something you can do @Ackmaniac ?
Perhaps it is already possible but could you share it once again then how ppl can upload their csv files to be opened later in another software? 

Im aware it might be possible to do this (open csv) in bldc tool but can someone walk me through it?

Of course I will also need someone who can share his setup and his files. Sorry for not being a vesc user yet ha.

Perhaps you @DeathCookies could share some of your logs to be viewed? 

If you do mind and dont want to share something (which perhaps might seem personal) I will understand.
```

---
## \#559 Posted by: DeathCookies Posted at: 2017-01-15T16:46:30.033Z Reads: 189

```
Yeah, i can share some logs. Just ask me again when there is a possibility to analyze it external
```

---
## \#560 Posted by: Okami Posted at: 2017-01-15T17:10:03.644Z Reads: 195

```
@DeathCookies Oh ok, seeing @Maxid posts I somehow thought it is possible to access @Ackmaniac vesc monitor app's data outside of app/video, too. 

Ok so I know there is 3 different vesc monitor apps available. 

Evoheyax's one which is available for iphone.

Then there is metr.at app, which might be called somewhat commercial by now.

And in this topic - Ackmaniac's one.

---

I also know that metr.at app lost some credibility due to some incentives to perhaps sniff out info but I will leave this out here.

---

So far I know that evoheyax was mentioning the possibility to upload data over wifi or such and metr.at already offers to view data (without video) on the website.

So if you Ackmaniac could offer a simar feature - **to view data without the video**, that would be great!

I know you / he is probably working a lot also on other projects  but it would be something nice to have without buying the special BT module to access metr.at

---

I still got some reading to do, so sorry If I have taken something by mistake
```

---
## \#561 Posted by: Ackmaniac Posted at: 2017-01-15T17:35:04.047Z Reads: 177

```
If anybody wants to program the webpage to upload the data then i would be happy to work with you. Otherwise this has to wait until i can find the time. But anyway, i think the videos are more helpful because you have the sound and see what is happening.
```

---
## \#562 Posted by: DeathCookies Posted at: 2017-01-15T17:44:37.860Z Reads: 180

```
The data is exported to a CSV file. I could send it to you but do you have an idea how you want to analyze it? Some sample data:

<img src="/uploads/db1493/original/3X/3/1/3152af1ff4debf6fef80e61a3ab5f0818ff55e80.png" width="690" height="301">
```

---
## \#563 Posted by: Okami Posted at: 2017-01-15T17:46:44.107Z Reads: 177

```
I just see now that video upload (due to size sometimes) might be an obstacle for ppl to share them.
```

---
## \#564 Posted by: DeathCookies Posted at: 2017-01-15T17:49:41.798Z Reads: 183

```
This is only an extract of an log file. I did not activate GPS therefore the last 4 columns do not have any valid numbers.


----------
Just about privacy: You can locate the exact position with such a log file....
```

---
## \#565 Posted by: gaetjen Posted at: 2017-01-15T18:30:34.999Z Reads: 186

```
https://www.youtube.com/watch?v=NM4X05jWT74&feature=youtu.be

@Ackmaniac Here is another video of your very nice app. I have a 10s3p setup with dual 190kv motors and 83mm wheels and a 16/36 ratio. I set 3 modes:Beginner, Medium and Ludacris and I just love the easyness of changing modes and adjusting the riding experience. In my Ludacris setup I have 1700 Watt max, 70a motor max, 50a battery max, -40 motor min, -6a batt min. 
After I drove some minutes the max power showed 2954 Watt. Should I set my max Watt in my Ludacris mode to that to get the most power out of my setup?
```

---
## \#566 Posted by: Pimousse Posted at: 2017-01-15T18:46:02.599Z Reads: 182

```
That is a point I talked about with a friend who is web designer. But the dev of VESC monitor (Solarturtle) wasn't so active to improve/debug its app so we were afraid to work for nothing.
But I'll check with him how difficult is to build a database and the website.
```

---
## \#567 Posted by: DeathCookies Posted at: 2017-01-15T19:01:20.230Z Reads: 181

```
@gaetjen can You try The following? Maybe it is only a Bug for me and is working for you

First time i got asked for a Name of the Bluetooth Chip. I just called it test for testing purpose :smiley:
Now i want to rename my chip but it does Not work... When i have changed The Name and leave The text Input it does Not save the New Name...even after  if i have uninstalled The App, deleted The folder on my Smartphone and installed it again The Name of the Bluetooth Module stays The same "test"...
```

---
## \#568 Posted by: gaetjen Posted at: 2017-01-15T19:16:32.594Z Reads: 178

```
Yeah, I can't change the name of the board as well. But I haven't deleted the app yet, because I don't want to set up everything again :-)
```

---
## \#569 Posted by: DeathCookies Posted at: 2017-01-15T19:23:17.946Z Reads: 175

```
I did not want you to uninstall it :D i am sorry if you had The impression to! 

@Ackmaniac Okay then it is a Bug. Would be nice if you could fix it ;)
```

---
## \#570 Posted by: gaetjen Posted at: 2017-01-15T19:24:59.357Z Reads: 192

```
Here are my other driving modes and I have to say they work very good. Kid modes goes up to 6kmh, beginner mode up to 25 and medium up to 35 kmh. 

<img src="/uploads/db1493/original/3X/e/d/ed7ab6dc739bec737c6dfd694d921237edecde57.png" width="281" height="500">
<img src="/uploads/db1493/original/3X/9/6/96579ab1a60bfb2b6dd546799ca52a24fc6549b7.png" width="281" height="500">
<img src="/uploads/db1493/original/3X/3/f/3fed11a897656f77afa68529770815cc6ef7cd71.png" width="281" height="500">
```

---
## \#571 Posted by: Jamy Posted at: 2017-01-15T19:51:14.841Z Reads: 178

```
I can do that webpage if you want. Send me a PM with what you'd like the page to do!
```

---
## \#572 Posted by: DeathCookies Posted at: 2017-01-15T19:52:46.999Z Reads: 176

```
Some sort of statistics of many different runs and something like oneboxing
```

---
## \#573 Posted by: Ackmaniac Posted at: 2017-01-15T19:55:11.802Z Reads: 172

```
Yes it is a bug and will be fixed with the next version. I am working on a bigger change at the moment so you have to wait a little.
```

---
## \#574 Posted by: DeathCookies Posted at: 2017-01-15T19:56:51.145Z Reads: 179

```
Nice to hear. Can you tell us what the next update will unlock?

I like the idea that you setup default values and change the modes on the fly. By far the best app i think. I am only missing a "onebox" feature :D
```

---
## \#575 Posted by: Ackmaniac Posted at: 2017-01-15T20:11:19.466Z Reads: 184

```
Very nice video. But let me give you a view tips. You are overstressing your batterys a bit. Because you have a 10S3P battery (i guess samsung R25 cells) and set your battery max limit to 50A each VESC. but the battery is only rated to 20A continuous. For a 3P setup that means 60A.
That means you allow a total max amp draw of 100 Amps for the Battery. You can do that but it is a bit much. And what is the value for your your Voltage Cutoff start and end. Because i think it is a bit too high (reduces power too early). 
So i recommend to set the cutoff start to 30A and cutoff end to 28A. And then the best would be to set your battery max to 30A for each VESC or if you want a bit more power to 40A.
```

---
## \#576 Posted by: Ackmaniac Posted at: 2017-01-15T20:14:23.360Z Reads: 188

```
Just to give a little update. 
I am working currently on new Features which will be available soon.

**- Full Nunchuk support**
So you can connect the Bluetooth module to the slave VESC when you have a dual drive and still change ride modes and the settings.

**- Power output limit visualization**
That should mean if the VESCs output power is limited by the low voltage or the VESCs Temperature you will be able to see it in the app and in the Videos.

**- Throttle curve adjustments are possible via the app** 
Each drive mode can have it's own throttle curve.

**- BLDC-Tool with have help tooltip text for the most parameters**

**- Visualization of average motor and battery amp draw and average Temperature**
And this even in total and in ride time.
Total = it counts it also when the board is not moving. Useful when you want get a feeling how the amps raise the Battery's temperature.
ride time = it only counts when the board is moving. Useful to know how much amps you draw in average when you are riding.

And i fix the bug with the speed limit in the firmware. So also a new Firmware file will be necessary.
```

---
## \#577 Posted by: gaetjen Posted at: 2017-01-15T20:22:32.046Z Reads: 172

```
My cutoffvoltage starts at 32V and ends at 28V, but I have a 60A BMS that cuts voltage at 30V. I have LG2 cells, so 60A is correct. Thanks for the tips with the battery max, I'll try it with 30A then (I have a Vedder-switch as well with a 40A fuse). 
What about my Max Watt? Should I leave it at 1700 watt?
```

---
## \#578 Posted by: DeathCookies Posted at: 2017-01-15T20:22:49.949Z Reads: 171

```
[quote="Ackmaniac, post:575, topic:12286"]
set your battery max limit to 50A each VESC
[/quote]

He has set his battery max to 50A. How is it possible that he is exceeding that limit? Over 90A was his peak draw :open_mouth:


How does he even get 90A on one VESC by running dual? --> Total draw = 180A ?
Do you multiply the battery draw by two when the user is running dual?

[quote="Ackmaniac, post:575, topic:12286"]
So i recommend to set the cutoff start to 30A and cutoff end to 28A.
[/quote]

I think you mean voltage ;)
```

---
## \#579 Posted by: DeathCookies Posted at: 2017-01-15T20:25:35.328Z Reads: 168

```
Just a **minor** bug fix: if you choose between different mode setups you cannot read the complete ERPM value because the last digit gets cut.

PS: The new features are nice. Keep up the good work :thumbsup:
```

---
## \#580 Posted by: Ackmaniac Posted at: 2017-01-15T20:26:59.679Z Reads: 170

```
When you set the value to 30A then you should set the max watts to 1080 (3,6V * 10S * 30A = 1080 watts).
if you set it to 40A (at your own risk) then 1440 (3,6V * 10S * 40A = 1440 watts).

@DeathCookies Yes, when you have 2 VESCs then the value gets doubled to show the summarized amp draw and watts on the entire system.
```

---
## \#581 Posted by: fedestanco Posted at: 2017-01-15T20:27:40.094Z Reads: 169

```
Hi, I really appreciate your work although I havent tried your software yet.
Do you think you will be able to add a feature that can help the rider in case of wireless controller failure? For example a feature that will gradually slow down the board, instead of an abrupt power cutoff (in case of complete signal loss).
```

---
## \#582 Posted by: Ackmaniac Posted at: 2017-01-15T20:28:04.436Z Reads: 174

```
[quote="DeathCookies, post:579, topic:12286"]
Just a minor bug fix: if you choose between different mode setups you cannot read the complete ERPM value because the last digit gets cut.
[/quote]
Can you please make a screenshot of that.
By the way in the new version you don't have to deal with the ERPM anymore. You set your tire and pulley size and the motor poles and then you can adjust the speed instead of the erpm.
```

---
## \#583 Posted by: DeathCookies Posted at: 2017-01-15T20:29:57.477Z Reads: 177

```
Here you get it :) <img src="/uploads/db1493/original/3X/3/4/34004022ae6d3cabb0df310731f7bd354de76d35.png" width="281" height="500">
```

---
## \#584 Posted by: Ackmaniac Posted at: 2017-01-15T20:31:54.076Z Reads: 167

```
Looks like you have a very small screen and the values don't fit. looks different on mine. That is the problem with Android devices. There are so many different devices and screen sizes. But i changed it already on the new Version. Hopefully it will work then.
```

---
## \#585 Posted by: DeathCookies Posted at: 2017-01-15T20:35:55.099Z Reads: 166

```
I have a OnePlusOne 5,5". I do not think that it is small :D
```

---
## \#586 Posted by: gaetjen Posted at: 2017-01-15T20:37:15.016Z Reads: 169

```
I have a dual setup. Wouldn't I draw then 60A (2x30A) and set the max amp to 2160?
```

---
## \#587 Posted by: DeathCookies Posted at: 2017-01-15T20:38:20.320Z Reads: 167

```
[quote="fedestanco, post:581, topic:12286"]
Do you think you will be able to add a feature that can help the rider in case of wireless controller failure? For example a feature that will gradually slow down the board, instead of an abrupt power cutoff (in case of complete signal loss).
[/quote]

That is already given even with the normal BLDC-Tool. 
App Configuration
--> General
--> Brake current to use when a timeout occurs (A)
```

---
## \#589 Posted by: Ackmaniac Posted at: 2017-01-15T20:39:18.317Z Reads: 161

```
[quote="gaetjen, post:586, topic:12286, full:true"]
I have a dual setup. Wouldn't I draw then 60A (2x30A) and set the max amp to 2160?
[/quote]
You set it for each VESC individually like you would do in the BLDC-Tool. So only 1080.
```

---
## \#590 Posted by: fedestanco Posted at: 2017-01-15T20:39:23.343Z Reads: 159

```
Thanks. I tried to find this info for days. I love this forum.
```

---
## \#591 Posted by: Ackmaniac Posted at: 2017-01-15T20:42:34.237Z Reads: 164

```
Sadly mostly it isn't a complete signal loss. Because that would only happen when the Receiver gets disconnected from the VESC. So the receiver gives the idle signal and the VESC thinks the remote is still available. There is not really a possibility to avoid that. Only chance would be to reduce the current ramping of the VESC. It would be better to fix the connection issues so that you have no dropouts.
```

---
## \#592 Posted by: Ackmaniac Posted at: 2017-01-16T01:22:03.334Z Reads: 169

```
The new firmware is fished today. Now I only have to make some last tests and review the code a second time and hopefully I can release it by tomorrow. I think this version of the bldc-tool will be a great help because there is a help for the most of the parameters we use. I think that can self a lot of problems for beginners. Took me the entire weekend to write all those texts.
```

---
## \#593 Posted by: mmaner Posted at: 2017-01-16T01:27:26.852Z Reads: 170

```
U r a rock star sir 😎
```

---
## \#594 Posted by: Eboosted Posted at: 2017-01-16T02:03:20.190Z Reads: 193

```
Hello @Ackmaniak, I just finished my build today and inmediately uploaded you FW to both VESCs, and  I'm having some issues, hope you can give me a hand:

1. On the bench, if I go full throttle and brake only one motor brakes, the other one just slows down
2. If I give it throttle inmediately after braking wheels do not spin, I need to wait until they stop and throttle works again
3. If I hold 20% of throttle it slowly goes up to full speed in 8-10 seconds, not sure i this is normal
4. If I go full throttle and then try to slow down, it keeps going full throttle, only when I reduce the throttle to 15-10% it starts to slow down, there's an on/off feeling

Here are my VESC settings:

[img]http://i.imgur.com/QQE17lX.jpg[/img]
[img]http://i.imgur.com/XKsmDPs.jpg[/img]
[img]http://i.imgur.com/QQE17lX.jpg[/img]

[img]http://i.imgur.com/WYjQAaJ.jpg[/img]
[img]http://i.imgur.com/6cVLKLr.jpg[/img]
```

---
## \#595 Posted by: mmaner Posted at: 2017-01-16T02:08:59.783Z Reads: 181

```
A lot of that, if not all,  will change when its under load.  The only thing you essentially get as far as real world conditions when bench testing is whether it works or not.
```

---
## \#596 Posted by: Ackmaniac Posted at: 2017-01-16T02:32:13.842Z Reads: 180

```
Something is terribly wrong. Post pictures of the settings of both VESCs. I need the motor, bldc, advanced, general and PPM tab. I see already that your battery cutoff start and end Is not adjusted. And the battery max at 60 amps is too high for a dual and the battery min as well. But that doesn't explain your problems.
```

---
## \#597 Posted by: Eboosted Posted at: 2017-01-16T02:45:55.762Z Reads: 181

```
I set up everything, even Maximum inpit voltage to 42V and Battery cutoff start to 37V, PPM pulsewidth and after a while I loose all data and I need to set it up again.

At the time I'm setting up two boards, and using the same USB cable and the BLDC tool for both, I think this happwens whenI switch from the VESC from one board to another
```

---
## \#598 Posted by: mortorojo Posted at: 2017-01-16T02:49:58.814Z Reads: 179

```
When on a dual motor does Max Watt need to be set on both vesc's, or can that value be set for the master and it work for the slave too?
```

---
## \#599 Posted by: Eboosted Posted at: 2017-01-16T02:51:56.479Z Reads: 180

```
@mortorojo that's a great question, I'm wondering the samething.

But If I set the max watt on the slave, nothing happens, if I do it in the master it works
```

---
## \#600 Posted by: Ackmaniac Posted at: 2017-01-16T03:01:37.961Z Reads: 182

```
When you change the settings then you also have to write the settings after the change so that the VESC keeps the data.  And if the VESC still looses the information then something is wrong with the VESC. And Max input voltage should be 57V.
```

---
## \#601 Posted by: Ackmaniac Posted at: 2017-01-16T03:09:21.187Z Reads: 183

```
It's enough to set max watt for the master. It is also remote related (PPM).
```

---
## \#602 Posted by: Eboosted Posted at: 2017-01-16T06:46:30.914Z Reads: 208

```
@Ackmaniac, so, any setting you input on a dual setup must be only stated on the master VESC?, all values on the slave VESC would be overwritten?

A friend and I are building two boards with almost the same setup, dual belt 6355 Polar motors, Torqueboard VESC, 10S4P with Samsung 25R battery packs.

We just tested the the first build in a parking lot, after 5 small tests we got a broken master VESC, no response from remote, red led on VESC is blinking, motor detection failed, we uploaded the Ackmaniac FW again, but samething, still fails at motor detection, I'm disturbing how all these VESC are so fragile, good thing is Dexter would not let us alone with this problem, so far, great customer service!

If I write "faults" on terminal, it says "No faults registered since startup", that's a small relief, so the VESC could still be good to go, nevertheless, at the moment, the motor connected to that VESC does not spin, if I plug a new VESC it works perfect.

Here are some pictures of the bad VESC, do you guys see anything wrong or burnt?
[img]http://i.imgur.com/EEdXJ2U.jpg[/img]
[img]http://i.imgur.com/4ntqd29.jpg[/img]
[img]http://i.imgur.com/BQpmTkV.jpg[/img]

In regards the second build, here are my master VESC settings, we extremely afraid to burn one more VESC, I still haven't test it outside because of this, would you guys please take a look a these settings?

[img]http://i.imgur.com/gCEKnNb.jpg[/img]
[img]http://i.imgur.com/ngpMwBk.jpg[/img]
[img]http://i.imgur.com/pkTwASI.jpg[/img]
[img]http://i.imgur.com/ao98sTK.jpg[/img]
```

---
## \#603 Posted by: Ackmaniac Posted at: 2017-01-16T07:09:37.648Z Reads: 170

```
At Master and Slave:
Set battery max to 30A, battery min to - 8A, battery cutoff start to 30V, battery cutoff end to 28V.

At Master:
Disable Send status over can. 

At the Slave:
Enable Send status over can. 
Set app in the General Tab to None

You have to do a motor detection for both VESCs. 
When you change motor values at the Master you have to do that also for the Slave as well.

When you are finished please post the same Screenshots for the Slave Vesc
```

---
## \#604 Posted by: Eboosted Posted at: 2017-01-16T07:47:31.343Z Reads: 197

```
Thanks @ackmaniac, here are the screenshots for the slave VESC as requested:

[img]http://i.imgur.com/IC6cNPW.jpg[/img]
[img]http://i.imgur.com/qG9cxKV.jpg[/img]
[img]http://i.imgur.com/JqwCKNy.jpg[/img]
[img]http://i.imgur.com/X47PP5G.jpg[/img]

1. My battery is a 10S4P with Samsung 25Rs, so 2.5A/hr * 8C * 4P = 80A, 40A on each VESC, I wonder why do you suggest to set it to 30A?

2. Should "max watt" be (3.7V * 10S) * 60A = 2220 Watts / 2 VESC = 1110 Watts on each VESC, but state it only 1110 watts on the Master VESC?

3. When I do motor detection for each VESC, the "Integrator Limit" and the "BEMF Coupling" are different between each motor, should I use the independent detected value for each motor, they are usualy different, or should I use the same values for both motors?
```

---
## \#605 Posted by: Ackmaniac Posted at: 2017-01-16T08:26:33.978Z Reads: 186

```
Does the board work now?

[quote="Eboosted, post:604, topic:12286"]
My battery is a 10S4P with Samsung 25Rs, so 2.5A/hr * 8C * 4P = 80A, 40A on each VESC, I wonder why do you suggest to set it to 30A?
[/quote]

Correct, but i think you are a beginner and i want you to be safe. Once the board is running i would have told you that you can do that in the future.

[quote="Eboosted, post:604, topic:12286"]
Should "max watt" be (3.7V * 10S) * 60A = 2220 Watts / 2 VESC = 1110 Watts on each VESC, but state it only 1110 watts on the Master VESC?
[/quote]

Correct, this value tells the master that it should use 1110. During riding the master tells the slave to do what the master is doing itself.

[quote="Eboosted, post:604, topic:12286"]
When I do motor detection for each VESC, the "Integrator Limit" and the "BEMF Coupling" are different between each motor, should I use the independent detected value for each motor, they are usualy different, or should I use the same values for both motors?
[/quote]

By manufacturing each motor is a bit different. You see that the values differ only a little bit. So i recommend to do a motor detection for each motor individually.



And one thing i forgot, you should set in the Masters PPM Tab the soft RPM limit. ERPM limit start to 58000 and ERPM limit end to 60000.
And set the Traction control Offset to 3000 and the Traction control ERPM diff to 5000. (Works better)
```

---
## \#606 Posted by: Jamy Posted at: 2017-01-16T10:48:31.212Z Reads: 177

```
@Ackmaniac looks like you missed [my previous post](http://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286/571?u=jamy). 

I can write that data upload webpage for you if you want, just need some specifics on what you want the page to display and how :) 

Hit me up!
```

---
## \#607 Posted by: DeathCookies Posted at: 2017-01-16T15:45:45.501Z Reads: 189

```
Currently i am working on a webpage like metr.at that is why he did not say any thing anymore. 

Currently i have programmed The Route overlay for Google maps. Now i Need to make the summary, a good graph, display the values in the graph and connect the route points to the graph points. 
<img src="/uploads/db1493/original/3X/4/e/4e6d4508af2877a55512856a94d0cd9f6d3952ce.jpg" width="690" height="342">
```

---
## \#608 Posted by: Jamy Posted at: 2017-01-16T15:59:45.052Z Reads: 182

```
Cool, let me know if you want some help :)
```

---
## \#609 Posted by: Eboosted Posted at: 2017-01-16T20:25:38.191Z Reads: 183

```
The 1st board does not work, the master VESC went bad. 

The 2nd board works on the bench, but I haven't test it yet on the road, testing tonight, hope to not burn another VESC again.

Thanks for all thje input @ackmaniac, I'll keep you posted
```

---
## \#610 Posted by: Ackmaniac Posted at: 2017-01-17T01:49:57.625Z Reads: 183

```
Good to hear that at least one is working. 

To keep you updated about the firmware update. I figured out today that I don't like the way the cruise control is handled. So I decided to try some improvements and that's keeping me busy at the moment. 
But when that what I am trying right now works then cruise control will be buttery smooth during carving. 
It's already cool in the actual firmware but if my theory is right then it will be f* awesome.
```

---
## \#611 Posted by: Eboosted Posted at: 2017-01-17T04:57:17.156Z Reads: 177

```
I replaced the blown VESC on the 1st board, borrowed it from 2nd build, used your settings,  restricted the "max watt" to 200 and went for a test ride, this time no more blown VESC, even after 5 miles riding it, not sure if restricting "watt max" would keep the VESC from blowing, but so far so good, it passed the test. 

If I go very gently on the throttle from a dead stop, the motors start to shake, I need to give it more throttle to avoid this behavior, is there any setting to keep this from happening? 

If everything goes well after a couple of days testing it, would you suggest to increase the "watt max" to 1100 or increase the max battery voltage to 30A, 40A or 80A?
```

---
## \#612 Posted by: Pimousse Posted at: 2017-01-17T08:00:59.197Z Reads: 176

```
I love this project !
I would really enjoy to help if needed.
@Ackmaniac : Is it complicated to build an API to ease the connection between your app and a website ?

When I rode bike on tracks, I used an app (Racechrono) which was able to push data to a website ( https://serious-racing.com ) that was a kind of database. Then, I could compare times with other users and analyze your ride with many statistics and routes.
A website like connected to Ackmaniac's app and firmware would be awesome.

Seriously guys, so many talents here and so many possibilities (app, website, and so on), it's a f***** exciting project !
Just keep working together instead of jumping into an business model, please ! :wink:
```

---
## \#613 Posted by: Ackmaniac Posted at: 2017-01-17T08:45:45.003Z Reads: 172

```
That is what DeathCookies, Jamy and i are doing. They are working on the webpage part. Looks already very cool.
```

---
## \#614 Posted by: Pimousse Posted at: 2017-01-17T09:22:30.624Z Reads: 170

```
:astonished:
Keep us updated ! Pleaaaaaase !
```

---
## \#615 Posted by: Ackmaniac Posted at: 2017-01-17T09:38:54.776Z Reads: 168

```
It's their project so they should provide you with information. Also they should get the shoulder clap. Not i.
```

---
## \#616 Posted by: DeathCookies Posted at: 2017-01-17T09:56:57.553Z Reads: 175

```
I will keep you all updated. In the next days i will make a thread or let Ackmaniac Update this thread description.
```

---
## \#617 Posted by: Ackmaniac Posted at: 2017-01-17T09:59:23.916Z Reads: 182

```
Make your own, i guess a lot of people have questions and ideas
```

---
## \#618 Posted by: DeathCookies Posted at: 2017-01-17T11:47:20.798Z Reads: 189

```
Would be nice if someone could share a long log-file with gps data (more than 10 minutes) for developing/testing
Maybe @Maxid @Jamy @SageTX @Pimousse
```

---
## \#619 Posted by: Maxid Posted at: 2017-01-17T11:52:19.764Z Reads: 190

```
I would - but I dn't have one with GPS right now and haven't ridden the board in a while.
Weather (and wet/salty roads) needs to be better before I take my precious :ring:  board out again.
```

---
## \#620 Posted by: Pimousse Posted at: 2017-01-17T12:17:59.776Z Reads: 192

```
I'll see if I have somes with GPS data.
```

---
## \#621 Posted by: SageTX Posted at: 2017-01-17T18:40:37.762Z Reads: 180

```
Just looked for previous files, but I completely reinstalled and don't have any. Will share as soon as I can.
```

---
## \#622 Posted by: DeathCookies Posted at: 2017-01-17T19:49:17.289Z Reads: 194

```
@Pimousse @Maxid @SageTX Thanks for the help. Right now i have enough test data.
I just need to develope the webapp. A little teaser:
<img src="/uploads/db1493/original/3X/1/a/1a13bab3e1cd502501ad4bbba7fd24e554155b6b.png" width="630" height="500">
```

---
## \#623 Posted by: SageTX Posted at: 2017-01-17T20:09:47.587Z Reads: 174

```
Oh cool. Wish I'd saved some of my previous rides!  How long of a ride is the graph optimized for? I've ridden up to an hour or so. Would it look too "squished"? 〽
```

---
## \#624 Posted by: DeathCookies Posted at: 2017-01-17T20:24:25.377Z Reads: 166

```
Just after analyzing it can look bad or good but you have the ability to zoom in any area you wan (the lower part of my picture)
```

---
## \#625 Posted by: Okami Posted at: 2017-01-17T20:59:13.597Z Reads: 172

```
Cool. How many hours are you working now on this one? 

Heh, a side note - I think it is okay we did not finish that esk8database, @tueboard took care of that and made a really good one in a ''matter of days'' :)
```

---
## \#626 Posted by: DeathCookies Posted at: 2017-01-17T21:59:15.659Z Reads: 175

```
Since two days. Lets stay on topic here ;)
```

---
## \#627 Posted by: Ackmaniac Posted at: 2017-01-18T19:32:08.070Z Reads: 187

```
Just a little teaser for the coming features. Video itself is bad (sorry) but it's only about the data.

Especially the information about the average amp hours is very interesting. I was surprised how low it is. It was only chilled cruising because mainly i was testing my new modified cruise control (it works :grin:). But i think we are able to see that if we setup 80 battery amps total (40 each at dual drive) that we are far away from drawing that contentiously.

https://youtu.be/nP0ZPTODwYs

<img src="/uploads/db1493/original/3X/d/2/d247d1517597ca7a12ca0a3404be08ee9faa8174.png" width="281" height="500">

1. Total Average Speed over the entire time (stops are counted)
2. Riding Average Speed  (stops are not counted)
3. The Volt Label will turn yellow when the VESC reduces the power because the Battery limit start is reached and red when the battery limit end is reached.
4. The actual volts for a single cell
5. The TemperatureLabel will turn yellow when the VESC reduces the power because the Temperature limit start is reached and red when the Temperature limit end is reached.
6. Average Motor amps over the entire ride time (stops included) drawn | charged
7. Average Motor amps over the entire ride time (stops not included) drawn | charged
8. Average Battery amps over the entire ride time (stops included) drawn | charged
9. Average Battery amps over the entire ride time (stops not included) drawn | charged
10. Average Temperature over the entire ride time (stops included)
11. Average Temperature over the entire ride time (stops not included)
```

---
## \#629 Posted by: Maxid Posted at: 2017-01-18T19:52:34.033Z Reads: 172

```
You'll still need one - otherwise your voltage will sag too heavily.
```

---
## \#630 Posted by: Ackmaniac Posted at: 2017-01-18T20:05:56.432Z Reads: 175

```
It is still nice to have a high discharge battery. But we don't need to reduce the max battery amps that can be drawn to half the continuous discharge rate because we are far away from doing that contentiously. But i don't want to talk about that here in detail. There are enough other threads already about it. I only want to provide the tool that everybody can collect and share their own data. So we can stop guessing and hopefully get rid of a couple of myths.
```

---
## \#631 Posted by: Pimousse Posted at: 2017-01-19T08:44:21.170Z Reads: 171

```
Awesome !!!
I can't wait to test it !

But I can see something strange on bargraph.
How are set the scale ?

i.e. at a moment, you reach 60A with the motor and the bar was half full.
Oh, and it's also strange that you could go over 60A (max current motor shown in the the mode tab), isn't it ?
Or is it due to your dual configuration ? (so the scale is twice the motor current parameter)
```

---
## \#632 Posted by: Ackmaniac Posted at: 2017-01-19T08:46:19.904Z Reads: 179

```
These values get multiplied by the amount of VESCs. If you only want to see it for a single one then say that you only have 1 VESC

<img src="/uploads/db1493/original/3X/a/f/afe45af8634c6f189d50f6910475d630497b13a9.png" width="281" height="500">
```

---
## \#633 Posted by: Pimousse Posted at: 2017-01-19T08:54:28.069Z Reads: 172

```
Yes, I got that.
It was mostly for the bargraph scale.
Are the max and min scale for green and red bar calculated from the Bat/Motor max and min parameters (multiply by the amount of VESC) ?
```

---
## \#634 Posted by: The_Dude Posted at: 2017-01-19T10:50:19.262Z Reads: 175

```
Awesome, sehr geil. But: iOS pleeeeease :grin:
```

---
## \#635 Posted by: Ackmaniac Posted at: 2017-01-19T11:08:50.098Z Reads: 170

```
Yes the red and green bar shows the maximum that is allowed by the actual settings. So you always see if you push any of the limits.
```

---
## \#636 Posted by: TarzanHBK Posted at: 2017-01-19T13:31:48.142Z Reads: 175

```
Again such a good job!
This app looks so good and shows lots of cool stuff to get a better understanding for our boards.
Thx very much for putting so much efford into this Ack!
Much love from your german brotha :kissing_heart:
```

---
## \#637 Posted by: Okami Posted at: 2017-01-19T15:28:30.958Z Reads: 187

```
Have you considered once again to place a temp sensor on batteries? I think this is the only way how to see, if batteries get a bit more damaged with heat or not.. and especially - to see when this heat starts to happen in them.

I think you mentioned you have such an idea but it seems there is not much info when you plant to implement this and show us some more complete picture about battery discharge characteristics..

So far we only know that there is not a continous charge happening for batteries, so you just recommend not to sitck to ''being safe with batteries'' but instead to use them fully.. 

At least that is what I got from you from other posts/commentions you've made in some other topics!

--

IF this goes astray a bit, please say so, can write some of that in private info or edit away
```

---
## \#638 Posted by: Ackmaniac Posted at: 2017-01-19T16:28:56.732Z Reads: 183

```
I will make videos with a temperature attached. But not to the VESC. But it would be possible to attach temperature sensors. Also for the motors which would make more sense to me.
```

---
## \#639 Posted by: Okami Posted at: 2017-01-19T16:51:42.037Z Reads: 189

```
Yeah, it can be either motor or battery. I also had idea to mount thermistor to a motor but then I just came up with an idea to install an outside 3d printed fan to help with cooling!

I have not installed it yet but If I saw that my motor warms up a lot, I would probably install it.

Besides that - This is what I saw in your video - if there was a place for motor temp or battery temp, then we would get a lot more info, related to these two other electronic devices, we use besides vesc!
```

---
## \#640 Posted by: Ackmaniac Posted at: 2017-01-19T23:01:40.480Z Reads: 198

```
At the moment i spent some time optimizing the cruise control so that it can be used for carving. In the actual firmware it is already quite nice but in the next release it will be even better. But to make the same optimization for the Nunchuk is not that easy. The cruise control PID controller will also be adjustable via the app later on. Because each time the motor amps get changed the PID controller needs fine adjustments. But with the app it will be easy to find a good setup quickly.

I also want to implement the feature to change from BLDC to FOC via app. But for that a restart will be necessary. That means you press the butten in the app and it will take around 3 seconds to update and restart the Master and all slave VESCs.
So you can decide by yourself if you want to run in silent or sound mode.
I will also check if the FOC or BLDC motor setup was executed. Otherwise i won't allow the change.
```

---
## \#641 Posted by: Eboosted Posted at: 2017-01-20T04:37:33.216Z Reads: 200

```
@Ackmaniac So we just need to connect the steering channel from the mini receiver to the slave VESC and choose "Cruise control via Secondary Channel" and that's it?

Or do we need to tweak something else?
```

---
## \#642 Posted by: Ackmaniac Posted at: 2017-01-20T07:07:45.676Z Reads: 197

```
You also have to adjust the pulse with min,  center and max and set the application to PPM. Because cruise gets activated when you steer 30% to the left or right.
```

---
## \#643 Posted by: DeathCookies Posted at: 2017-01-22T16:01:25.610Z Reads: 246

```
Your voltage will sag either way!
I have 12S 8Ah Zippy Flightmax rated to "30C". They have enough juice but the voltage still sags but the battery draw was at peak 21.17A! Maybe it is just because the battery is a 1P but they can deliver at least 100A
<img src="/uploads/db1493/original/3X/2/3/23192e857db6b651aafeb3edd9d6a0fdf3b430fe.png" width="690" height="364">
```

---
## \#644 Posted by: Ackmaniac Posted at: 2017-01-22T19:56:09.234Z Reads: 249

```
**I published the new Firmware 2.53**

**The BLDC-Tool now has Tool-tips** to the most parameters so that it should be more understandable what those parameters mean. They also include tips to which values you should set them based on your battery or motors. To see them please go with the mouse to the parameters Name and don't move the mouse. After a second or 2 they should appear. 
**FOC motor detection should be a bit easier because i added a numbering of the steps and a little explanation.**

**PPM has a setup wizard for the minimum, center and maximum pulse-width.** This should make it easier for newbies to set it up.

**PPM has a new Cruise Control calculation for Current control and Watt control.** It makes the ride smoother especially when you carve at cruise control.


**---------------------------------------------------------------------------------------------------------------**
**A lot of new features are added which improves the communication with my app.**
**---------------------------------------------------------------------------------------------------------------**

**- Full Nunchuk support (NRF should work as well)**
So you can connect the Bluetooth module to the slave VESC when you have a dual drive and still change ride modes and the settings.

**- Power output limit visualization**
That should mean if the VESCs output power is limited by the low voltage or the VESCs temperature you will be able to see it in the app and in the Videos.

**- Throttle curves are adjustable via the app** and for each drive mode individually.

**- Support for @DeathCookies web too**l so that all the data can be detected and visualized

**- Each time the app starts it first asks all the VESCs in the system for Faults and shows detailed information.** These will be shown on the main screen.

**- If a fault is detected on the master VESC during a ride it will be shown on the Main Page with detailed information**. Sadly it is not possible at the moment to detect faults of Slaves after the first startup. So if you think one of the slaves had a problem just simple close and start the app and all VESCs will be asked for faults. Later on i will implement a button to ask at any time. 

Errors are shown like this
<img src="/uploads/db1493/original/3X/6/6/661d904d5afcb040ec52a472280fad3c19153158.png" width="281" height="500">

**- You can connect to each slave in the system, or to the Master via Slave** by enabling the can communication in the settings and adjust the controller Id of the VESC you want to communicate with. this way it is also possible to connect to the master when the Bluetooth module is connected to the Slave.

**- Supports Realtime data for standard Vedder Firmware.** Aditional features only work with my firmware mod. But the actual motor settings and the Realtime data is also visible for the standard firmware.

**- Average Motor, Battery and Temperature values** are calculated and shown for total time and also for riding time only.

And i fix the bug with the speed limit in the firmware. So also a new Firmware file will be necessary.

I fixed a bug with the communication to the Bluetooth module and it is very stable now. If it looses connection it will reconnect automatically within a second.


_As always google needs half a day for to publish the new Version in the Play store. If you can't wait you can find the apk file in my Dropbox link in the first post of this thread._




[Windows BLDC-Tool, Modified Firmware, Ubuntu BLDC-Tool and Android app](https://www.dropbox.com/sh/t7dl90owz5ccbyl/AAANyC-yQCMeveA7errNRnYqa?dl=0)

Android App download
[Android App](https://play.google.com/store/apps/details?id=ackmaniac.vescmonitor&hl=de)

[Bluetooth modules ca be ordered here.](https://de.aliexpress.com/item/HM-10-BLE-Bluetooth-4-0-CC2540-CC2541-Serial-Wireless-Module/32516357718.html?spm=2114.13010608.0.0.cbyTeS&detailNewVersion=&categoryId=400103)

Cable to connect the Bluetooth Module with the VESC easily
[Cable with Connector](https://www.aliexpress.com/item/2-0mm-PH-7-Pin-Male-Female-Connector-with-Wire-x-10-Sets/32616271304.html?spm=2114.01010208.3.18.RewfhB&ws_ab_test=searchweb0_0,searchweb201602_3_10065_10068_10000032_10000025_10000029_430_10000028_10060_10062_10056_10055_10054_10059_10099_10000022_10000012_10103_10102_10000015_10101_10096_10000018_10000019_10052_10053_10107_10050_10106_10051_10000007_10084_10083_10080_10082_10081_10110_10111_10112_10113_10114_10115_10037_10032_10000041_10000044_10078_10079_10077_10000038_429_10073_10000035,searchweb201603_1,afswitch_2,single_sort_2_default&btsid=0ef89f27-529d-4685-8740-13e10dbd5fcc)

And if somebody wants to honor all the work.
[Donations](https://www.paypal.com/de/cgi-bin/webscr?cmd=_flow&SESSION=-P6lRlkFOyJeroABtf7htelg80qLQk2pKvQD8dkA_L3ff5QSvJmz8Z0LeQK&dispatch=5885d80a13c0db1f8e263663d3faee8d333dc9aadeed3fe0b5b299d55fd35542)
When you want to send a donation then don't use dots. (Germany uses commas). So use full numbers or a comma.
```

---
## \#645 Posted by: jmasta Posted at: 2017-01-22T20:09:13.907Z Reads: 206

```
I've been following this for awhile, but I must say that this looks pretty amazing

Would you ever consider an iPhone version?  I would easily pay $5-10 for an app like this
```

---
## \#646 Posted by: IDVert3X Posted at: 2017-01-22T20:59:30.726Z Reads: 200

```
Use the search function, it has been asked a few times already.
```

---
## \#647 Posted by: Okami Posted at: 2017-01-22T21:09:14.308Z Reads: 204

```
So - from these who have already tried the new BLDC tool 2.53 - how does it look? 

**Can you feel the improvement?**

 Im especially interested in how these Tooltip text fields turned out! Does it offer info which was not momentarily available in the bldc tool?
```

---
## \#648 Posted by: DeathCookies Posted at: 2017-01-22T21:12:52.603Z Reads: 193

```
- Watt-Control ist awesome
- Data-Monitoring is working flawlessly
```

---
## \#649 Posted by: Ackmaniac Posted at: 2017-01-22T21:15:14.340Z Reads: 189

```
Just download it and test it. To see the Tooltip texts you don't need to connect a VESC. Only start BLDC-Tool.
```

---
## \#650 Posted by: The_Dude Posted at: 2017-01-22T21:17:55.308Z Reads: 193

```
Great, thank you! You also made modifications to the firmware compare to the source you published the last time in "Modded BLDC complete source code.zip"? I try to check and compile your FW for my VESC4.7 HW - so would be good to know.
```

---
## \#651 Posted by: SeanHacker Posted at: 2017-01-22T22:34:14.103Z Reads: 192

```
Great job @Ackmaniac!!!
```

---
## \#652 Posted by: SageTX Posted at: 2017-01-22T23:48:16.415Z Reads: 188

```
AWESOME JOB @Ackmaniac !!!!   Thanks!
```

---
## \#653 Posted by: The_Dude Posted at: 2017-01-23T07:52:58.879Z Reads: 190

```
Ok guys - this latest announcement from Ackmaniac finally forced me to akt reagarding the fact that the AckApp won't run on my iPhone. Hijacked the Android phone of my youngest son :smiling_imp:
```

---
## \#654 Posted by: jmasta Posted at: 2017-01-23T16:43:32.203Z Reads: 198

```
[quote="IDVert3X, post:646, topic:12286, full:true"]
Use the search function, it has been asked a few times already.
[/quote]

I realize it has been asked before; I have been following this thread since day one.  

But if people don't keep asking, it will never happen.  There has be a continued interest in an iPhone version to convince Ackmaniac (or others) to develop one

From what I recall, the main arguments against an iPhone version were (1) the developer costs, and (2) lack of access to a Mac/iPhone.    If the app cost $5-10 to download, the $100/year in developer fees would be easily covered and then some. I would throw $10 to your developer fees right now, and I'm sure 9 others would too.  Lastly, you don't need a Mac or an iPhone to produce apps for them; all you need is a virtual machine running X-code.

Fact of the matter... iPhone users are a bit in the dark here. There isn't one solid app that do both data monitoring/logging as well as VESC configuration with watt control.  I sincerely appreciate all the hard work of the developers doing this stuff in their spare time
```

---
## \#656 Posted by: E-Boarding Posted at: 2017-01-23T20:11:22.367Z Reads: 191

```
I finnally got an Android Phone because of this App. You can get old Android Phones pretty cheap.
I fully understand that he is not providing an IOS-Version.
Porting an APP to different platform takes a lot of time and for IOS a lot of money too and it's not fun. I rather want him to put this time into more feature and bugfixes.
```

---
## \#657 Posted by: jmasta Posted at: 2017-01-23T20:52:36.910Z Reads: 196

```
[quote="hexakopter, post:655, topic:12286, full:true"]
10$ is a joke compared to the time and work it takes.
[/quote]


$10 from one person is meaningless.  $10 from many people is not. A crowd-funded iPhone VESC app of this caliber could be very successful.  I am aware of the amount of work that this entails; I am also aware that almost half of all [USA] smartphone users have an iPhone.

EDIT:  Source: http://fortune.com/2016/10/24/apple-market-share/
```

---
## \#658 Posted by: DeathCookies Posted at: 2017-01-24T02:08:56.495Z Reads: 198

```
The tool is more or less finished @Pimousse @maxid @SageTX @Okami
http://www.electric-skateboard.builders/t/vesc-data-log-analyzer-vdla/16582?u=deathcookies
```

---
## \#659 Posted by: IDVert3X Posted at: 2017-01-24T15:50:47.644Z Reads: 194

```
[quote="jmasta, post:657, topic:12286"]
I am also aware that almost half of all smartphone users have an iPhone.
[/quote]

Maybe in the US, in the rest of the world, not really.
```

---
## \#660 Posted by: Maxid Posted at: 2017-01-24T16:08:49.741Z Reads: 201

```
[quote="jmasta, post:657, topic:12286, full:true"]
I am also aware that almost half of all smartphone users have an iPhone.
[/quote]
http://static3.businessinsider.com/image/5665bad08430761a008b7ef9-1200-900/20151207_smartphone_bi.png
```

---
## \#661 Posted by: Stefan Posted at: 2017-01-24T16:21:50.847Z Reads: 192

```
Well, my impression does not really match that statistic. Not claiming it was not true, but i would say more than 60% of my friends have an iPhone. And they belong to the main target group of electric longboards. Beside that target group, i see far more people using non-IOS smartphones. Maybe that statistic is not the best one to look at here?
```

---
## \#662 Posted by: Ackmaniac Posted at: 2017-01-24T17:12:27.574Z Reads: 202

```
I can understand all the concerns that there is no apple app. 
The reasons are:
- i don't have experience in developing Iphone apps
- i don't have a developer account
- i don't have a MAC
- i don't have a IPhone
- no time at the moment
- want to finish the Andoid App with the features i have in mind

I don't want to offend anybody but i will delete future posts about the IPhone discussion because many times people ask me if i can give explain them what the need to do get the firmeware, bldc-tool, bluetooth module and app installed because they don't want to read more than 600 posts. So please try to stay a bit on topic. (I know IPhones could be counted as a topic but it doesn't help in improving the app or firmware mod).
```

---
## \#663 Posted by: Ackmaniac Posted at: 2017-01-24T17:16:41.529Z Reads: 195

```
[quote="Okami, post:647, topic:12286"]
Can you feel the improvement?
[/quote]

You can feel that cruise control in PPM mode changed for dual drives(smoother at carving) and the app has more features. Also NRF should be supported now (somebody has to test it) as well as the possibility to connect the bluetooth module to the slave when a Nunchuk is connected to the master.

Cruise Control now takes both wheels into account and adjusts the speed for each wheel. Because of that it needs some time that both wheels come to the same speed when the board is on the bench. But during riding it works nicely because when you make corners the inner wheel is slower then the outer wheel.
```

---
## \#664 Posted by: Okami Posted at: 2017-01-24T18:37:26.643Z Reads: 205

```
hah yeah I did take a look.. The text descriptions were really nice.. sort of like you were sitting right next to me and explain what each settings does.. thumbs up for that!

I found a very minor (text) mistake here:

<img src="/uploads/db1493/original/3X/e/9/e9f8f85310fd5e351cf8f8d5cdc4f7c868d2f1a7.png" width="520" height="498">

Instead of word ''devide'' there probably should be ''divide''

You should care very much about it.. especially if the text description might change in the future.. just a little note..
--

Anyways nice Job! For me.. who has not used a vesc before.. almost all of the settings in this window were easy to understand with the help from tooltips alone..

Besides, were nice, if there was some kind of information, that these tooltips exist now (if there werent any before).. since I assume some ppl might just download your firmware without knowing it has been updated (then again, how many ppl there are who download yours straight away, as their got their vesc in their hands..)

The only a bit harder part was to understand what each ERPM setting meant but I think there were general example to just leave it at '60 000' and that's it.

I wonder when Benjamin vedder will release his new app / bldc tool,  which some ppl are waiting for here.. (vescs too, of course :D )
```

---
## \#665 Posted by: Ackmaniac Posted at: 2017-01-25T00:36:50.310Z Reads: 209

```
Just made some small updates. 
I didn't like the motor and battery's total average values. Because it doesn't make that much sense when you make a long brake. So i replaced that value by the **"Active"** value. So only when amps are drawn or charged it will be counted. When you coast and don't touch the throttle it won't be counted.
So the average **"Active"** value is for that and the average **"Riding"** value is to have the average amps when the board is moving. This way we can get good values to find out in which way we use the battery's.

Also the **average watts during riding** are added in the last line besides the average Temperature.

i also added the **question mark button** with that you can ask all the VESCs in the system if any of them had a fault during the ride. When you press the "Check for faults" and you see nothing then there was no fault. But you have to be connected to the Master to check all VESCs automatically.

<img src="/uploads/db1493/original/3X/e/c/ec6884f25f756b0a128a0fc9d74acea0d24de8ff.png" width="281" height="500">

<img src="/uploads/db1493/original/3X/d/f/dfac1f54e55b3bab320b60e5123ebfcf4927adce.png" width="281" height="500">

next feature is that the throttle curve, braking at cruise control and the cruise control PID Controller is adjustable by the app for each mode. So you can decide if you use the settings which you have for your default mode or if you want to override it with individual settings when you activate this mode. this way it should be easy for everybody to find the sweet spot for the cruise control. 
(Hint: When Motor amps get changed a lot then you normally need to adjust the PID Controller, good setting for 60 Motor max is P=0.0040, I=0.0040, D=0.0000)
<img src="/uploads/db1493/original/3X/d/7/d790d7bd723bedadf0230e238d81412ec3e50c31.png" width="281" height="500">

And of course the throttle curve is adjustable for each individual mode as well via the app
<img src="/uploads/db1493/original/3X/7/c/7c57608ff8a1a6c5473d4aa39f1848b8d4029a50.png" width="281" height="500">

i think now we have everything we need to create a couple of drive modes for every situation. 
Like Carving mode, Chill mode, Power mode, Kids mode, Hangover mode, Ludicrous mode and so on. And if you have more than one board then the apps remember the settings for each one. So adjust it ones for each of them and that's it.

Anyway, i will create a thread about all the features of the app in the next days.
```

---
## \#666 Posted by: SageTX Posted at: 2017-01-25T01:10:05.873Z Reads: 181

```
[quote="Ackmaniac, post:665, topic:12286"]
Hangover mode,
[/quote]

Ha! 😂😂😂
```

---
## \#667 Posted by: mortorojo Posted at: 2017-01-29T00:31:41.557Z Reads: 186

```
I noticed when trying to setup some modes that I dont have the ability to use decimals in Motor/Batt. Max and Motor/Batt Min.

Also, I have the bluetooth connected to my slave vesc, CAN ID 1, and when I check the "Connect by CAN to ID" to 1 to match I get nothing from the app. While when I set it ID 0, the master, values are displayed in the app, but i noticed when riding the values have intermittent pauses. When I just leave the box unchecked everything seems to work fine, values are displayed and no noticeable intermittent values.
```

---
## \#668 Posted by: Ackmaniac Posted at: 2017-01-29T18:03:08.599Z Reads: 187

```
When you connect it to the slave and want to read the values of the master then you need to enable "Connect by CAN to ID" and select the controllerid of the master. So it was correct that you selected the id 0. 
the problem when you try to get the values of the master via the slave vesc then it takes a bit longer to get the data Because the slave needs to receive the command from the Buetooth module, send the ´command to the master, receive it again from the master  and send it again to the Bluetooth module. Maybe it makes more sense to get the motor settings of the master but the realtime data of the slave itself.
```

---
## \#669 Posted by: The_Dude Posted at: 2017-01-29T22:38:04.446Z Reads: 189

```
Is this then still completely valid:
>For cruise control the 2 VESC's need to be connected via can bus and the Slave VESC needs to send the status via can and the Master VESC needs to enable "Multiple ESCs over Can"?

Or does the master now has to send his status via CAN since the slave communicates via BT?
```

---
## \#670 Posted by: Ackmaniac Posted at: 2017-01-29T22:40:13.627Z Reads: 188

```
Still the old setup.
```

---
## \#671 Posted by: Ackmaniac Posted at: 2017-02-01T19:58:35.457Z Reads: 190

```
Thanks to @The_Dude a MAC version of the Modded BLDC-Tool 2.53 is now available at the Dropbox link.

I also added a new Version of the Android App. It makes the app a bit more user friendly and small bugs are fixed. So i recommend to update to this new version. As always it will take a while until the new version is available at the Google Play store.

And it would be great if some of you can post some videos which are made by the app. I would love to see the data of a board with pneumatic wheels.
```

---
## \#672 Posted by: mmaner Posted at: 2017-02-02T00:42:28.703Z Reads: 193

```
@Ackmaniac I should have my aluminum board with skikes up by next week.  Ill get you some video of it.  Also, if you want a google drive repository I have a google business account, I'd be glad to share you a directory you can dump stuff in to.
```

---
## \#673 Posted by: onloop Posted at: 2017-02-02T00:48:18.486Z Reads: 195

```
[quote="Ackmaniac, post:671, topic:12286"]
And it would be great if some of you can post some videos which are made by the app
[/quote]

my raptor 2 vid is coming soon!
```

---
## \#674 Posted by: Eboosted Posted at: 2017-02-03T00:28:07.037Z Reads: 201

```
I'm really enjoying this firmware, I increased batt max from 30A to 35A for each VESC and it's runing super smooth, I also  dialed the throttle curve to get a better initial torque as I'm used to the very sensitive Evolve Bamboo GT remote.

<img src="/uploads/db1493/original/3X/0/5/0552d52b6d4dbf201f5bd37b728a98bdcc46e1b5.png" width="690" height="447">

I just have some small things I'd like to tune.

1. Increase braking force. I almost crashed a couple of times behind cars when they brake all of the sudden, the 100mm MBS wheels have a lot of mass and keep spinning, not easy to brake them. Would you suggest to increase batt min regen from -8A to -10A on each VESC safely without friying the VESC.

2. Increase the acceleration from a stand still. I wonder if I should increase the batt max to 40A, changing the motor a pulley from 16T to 12T should also be an option. I increased the throttle curve, it felt better but when I'm at high speed it's too jerky and I loose balance easily if I'm not pulling myself forward

3. Traction control is blocking the wheels just 10cm away from a dead stop and it throws me forward every time, is there a way to smooth the final stop?

<img src="/uploads/db1493/original/3X/e/6/e6bce89ddfa926adef926962aa6f55607f6b3379.png" width="690" height="443">

By the way I just donated a small amount to support your awesome work!
```

---
## \#675 Posted by: Ackmaniac Posted at: 2017-02-03T07:30:22.920Z Reads: 180

```
Please also post a Screenshot of your motor general, advanced and BLDC or Foc tab. And tell me which battery and motors you use (single or dual).

I think i can give you a answer to all of your problems but i need the screenshots first so that we know what we are talking about in detail.
```

---
## \#676 Posted by: Eboosted Posted at: 2017-02-04T22:58:53.082Z Reads: 201

```
Here are the screnshots:

[img]http://i.imgur.com/f8YgBaN.jpg[/img]
[img]http://i.imgur.com/RGvww1B.jpg[/img]
[img]http://i.imgur.com/Q48IoCe.jpg[/img]
[img]http://i.imgur.com/kenNPQ8.jpg[/img]

I raised the batt max to 40A on master and slave and the Max Watt to 1300W on the master and now I'm getting more torque but not in the place I need.

From 0-15kms my torque is too low
From 15-30 the board is a smoking rocket!!, all of the sudden it pulls way harder, maybe too much so I need to throw myself forward 45 degrees LOL :smile:
From 30-40Km/Hr it slowly raises the speed

I'd like to raise the torque from 0-10Km/Hr, so if not other VESC settings are possible to adjust I might go from 16T to 12T motor pulley or from 36T to 40T wheel pulley.
```

---
## \#677 Posted by: Ackmaniac Posted at: 2017-02-04T23:43:46.099Z Reads: 193

```
- You can raise the motor max to 80 and give that a try. But your Gearing is really high. It would be better to use 15 or 14 teeth. 12 teeth would be to small so that the belt would slip.
You can also try to raise the startup boost. But only raise it in 0.01 steps.

- To have more control especially at the range between 10 - 30 km/h you should lower the throttle curve.
Just try 12.5, 30, 60 for the Y acceleration values. You quickly get used to it that when you want more power you only have to pull the trigger a bit more.

- Then to have a better brake power at high speeds you can raise the battery min to -10. I prefer to might loose some cycle lifes of my battery instead of crashing into a car. But i don't think that this would harm the battery because you would use those amps only for a second or two.

- If the brake power is too weak at low speeds you should raise the motor min to maybe -80.

- To have a smoother brake close to standstill you should reduce the "Max ERPM at full Brake in current control mode" to like 500. 

- And please check your minimum and maximum pulsewidth again because they seem to be a bit far away from each other. But they also could be ok.
```

---
## \#678 Posted by: mrplaygood Posted at: 2017-02-06T08:41:48.948Z Reads: 190

```
Hello together!

I, too, use a mac and wanted to get this cool BLDC mod running on my computer. When I looked in the Dropbox link I discovered a Mac App but unfortunatly it didn't work on my laptop. After a little research I discovered the program "WineBottler" which will let you run Windows applications on a mac.
http://winebottler.kronenberg.org

I tried it and after a few updates of the current beta of WineBottler I got BLDC running.

Maybe that will help all Mac users as well as @Ackmaniac with the question about a Mac App. 

Greetings -Daniel

--SHORT UPDATE--

As you can read in the following posts, it seems that only MacOS 10.12.3 a.k.a. Sierra does not work with @The_Dude's provided Mac App.
```

---
## \#679 Posted by: The_Dude Posted at: 2017-02-06T17:48:55.389Z Reads: 182

```
Hi Daniel,

can you tell me what went wrong? I tested the installation file of the BLDC app on my MacBook and it installed fine. Unfortunately I have no other Mac to try it on another computer. May be there is any error message that helps finding the root cause.

Dude
```

---
## \#680 Posted by: Pimousse Posted at: 2017-02-06T19:05:05.422Z Reads: 179

```
I give it a try.
Thanks for the tip !
```

---
## \#681 Posted by: mrplaygood Posted at: 2017-02-06T19:32:09.478Z Reads: 182

```
Hi Dude,

unfortunatly I didn't make a screenshot but I will reinstall it and will capture the frame. And of course I will try to translate it to english ;) 

-Daniel
```

---
## \#682 Posted by: The_Dude Posted at: 2017-02-06T20:37:05.561Z Reads: 186

```
Speaking german (native) - maybe you can use the captured frame directly :stuck_out_tongue_winking_eye:
```

---
## \#683 Posted by: mrplaygood Posted at: 2017-02-06T21:18:00.952Z Reads: 177

```
Same with me ;) That's making things way easier :D
```

---
## \#684 Posted by: mrplaygood Posted at: 2017-02-07T15:24:15.905Z Reads: 198

```
Hi,

as demanded here are some screenshots of the installation process as well as of the failure:

<img src="/uploads/db1493/original/3X/6/6/66507ccdaf8395526d50367f9451621728f6cf94.png" width="690" height="243">
<img src="/uploads/db1493/original/3X/7/c/7c7144f40e190a2959e5bb8e560b4026da77cba9.png" width="690" height="396"><img src="/uploads/db1493/original/3X/5/4/54784ce68df45db37d1067b397dd65b6248f5048.png" width="690" height="488">

And here the detailed report:
> Process:               BLDC_Tool [98369]
> Path:                  /Applications/BLDC-Tool_2.53.app/Contents/MacOS/BLDC_Tool
> Identifier:            com.yourcompany.BLDC-Tool
> Version:               ???
> Code Type:             X86-64 (Native)
> Parent Process:        ??? [1]
> Responsible:           BLDC_Tool [98369]
> User ID:               501

> Date/Time:             2017-02-07 16:17:00.212 +0100
> OS Version:            Mac OS X 10.12.3 (16D32)
> Report Version:        12
> Anonymous UUID:        DC71223D-BAD1-CB7B-4986-20839E01A453

> Sleep/Wake UUID:       D17EF8F6-36D4-4518-AC4F-C380674C5030

> Time Awake Since Boot: 230000 seconds
> Time Since Wake:       21000 seconds

> System Integrity Protection: enabled

> Crashed Thread:        0

> Exception Type:        EXC_CRASH (SIGABRT)
> Exception Codes:       0x0000000000000000, 0x0000000000000000
> Exception Note:        EXC_CORPSE_NOTIFY

> Termination Reason:    DYLD, [0x1] Library missing

> Application Specific Information:
> dyld: launch, loading dependent libraries

> Dyld Error Message:
>   Library not loaded: @rpath/QtPrintSupport.framework/Versions/5/QtPrintSupport
>   Referenced from: /Applications/BLDC-Tool_2.53.app/Contents/MacOS/BLDC_Tool
>   Reason: image not found

> Binary Images:
>        0x108958000 -        0x108ab3ff7 +com.yourcompany.BLDC-Tool (???) <EB4A895F-6B5A-323F-9110-CF33D47CC3B6> /Applications/BLDC-Tool_2.53.app/Contents/MacOS/BLDC_Tool
>        0x11707e000 -        0x1170bb267  dyld (421.2) <947FC440-80F9-32F7-A773-6FC418FE1AB7> /usr/lib/dyld

> Model: MacBookPro12,1, BootROM MBP121.0167.B21, 2 processors, Intel Core i5, 2,7 GHz, 8 GB, SMC 2.28f7
> Graphics: Intel Iris Graphics 6100, Intel Iris Graphics 6100, Built-In
> Memory Module: BANK 0/DIMM0, 4 GB, DDR3, 1867 MHz, 0x80AD, 0x483943434E4E4E424C54424C41522D4E5544
> Memory Module: BANK 1/DIMM0, 4 GB, DDR3, 1867 MHz, 0x80AD, 0x483943434E4E4E424C54424C41522D4E5544
> AirPort: spairport_wireless_card_type_airport_extreme (0x14E4, 0x133), Broadcom BCM43xx 1.0 (7.21.171.68.1a5)
> Bluetooth: Version 5.0.3f1, 3 services, 27 devices, 1 incoming serial ports
> Network Service: USB 10/100/1000 LAN, Ethernet, en5
> Serial ATA Device: APPLE SSD SM0256G, 251 GB
> USB Device: USB 3.0 Bus
> USB Device: USB 10/100/1000 LAN
> USB Device: Bluetooth USB Host Controller
> Thunderbolt Bus: MacBook Pro, Apple Inc., 27.1

I think it could be that the OS isn't supported yet, because that's the normal problem I encounter with software even I have no beta OS running on my Mac.

Maybe the Log will help you @The_Dude.

Greetings -Daniel
```

---
## \#685 Posted by: The_Dude Posted at: 2017-02-07T15:29:45.816Z Reads: 171

```
[quote="mrplaygood, post:684, topic:12286"]
Mac OS X 10.12.3
[/quote]

OK - which OS X is installed on your system?
```

---
## \#686 Posted by: mrplaygood Posted at: 2017-02-07T15:32:01.598Z Reads: 163

```
MacOS Sierra
```

---
## \#687 Posted by: The_Dude Posted at: 2017-02-07T15:36:52.267Z Reads: 166

```
OK, I'm still with El Capitan (10.11). Don't now when I will upgrade, but after that I will rebuild the app and send a notification.
```

---
## \#688 Posted by: Ackmaniac Posted at: 2017-02-07T15:41:31.021Z Reads: 175

```
[quote="mrplaygood, post:684, topic:12286"]
Dyld Error Message:  Library not loaded: @rpath/QtPrintSupport.framework/Versions/5/QtPrintSupport  Referenced from: /Applications/BLDC-Tool_2.53.app/Contents/MacOS/BLDC_Tool  Reason: image not found
[/quote]

I guess the reason is that the librarys like QtPrintSupport  are missing. These libraries exist on your machine but not on others. So they need to be added in the pkg.
I had to do the same for windows.
```

---
## \#689 Posted by: mrplaygood Posted at: 2017-02-07T15:41:48.671Z Reads: 172

```
Updated my former post. Seems I was right with the OS :smiley:
```

---
## \#690 Posted by: The_Dude Posted at: 2017-02-07T20:47:57.788Z Reads: 177

```
[quote="Ackmaniac, post:688, topic:12286"]
QtPrintSupport.framework/Versions/5/
[/quote]


Hmm ... not that trivial for me, the aforementioned path does not exist on my Mac.
```

---
## \#691 Posted by: Pimousse Posted at: 2017-02-07T21:03:03.324Z Reads: 169

```
I tried with OS X Yosemite (10.10.5), it doesn't work neither. :confused:
```

---
## \#692 Posted by: The_Dude Posted at: 2017-02-07T22:04:51.684Z Reads: 167

```
Must be some missing libraries,  I will try to elaborate on that - Ackmaniac offered his support. I suppose, you have not installed Qt?
```

---
## \#693 Posted by: mrplaygood Posted at: 2017-02-07T22:14:22.886Z Reads: 167

```
I mentioned that it would be easy to use the Windows Application on a mac with winebottler....
I'm sorry but I can't get my VESC COM Port into the modded BLDC tool, even though I mapped the COM port from the mac into winebottler. Sorry to inform you but it seems much harder than I thought. 
Since I'm not a developer or programmer that's where my limits are. Maybe someone around here knows more about this problem?!

@The_Dude I just try to get my hands on qt to just try what happens if it is installed on my mac. Will reply shortly after I tried.
```

---
## \#694 Posted by: mrplaygood Posted at: 2017-02-07T22:47:19.554Z Reads: 166

```
Hi, 

I just installed QT and have no clue if I have to do any more things afterwards. :D 
I tried to start the modded app but still no success.
```

---
## \#695 Posted by: Eboosted Posted at: 2017-02-08T06:43:44.874Z Reads: 171

```
Hey man! thanks for the tips. I just updated the suggested settings, will test tomorrow morning and I report back.

I increased start up boost from 0.01 to 0.02, it says increase ir carefully, does it add more current from stand still only? or it keeps adding until you reach certain speed?
```

---
## \#696 Posted by: The_Dude Posted at: 2017-02-08T08:13:01.382Z Reads: 176

```
I used brew to install. What did you use? Which version of Qt?
Anyway, I will try to get it working but it seems to me that it's not trivial. Qt is somehow hardcoding a library path which does not exist on my Mac ... we'll see.
```

---
## \#697 Posted by: Eboosted Posted at: 2017-02-09T01:17:06.822Z Reads: 195

```
@ackmaniac I have a friend with the same setup as me, 2 VESC, 2 6355 190KV motors, 100mm wheels, 10S4P with Samsung 25R, but instead of 16/36T he has 13T/36T pulley kit.

Whenever the battery charge is between 90-100%, if he applies brakes on high speed, regen sends amps to the battery until it overcharges more than 57V and throws an overvoltage fault code:

Fault            : FAULT_CODE_OVER_VOLTAGE
Current          : -14.2
Current filtered : -14.3
Voltage          : 57.35
Duty             : 0.27
RPM              : 21833.1
Tacho            : 453339
Cycles running   : 10841
TIM duty         : 3498
TIM val samp     : 1748
TIM current samp : 8175
TIM top          : 12854
Comm step        : 5
Temperature      : 48.62

Fault            : FAULT_CODE_OVER_VOLTAGE
Current          : -20.3
Current filtered : -15.9
Voltage          : 57.41
Duty             : 0.20
RPM              : 17775.2
Tacho            : 464138
Cycles running   : 4798
TIM duty         : 3221
TIM val samp     : 1610
TIM current samp : 9744
TIM top          : 16268
Comm step        : 2
Temperature      : 46.49

Fault            : FAULT_CODE_OVER_VOLTAGE
Current          : -11.4
Current filtered : -11.5
Voltage          : 57.45
Duty             : 0.23
RPM              : 17776.1
Tacho            : 486449
Cycles running   : 6651
TIM duty         : 3358
TIM val samp     : 1677
TIM current samp : 8969
TIM top          : 14583
Comm step        : 3
Temperature      : 47.65

Fault            : FAULT_CODE_OVER_VOLTAGE
Current          : -23.3
Current filtered : -16.5
Voltage          : 57.63
Duty             : 0.14
RPM              : 14073.5
Tacho            : 505408
Cycles running   : 4414
TIM duty         : 2848
TIM val samp     : 1426
TIM current samp : 11865
TIM top          : 20877
Comm step        : 2
Temperature      : 48.48

Fault            : FAULT_CODE_OVER_VOLTAGE
Current          : -34.5
Current filtered : -22.3
Voltage          : 57.68
Duty             : 0.10
RPM              : 11553.5
Tacho            : 522941
Cycles running   : 3915
TIM duty         : 2513
TIM val samp     : 1264
TIM current samp : 13767
TIM top          : 25007
Comm step        : 1
Temperature      : 51.99

and VESC reboots itself, I'm guessing if the battery is fully charged at 42V there's no place for the regen current to go, so system crashes, he looses all remote control and brakes, really scary to ride this way.

I the battery is below 90% the board rides perfect and braking works flawlessly

[img]http://i.imgur.com/f8YgBaN.jpg[/img]

We tried:

1. Reducing the Batt Min (regen) from -8.00 to -5.00A (same problem, overcharge, less braking)
2. Reducing the batt Min (regen) to -2.00A (no cutting out, but almost no brakes)
3. Increasing Maximum Input Voltage from 57V to 58V (same problem, overcharge, voltage spike now 58.7V instead of 57.6V)

I'm pretty sure it must have something to do with the pulley kit 13T/36T as it spins the motor a lot more and charges will too much current.
```

---
## \#698 Posted by: Ackmaniac Posted at: 2017-02-09T07:24:44.311Z Reads: 169

```
I guess he has another BMS or you have no BMS and he has one. Sounds to me that his BMS shuts down and the VESC doesn't know where to put that power.
```

---
## \#699 Posted by: Pedrodemio Posted at: 2017-02-09T12:43:11.999Z Reads: 169

```
As @Ackmaniac said, probably the BMS is detecting an overcharge of the battery
The easy way to figure it out is bypass the charge and use it only for charging
```

---
## \#700 Posted by: Eboosted Posted at: 2017-02-09T14:39:41.966Z Reads: 167

```
Both boards, mine and his, have the Battery Supports 10S 60A BMS. VESC doesn't know where to put that regen power
```

---
## \#701 Posted by: Eboosted Posted at: 2017-02-09T15:41:26.720Z Reads: 166

```
@Pedrodemio if BMS would be detecting a battery overcharge then why would the VESC detect a overcharge and store the fault?, if VESC cutsoff 5 times there would be 5 overcharge stored faults.

Would this have anything to do with the fact I have 100mm wheels, 13T/36T pulley ratio?

Same braking speed, very big wheel diameter, very small motor pulley, a lot of rpms on the motor pulley side during braking, a lot of current being produced by the motor and flowing back to the battery = VESC cutsoff and reboots.
```

---
## \#702 Posted by: Ackmaniac Posted at: 2017-02-09T16:00:42.336Z Reads: 164

```
When the BMS detects a overcharge it shuts off. So where should the VESC send the power now? If you would have 12S battery it might can reach the 57V if you have very very bad batterys. But with a 10S you should not face that issue. So i think it's the BMS. 
And if the Motor spins faster with the lower motor gear it also produces a higher current. But still it shouldn't be a issue for a 10S Battery. Just try to bypass the BMS and i think the problem will be solved.
```

---
## \#703 Posted by: Eboosted Posted at: 2017-02-09T16:04:44.880Z Reads: 158

```
Thanks Nico, I'll try to do that tonight and report back the results
```

---
## \#704 Posted by: Pedrodemio Posted at: 2017-02-09T16:53:12.651Z Reads: 164

```
Exactly what @Ackmaniac said, the BMS cut the conection  between  the VESC and battery, but there still a current wanting to flow, all energy goes into the capacitors and the voltage rise quickly since they can't store much charge, triggering the cut off.

I would say to stop riding in this condition, if the conditions are right (or wrong in this case) the VESC may react to slow to the rising voltage and something might blow
```

---
## \#705 Posted by: Ackmaniac Posted at: 2017-02-09T20:12:43.346Z Reads: 159

```
@The_Dude was so nice and provided a new Version for MAC. Thanks again, much appreciated.

I added it already to the Dropbox link. Hopefully the problems are now fixed for all operating systems.
```

---
## \#706 Posted by: DavidC Posted at: 2017-02-09T20:24:13.049Z Reads: 160

```
This new version doesn't work with macOS Sierra 10.12.3 for me.

"BLDC-Tool_2.53 cannot be opened because of a problem."
```

---
## \#707 Posted by: Pimousse Posted at: 2017-02-09T20:29:23.674Z Reads: 161

```
Works for me now (Yosemite 10.10.5).
Thank you very much @The_Dude !!!
```

---
## \#708 Posted by: The_Dude Posted at: 2017-02-09T20:34:15.369Z Reads: 165

```
Strange - I also gave it to @mrplaygood and it worked for him. As far as i know, he's also with OSX Sierra. I will see, if I can get access to a Mac with Sierra to check.
```

---
## \#709 Posted by: Ackmaniac Posted at: 2017-02-09T20:35:47.602Z Reads: 166

```
Can you post a screenshot of the error? That would help.
```

---
## \#710 Posted by: Maxid Posted at: 2017-02-09T20:49:02.522Z Reads: 163

```
Wasn't there some issue with newer Macs that you have to allow "sideloaded" applications. Maybe that's the case...
```

---
## \#711 Posted by: DavidC Posted at: 2017-02-09T21:11:02.843Z Reads: 170

```
Of course :

Process:               BLDC_Tool [2017]
Path:                  /Applications/BLDC-Tool_2.53.app/Contents/MacOS/BLDC_Tool
Identifier:            com.yourcompany.BLDC-Tool
Version:               ???
Code Type:             X86-64 (Native)
Parent Process:        ??? [1]
Responsible:           BLDC_Tool [2017]
User ID:               501

Date/Time:             2017-02-09 22:09:42.438 +0100
OS Version:            Mac OS X 10.12.3 (16D32)
Report Version:        12
Anonymous UUID:        AFABF4B5-5A46-F9CE-8C3B-576757210306

Sleep/Wake UUID:       15F18420-A086-4009-A58B-314C4EC275DB

Time Awake Since Boot: 7700 seconds
Time Since Wake:       39 seconds

System Integrity Protection: enabled

Crashed Thread:        0

Exception Type:        EXC_CRASH (SIGABRT)
Exception Codes:       0x0000000000000000, 0x0000000000000000
Exception Note:        EXC_CORPSE_NOTIFY

Termination Reason:    DYLD, [0x1] Library missing

Application Specific Information:
dyld: launch, loading dependent libraries

Dyld Error Message:
  Library not loaded: @rpath/QtPrintSupport.framework/Versions/5/QtPrintSupport
  Referenced from: /Applications/BLDC-Tool_2.53.app/Contents/MacOS/BLDC_Tool
  Reason: image not found

Binary Images:
       0x10a736000 -        0x10a891ff7 +com.yourcompany.BLDC-Tool (???) <EB4A895F-6B5A-323F-9110-CF33D47CC3B6> /Applications/BLDC-Tool_2.53.app/Contents/MacOS/BLDC_Tool
       0x10e133000 -        0x10e170267  dyld (421.2) <947FC440-80F9-32F7-A773-6FC418FE1AB7> /usr/lib/dyld

Model: iMac13,2, BootROM IM131.010A.B0A, 4 processors, Intel Core i7, 3,4 GHz, 16 GB, SMC 2.11f14
Graphics: NVIDIA GeForce GTX 680MX, NVIDIA GeForce GTX 680MX, PCIe, 2048 MB
Memory Module: BANK 0/DIMM0, 8 GB, DDR3, 1600 MHz, 0x80AD, 0x484D5434314753364D465238432D50422020
Memory Module: BANK 1/DIMM0, 8 GB, DDR3, 1600 MHz, 0x80AD, 0x484D5434314753364D465238432D50422020
```

---
## \#712 Posted by: DavidC Posted at: 2017-02-09T21:12:33.794Z Reads: 164

```
<img src="/uploads/db1493/original/3X/4/3/435597d25b9a699f3cde9d9bdab6a118e0e718f8.jpeg" width="420" height="234">
```

---
## \#713 Posted by: mrplaygood Posted at: 2017-02-09T21:13:24.047Z Reads: 163

```
Hi, 
I tried @The_Dude s software on Mac OSX Sierra 10.12.3 and it worked fine. I had not installed QT which he said could solve the problem but I have installed Xcode. If you don't want to install this because it is about 5 GB you can also install the Xcode command line tools which are free and much smaller. I hope that helps.
```

---
## \#714 Posted by: DavidC Posted at: 2017-02-09T21:18:35.137Z Reads: 160

```
I have all updates done, but I have Xcode Version 8.0 (8A218a).

I'm downloading Version 8.2.1 to see if it helps.


The problem is : "dyld: Library not loaded: @rpath/QtPrintSupport.framework/Versions/5/QtPrintSupport"
```

---
## \#715 Posted by: The_Dude Posted at: 2017-02-09T22:07:43.063Z Reads: 161

```
What is the size of your pkg-file you downloaded and used for the installation?
```

---
## \#716 Posted by: DavidC Posted at: 2017-02-09T22:09:50.414Z Reads: 164

```
It's 852 858 bytes.

Updating Xcode didn't help.

I'm installing QT now… Maybe that was the problem? :blush:
```

---
## \#717 Posted by: The_Dude Posted at: 2017-02-09T22:14:34.222Z Reads: 159

```
You really downloaded the latest version? The size should be around 10 MB or more. The error you encounter was exactly the error of the version before ...
```

---
## \#718 Posted by: Ackmaniac Posted at: 2017-02-09T22:19:00.007Z Reads: 164

```
Yes the new version is 10 MB and the old version was around 900 kb. So it seems that you have the old version. Please look again at the Dropbox link and download the actual version. Could be that Dropbox needed a couple of minutes to Update the new files.
```

---
## \#719 Posted by: DavidC Posted at: 2017-02-09T22:20:20.154Z Reads: 166

```
You're right I downloaded the same way the real new version and it works!

That's weird when I downloaded it first it shown on Dropbox as it was modified 18 minutes ago but actually it was the old version…

Thank you very much! :grinning:
```

---
## \#720 Posted by: The_Dude Posted at: 2017-02-09T22:24:52.044Z Reads: 173

```
Great, have fun :sunglasses:
```

---
## \#721 Posted by: Riako Posted at: 2017-02-09T23:33:29.828Z Reads: 177

```
I there, 
just a quick message to thanks loudly Ackmaniac !!!! Pimousse told us sooooo much good feedback with it, I'm now in FW 2.53 HW4.10 (no custom throttle curve actualy, wanna test it like that and enjoy the changement of the dual first, then watt and custom throttle curve and maybe cruise controle on CH3?! And test all in session by android ... It's like a dream !).
Many thanks for all waht have done Ackmaniac !!!
If we could help in any report or other think please feel free to ask
(I'm with a GT2B MadMunkey custom by Pimousse with CH3 channel, running 10s5ah20c lipo, dual VESC via canbus and 2 APS 6355 190kv motor)
little unusefull video :blush: 
https://youtu.be/UbA4eIqj1Wc
```

---
## \#722 Posted by: Ackmaniac Posted at: 2017-02-10T08:40:46.500Z Reads: 186

```
Great to see that more and more people are using the mod. 
You can do me a favor. You can check which pulsewidth signal (PPM) you get at channel 3 when the  button is pressed and not pressed.

And do yourself a favor and try the throttle curve with these settings. Makes the throttle much smoother without loosing power.

<img src="/uploads/db1493/original/3X/8/e/8e87deae62bd1393d9f496c21337e61c12cf681b.png" width="686" height="499">
```

---
## \#723 Posted by: Riako Posted at: 2017-02-10T09:23:32.020Z Reads: 169

```
Many thanks Ack ! I will do maybe tomorow during a test ride :smile: !!!
(the CH3 is not connected yet, and it's a switch like the on/off button of the remote but it should work with some practice :blush: ).

Once again, a big thanks to you ! I'll let you know.
```

---
## \#724 Posted by: Pimousse Posted at: 2017-02-10T10:11:35.497Z Reads: 169

```
When CH3 on : around 2 ms
when CH3 off : around 1ms

I checked it on BLDC Tool while checking the mad munkey mods I made recently.
(checked maybe 5 remotes, all act the same)
```

---
## \#725 Posted by: Ackmaniac Posted at: 2017-02-10T10:16:19.311Z Reads: 168

```
That is great to hear. Then you can use channel 3 for cruise control. Just set the center to the value when it is off (1.00 ms pulsewidth). And max to 2.00 and min to 0.00 pulsewidth for example and then you should have a software cruise control via the slave VESC.
```

---
## \#726 Posted by: Surfer Posted at: 2017-02-10T11:30:18.022Z Reads: 167

```
Yes!! You are The-Dude!!! Now is working fine in Sierra, thanks a lot.
```

---
## \#727 Posted by: PXSS Posted at: 2017-02-10T13:33:39.745Z Reads: 162

```
I wish there was a way to record onboard, i do not have an android phone :frowning:
```

---
## \#728 Posted by: Eboosted Posted at: 2017-02-10T16:10:26.566Z Reads: 165

```
I used this throttle curve and now I have a lot of throttle range, I just need to pull more if I want to have more power, I also increased the start up boost and it feels more alive from launch from stand stills.

I'm loving this FW.

I wonder what could have changed by increasing te FW from 199KB to 10MB? it's 9.8MB more!
```

---
## \#729 Posted by: Ackmaniac Posted at: 2017-02-10T16:20:25.206Z Reads: 165

```
No no, the firmware file is still around 200kb. Only the BLDC tool is around 10MB for the Mac because of the libarys which are needed. To write 10 MB of source code you would need a couple of years.
```

---
## \#730 Posted by: Randyc1 Posted at: 2017-02-10T16:29:26.359Z Reads: 169

```
Just read the "intro" to this thread ,...why can you only get 50% throttle at high speeds ?

Is an additional hardware needed to get this appt working  ?
```

---
## \#731 Posted by: SeanHacker Posted at: 2017-02-10T18:30:11.233Z Reads: 174

```
@Ackmaniac How exactly do I go about using channel 3 button on my mad munkey (gt2b) controller? Do I need to make a Y splitter for the receiver cable to plug into channel 3 on the receiver in order to use the channel 3 button for cruise control?
```

---
## \#732 Posted by: Ackmaniac Posted at: 2017-02-10T20:36:26.832Z Reads: 172

```
You use a new servo cable that goes from the receivers channel 3 to the Slave VESC. So it only works when you have the Master and the Slave connected via CAN.
```

---
## \#733 Posted by: SeanHacker Posted at: 2017-02-10T23:57:04.986Z Reads: 175

```
Alright. Got it. Now how do I set it up in BLDC_Tool? And then how do I use it on my remote controller? I'm totally new to the cruise control option. 

<img src="/uploads/db1493/original/3X/5/0/505ec779efb6f89c335659026b8c14623d1e725c.jpg" width="392" height="499">
```

---
## \#734 Posted by: Eboosted Posted at: 2017-02-11T06:10:20.448Z Reads: 165

```
What setting are replicated in slave VESC when you set them on master?

If you set the max watt in master there's no need to set it on slave, each motor and hall sensorssettibgs must be done individually. 

What about Batt max, batt min (regen), motor am,  should I set them on the master and slave individually?
```

---
## \#735 Posted by: Pimousse Posted at: 2017-02-11T06:40:23.409Z Reads: 158

```
Set your VESC as independant ESC.
The CAN bus communication is roughly used for communicating the PPM signal from the maqter to the slave.
```

---
## \#736 Posted by: Ackmaniac Posted at: 2017-02-11T11:00:18.183Z Reads: 161

```
The motor max min,  battery max min needs to be set on both. But the max watts is only needed on the master. The master doesn't share the ppm signal. It tells the slave which current to use. And the max watts is needed at the master to calculate the current and then sends it to the slave. The motor and battery settings are the limits for each vesc individually. That means when you tell the slave to use 1000 amps it would still only go as high as its limits allows it.
```

---
## \#737 Posted by: Pimousse Posted at: 2017-02-11T17:10:05.827Z Reads: 165

```
A little precision about CH3 :

PPM when CH3 on : 1.06 ms
PPM when CH3 off : 2.06 ms

:wink:

EDIT : @Ackmaniac I just updated the FW to 2.53 and now the PPM displays shows nothing in the ms counter.
I didn't touch anything in the hardware, just updated the FW...
What did I miss ?
```

---
## \#738 Posted by: Ackmaniac Posted at: 2017-02-11T17:56:04.652Z Reads: 173

```
You have to activate PPM in the Application General Tab on the Slave VESC and then Reboot.
After that chose "Cruise Control via Secondary Channel" as Control Mode and Enable the Display Checkbox to see the signal.

Then Choose the Pulsewith signal that is shown when it is off as Center Pulsewidth.
Then Choose the Pulsewidth signal that is shown when it is on as minimum Pulsewidth.
Then enter as maximum pulsewidth the difference between the both and calculate center + difference.

So in your case
min = 1.06
center = 2.06
max = 3.06

This way it should work.
```

---
## \#739 Posted by: Pimousse Posted at: 2017-02-11T17:57:56.120Z Reads: 168

```
I use a single setup.
Again, all was fine before I update (from 2.52).
No hardware issue (didn't touch anything,  receiver's led is solid red)
```

---
## \#740 Posted by: Ackmaniac Posted at: 2017-02-11T18:00:43.727Z Reads: 174

```
With a single you can't use cuise control. Could it be that you connected to the wrong channel after you tested channel 3. The correct channel for the trigger is number 2 for the GT2B.
And there is absolutely no difference between 2.52 and 2.53 to identify the Pulsewidth. So it must be another issue.
```

---
## \#741 Posted by: Pimousse Posted at: 2017-02-11T18:05:25.201Z Reads: 178

```
I'm not using cruise control.
I'm talking about the PPM display in the App configuration -> PPM tab.
It stays at 0 ms.

I double-cheked the receiver wiring, it's ok.
I'll test another remote.
```

---
## \#742 Posted by: Ackmaniac Posted at: 2017-02-11T18:06:40.066Z Reads: 176

```
Are you sure that you got VCC and ground connected to the correct pins? And did you make sure that you selected PPM in the applications General Tab.
```

---
## \#743 Posted by: Ackmaniac Posted at: 2017-02-11T18:07:28.318Z Reads: 178

```
After you selected PPM or PPM and UART you have to reboot the VESC.
<img src="/uploads/db1493/original/3X/a/5/a526653ef0ff1f3f9e12dcf724d73c3cc7380027.png" width="690" height="492">
```

---
## \#744 Posted by: Pimousse Posted at: 2017-02-11T18:08:48.925Z Reads: 169

```
PPM + UART, yes.
And I'm sure about the wiring.
I checked another remote, same issue. :unamused:

EDIT : re-flashed and reboot. It works now...
Very strange.
Something I mentioned with the linux version but same for mac version : the app crashes when rebooting through the app.
```

---
## \#745 Posted by: Pedrodemio Posted at: 2017-02-11T20:16:58.890Z Reads: 165

```
@Ackmaniac could your firmware have some sort of bug that's affecting the brake?

my VESC was in firmware 2.10 an I've been using it for more than a year  in BLDC with no drops, no faults, nothing

I've uploaded yours 2.53 and went straight to FOC, everything ok but on the first test ride i have the same problem of the first FOC version, suddenly loss of braking and a very high pitched ugly noise on startup

Back to BLDC, fresh installation, everything the same as i ever had, detection as always went ok

First test ride and i'm losing brake on BLDC to, unfortunately Jacob's site is offline and there is no way for me to get the unmoded firmware

Our friend a few posts above was having this problem and you and me pointed to the BMS, unfortunately i don't use one to blame

EDIT: didn't know that i could roll back, going back to 2.10 and will report back in a few minutes
```

---
## \#746 Posted by: Pedrodemio Posted at: 2017-02-11T20:33:54.723Z Reads: 164

```
Ok, there is  definitely something going on, i will start a new thread

No problems on 2.10, 5 minutes of braking and accelerating and no problems
```

---
## \#747 Posted by: Deakbannok Posted at: 2017-02-11T22:07:35.539Z Reads: 167

```
I did have to same problem; I couldnt get my remote Nano-X to work VESC-X after flashed firmware 2.53
On VESC-X there is no flashing green LED when I pushed control. No fault code on BLDC
So I flashed back to 2.18; now is working normal
```

---
## \#748 Posted by: Ackmaniac Posted at: 2017-02-11T22:15:29.905Z Reads: 170

```
Can you please check the Voltage in the Realtime Tab of the BLDC-Tool and then check your battery with multimeter. And what is your maximum input voltage in the settings.
```

---
## \#749 Posted by: Ackmaniac Posted at: 2017-02-11T22:17:41.236Z Reads: 165

```
@Deakbannok Did you setup your PPM settings after flashing to Version 2.53?
```

---
## \#750 Posted by: Deakbannok Posted at: 2017-02-11T22:26:29.321Z Reads: 167

```
Yes. I did rechecked everything after I flashed 2.53; I did with a soft reboot and reset power.
my voltage on the multimeter is the same as it showed on BLDC.
I just uninstalled the BLDC  and reflash back to 2.18. Now is working normal
```

---
## \#751 Posted by: Ackmaniac Posted at: 2017-02-11T22:27:52.605Z Reads: 171

```
I mean did you setup the pulsewidth settings in the PPM Tab?
```

---
## \#752 Posted by: Deakbannok Posted at: 2017-02-11T22:31:56.283Z Reads: 169

```
Yes. But
The green LED dim light on VESC-X is not bright when I pushed to controller.
```

---
## \#753 Posted by: Ackmaniac Posted at: 2017-02-11T22:39:54.503Z Reads: 173

```
And do you know that there is a center pulsewidth parameter now. Because there isn't really anything i can think of that would lead to a non functioning remote. So if you want to give it another try it would be great when you set the controller to disabled. And then send screenshots with the display enabled at full brake, idle and full acceleration.
The only thing i can thing if is the Safe start option which doesn't give power as long as the VESC is not in idle or brake for a short moment. This is to prevent that the board moves when you switch it on with the wrong settings.
We can have a Skype session of you want to check together what could be wrong.
There are also many others without any issues. And i also have a 4.10 HW version beside my 4.12 and it is working without issues.
```

---
## \#754 Posted by: Ackmaniac Posted at: 2017-02-11T22:53:08.839Z Reads: 172

```
And when you switch from a older version you should not use your safed xml files. You should do all the configuration again from scratch. And maybe the BLDC-Tool for 2.10 was working different. I never worked with that one. And a screenshot of your settings would also be very helpful to analyse if there are any mistakes.
```

---
## \#755 Posted by: E-Boarding Posted at: 2017-02-12T12:05:18.935Z Reads: 169

```
I've a Galaxy Ace2 with CyanogenMod (Android 5.1) VESC-Monitor 1.3
When I use the Video-Capture, the Phone freezes :frowning: Is there anything I can do about it, I already set video options to minium, maybe this phone is too weak or something?
the generated mp4-files are corrupted
```

---
## \#756 Posted by: Ackmaniac Posted at: 2017-02-12T12:13:34.154Z Reads: 171

```
First you should get the latest Version of the app. 
After that in the app there is a Galleries Icon. When you press it you see a explorer view. Just go there in the folder where you want your files to be stored. Then Press the Disk Icon on the upper right. That makes this folder the default folder for the files to be stored.

If you get a error message please try to get the details about it or send it.
```

---
## \#757 Posted by: Deakbannok Posted at: 2017-02-12T15:57:02.209Z Reads: 170

```
I will give it a try again this week and will keep you update.
```

---
## \#758 Posted by: jul88 Posted at: 2017-02-12T21:23:38.357Z Reads: 181

```
Hello,
can we use cruise control with this remote ??
[https://fr.aliexpress.com/item/Wholesale-New-arrival-2-4Ghz-mini-remote-controller-with-receiver-for-electric-skateboard-longboard/32678995218.html?isOrig=true#extend](https://fr.aliexpress.com/item/Wholesale-New-arrival-2-4Ghz-mini-remote-controller-with-receiver-for-electric-skateboard-longboard/32678995218.html?isOrig=true#extend)
<img src="/uploads/db1493/original/3X/5/3/53702294b2e3497632465704ec77776b75ff243a.png" width="618" height="500">
```

---
## \#759 Posted by: Ackmaniac Posted at: 2017-02-12T22:01:57.081Z Reads: 177

```
I don't think that it works. If you would modify the switch to a button which you can press and automatically switches off when you release it then it would work. But the other question is also what signal you get. For example if the output is 5V then it would be to much for the VESC. But with some voltage dividers it could be modified then.
I recommend the Mini Remote for cruise control. Works great.
```

---
## \#760 Posted by: Ackmaniac Posted at: 2017-02-12T22:16:31.428Z Reads: 174

```
I made a little update of my App. It is possible now to make the Data Visualisation a little bit transparent in the Video mode. Just go to the Video settings and enable it if you want.
This way you still can see a bit of the rest of the video. Tell me how you like it and if you have better ideas then let me know.
```

---
## \#761 Posted by: Msk8 Posted at: 2017-02-13T07:02:19.808Z Reads: 202

```
Thank you Ackmaniac for this fantastic watt control mod and these awesome throttle curves. I recently added a 2nd SK3 6364 to deal with some hills here but the fun on flats totally suffered, it's a beast and the power and acceleration was just scary. Now with your mod it's fun again! :) I played around quite a bit with the breaking, that was even more scary before your update with a 2nd motor even though I cut the breaking amps way down to 6A per VESC. Now i like the breaks again. Here are the throttle setting that worked best for me so far. <img src="/uploads/db1493/original/3X/b/2/b2ed88e9367858474134774ebe366caf231d0e0b.PNG" width="690" height="441">
```

---
## \#762 Posted by: Duffman Posted at: 2017-02-13T11:13:40.557Z Reads: 209

```
After a lot of rebuilding, improving and bad weather I finally had the chance to do some logging.
Still with modded FW2.18. Need more tests on the small board before I upgrade the monster to FW2.53.

peak power was around 7,8kW (176A battery - logfile)
peak motor current was around 435A (blocked - video)

Setup:
120A motor max / 60A battery max
12s30Ah
4x VESC 4.7 with 0,005mOhm Shunts, extra caps, extra TVS diodes and heatsinks
4x c6364 with embedded sensors

Video with datalog overlay:
https://www.youtube.com/watch?v=UxpQMWbrWwg

VESC Log Data File (.csv):
https://www.dropbox.com/sh/3v9isv7oir3drv4/AABBeF_1eScl1Pzq1g2giRTja?dl=0

for VESC DataLogAnalyzer:
http://www.gct-hp.de/VDLA/
```

---
## \#763 Posted by: Ackmaniac Posted at: 2017-02-13T11:25:43.933Z Reads: 191

```
F****** awesome to see my app on that monster. 
The power consumption is crazy. 72 Wh a km on average. I would call that a record. But you still see that the average current is low in the active and riding Tab.
But something doesn't work properly with the original firmware. Because you only get one Reatime data update a second. Normally it is 8 till 9 a second so it would give much more data. But i will test this evening with the original 2.18 firmware to find that bug and then the information would be much more fluent and much more detailed.
```

---
## \#764 Posted by: Duffman Posted at: 2017-02-13T11:35:22.526Z Reads: 188

```
Jepp, I also noticed the low sampling rate, will make further tests... More time resolution would be great!

Another record is 800W of friction losses when freewheeling (end of the video). Have to blame my 'gamma ring' sealed gearboxes for that.

Also sometimes it seemed that the logfile was written while the video was recorded and sometimes not, will try to take a closer look next time.
```

---
## \#765 Posted by: Ackmaniac Posted at: 2017-02-13T11:37:29.896Z Reads: 179

```
Found the bug already but need a little while to fix it.
The log file is always written when the board moved once. SO it doesn't matter if you take a video or not. Only when the board doesn't move (for example to check the battery voltage) then the log file get's deleted automatically.
```

---
## \#766 Posted by: Duffman Posted at: 2017-02-13T12:03:26.457Z Reads: 180

```
Ok, this makes sense. I wondered over the strange logfile behavior while benchtesting.

Is there a technical reason why your app only supports newer android versions. Would have been great to take my old mobile out for skating...
```

---
## \#767 Posted by: Ackmaniac Posted at: 2017-02-13T15:31:54.012Z Reads: 179

```
To record your actual screen you need at least Android 5.0. Before it was only allowed to record the camera by the Android policies.
```

---
## \#768 Posted by: Ackmaniac Posted at: 2017-02-13T19:30:46.703Z Reads: 178

```
I fixed the Issues for the firmware version 2.18. Should work without issues now. 
Of course you can only watch the data and not change the mode because you need my firmware mod for this.

Google play needs a while for the upload but you find the file also at my dropbox account.
```

---
## \#769 Posted by: ekitesurfer Posted at: 2017-02-14T07:04:55.379Z Reads: 179

```
I would like to try this app, but I cant figure out how to download it properly... I have ubuntu 14.04, when I click on bldc tool in the downloaded file it doesn't do anything....
```

---
## \#770 Posted by: Ackmaniac Posted at: 2017-02-14T07:24:01.695Z Reads: 176

```
@ekitesurfer You have to do it the same way as for vedders firmware. Only difference is that you use my bldc-tool mod and firmware mod instead of his. 

http://vedder.se/2015/01/vesc-open-source-esc/
```

---
## \#771 Posted by: ekitesurfer Posted at: 2017-02-14T08:13:23.953Z Reads: 177

```
I do not understand how to use yours instead of his.....
```

---
## \#772 Posted by: Duffman Posted at: 2017-02-14T08:18:50.749Z Reads: 177

```
I had the same problem, when I tried to start the downloaded BLDC Tool via double click.

You have to do a right click on the file, choose 'Properties' go to the 'Permissions' tab and activate the checkbox 'Allow executing file as program'.

That solved the problem for me.
```

---
## \#773 Posted by: ekitesurfer Posted at: 2017-02-14T08:21:15.662Z Reads: 175

```
already tried that, doesn't do anything for me...
```

---
## \#774 Posted by: Ackmaniac Posted at: 2017-02-14T08:30:18.081Z Reads: 168

```
Just go into the folder with the terminal and run "make". After that it should be runnable.
```

---
## \#775 Posted by: Duffman Posted at: 2017-02-14T08:31:00.385Z Reads: 166

```
Maybe a stupid question but did you 'click on bldc tool in the downloaded file' or did you unzip the archive (BLDC-tool_ACKMANIAC_Mod_Ubuntu_2_53.zip) in a new folder and clicked on the BLDC-Tool file?
```

---
## \#776 Posted by: ekitesurfer Posted at: 2017-02-14T08:39:45.895Z Reads: 164

```
Folder with a terminal? This Ubuntu stuff is beyond me...
```

---
## \#777 Posted by: ekitesurfer Posted at: 2017-02-14T08:42:47.586Z Reads: 165

```
unzipped...
```

---
## \#778 Posted by: Ackmaniac Posted at: 2017-02-14T09:58:56.470Z Reads: 163

```
After unzipping

[quote="Duffman, post:772, topic:12286"]
You have to do a right click on the file, choose 'Properties' go to the 'Permissions' tab and activate the checkbox 'Allow executing file as program'.
[/quote]
```

---
## \#779 Posted by: ekitesurfer Posted at: 2017-02-14T10:35:43.798Z Reads: 160

```
I downloaded your file. I "extracted" it, I assume this mean "unzipping"? I right clicked on the bldc tool icon, did the permissions thing and it does nothing when I double click it....
```

---
## \#780 Posted by: Ackmaniac Posted at: 2017-02-14T11:19:56.796Z Reads: 164

```
Then go into the unzipped folder in the terminal (shell) and type "make" without the high quotes. If you get an error then post it here. If it works without issues then double click the bldc-tool file and you should be good to go.
```

---
## \#781 Posted by: ekitesurfer Posted at: 2017-02-14T11:38:23.588Z Reads: 171

```
I clicked on the unzipped folder and do not see anything that I can type "make" into....
```

---
## \#782 Posted by: Ackmaniac Posted at: 2017-02-14T11:42:41.690Z Reads: 169

```
Do you have a windows PC or MAC?
```

---
## \#783 Posted by: ekitesurfer Posted at: 2017-02-14T11:43:16.087Z Reads: 165

```
pc running ubuntu 14.04
```

---
## \#784 Posted by: Ackmaniac Posted at: 2017-02-14T11:43:58.503Z Reads: 169

```
You know what a terminal or shell is in Ubuntu? The window where you can type in commands.
```

---
## \#785 Posted by: ekitesurfer Posted at: 2017-02-14T11:45:01.151Z Reads: 174

```
yes sir
 10 char
```

---
## \#786 Posted by: Ackmaniac Posted at: 2017-02-14T11:45:36.145Z Reads: 175

```
Then go there, select the folder where you unzipped the files and type 
make
```

---
## \#787 Posted by: ekitesurfer Posted at: 2017-02-14T11:49:02.987Z Reads: 169

```
The terminal is a black screen. How do I select the folder in the terminal?
```

---
## \#788 Posted by: Ackmaniac Posted at: 2017-02-14T11:50:39.720Z Reads: 171

```
read this (google is your friend)
http://www.computerhope.com/unix/ucd.htm
```

---
## \#789 Posted by: ekitesurfer Posted at: 2017-02-14T12:02:02.192Z Reads: 176

```
This shit is way beyond my skill level. My brain does not want to learn all this computer crap. I can copy and paste, but beyond that reading all that computer garble gives me a headache. I would like to try your app, but unless someone can walk me through this, I give up
```

---
## \#790 Posted by: Ackmaniac Posted at: 2017-02-14T12:07:09.639Z Reads: 174

```
Have a look at that video. 
https://www.youtube.com/watch?v=z-qMFwLMrLc
```

---
## \#791 Posted by: Maxid Posted at: 2017-02-14T12:11:04.592Z Reads: 171

```
Why are you using ubuntu then? How can one be a Linux user and not want to deal with terminals and the basic commands? You do realize there is a Windows and Mac version out there that does not require fiddling with a terminal window.
```

---
## \#792 Posted by: ekitesurfer Posted at: 2017-02-14T12:14:56.424Z Reads: 175

```
Because when I got into this esk8 stuff, the windows bldc app was not available. I was able to follow Vedder's video and copy and paste my way into success. I found that I like Ubuntu, but only when I can copy and paste easily understandable instructions, like Vedder has....
```

---
## \#793 Posted by: Maxid Posted at: 2017-02-14T12:16:42.407Z Reads: 173

```
But you do have a windows PC or Mac don't you? So why not switch now?
```

---
## \#794 Posted by: ekitesurfer Posted at: 2017-02-14T12:18:54.631Z Reads: 170

```
I kinda like Ubuntu, don't want to change. I just want some easy instructions on how to open this app...
```

---
## \#795 Posted by: Ackmaniac Posted at: 2017-02-14T12:26:41.765Z Reads: 173

```
Then you need to study at least how the cd command (**c**hange **d**irectory ) works. It's described in the video i posted. Because you need to select the extracted folder in the terminal.
If that is too much for you then i recommend to stay with vedders original version.
```

---
## \#796 Posted by: ekitesurfer Posted at: 2017-02-14T12:37:53.829Z Reads: 180

```
Cool, I will give it a shot or give up, thanks!
```

---
## \#797 Posted by: SeanHacker Posted at: 2017-02-14T16:24:00.438Z Reads: 187

```
I made an install video for you. Hope it helps you out dude. Screencast software I was using sucks and I'm down to one-handed typing because I broke my collar bone the other day. Sorry about that. But you get the idea I'm sure. ;)

https://www.youtube.com/watch?v=S8bhPrt7R9M
```

---
## \#798 Posted by: Ackmaniac Posted at: 2017-02-15T00:09:10.610Z Reads: 184

```
Thanks a lot for the video. I hope this solves the problem for @ekitesurfer.
```

---
## \#799 Posted by: SeanHacker Posted at: 2017-02-15T00:41:40.168Z Reads: 179

```
No problem. Hopefully it does. :slight_smile:
```

---
## \#800 Posted by: ekitesurfer Posted at: 2017-02-15T02:00:56.299Z Reads: 183

```
Right on, I am looking forward to checking it out when I get to work!
```

---
## \#801 Posted by: CamBo Posted at: 2017-02-15T05:05:25.405Z Reads: 180

```
@SeanHacker was this an esk8 injury?
```

---
## \#802 Posted by: SeanHacker Posted at: 2017-02-15T05:25:04.995Z Reads: 178

```
Yep :smile:
```

---
## \#803 Posted by: ekitesurfer Posted at: 2017-02-15T06:51:56.024Z Reads: 174

```
Hey, thanks a lot for the step by step video! That was exactly what I was hoping for. I have a few beers for you if you are ever in Vegas :)
```

---
## \#804 Posted by: etvoila Posted at: 2017-02-15T20:08:35.930Z Reads: 179

```
Hi, sorry about my english, i'm a french esk8.fr customer so i came here because i have a problem with the "start detection" with the great 2.53 firmware.

Pimousse advised me to come and ask you directly

when i started the detection, the engine starts to jerk and force, the vesc's light blink red/blue, finally "detecion failed" appears

I allready try to commute the cuttoff to 57v and 8v, many people have solved their problem like this but that doesn't work with me.
If anyone have an idea, thats will be great

Thanks a lot
```

---
## \#805 Posted by: Ackmaniac Posted at: 2017-02-15T20:26:10.952Z Reads: 174

```
You need to disable the remote settings. For example if you have a ppm remote you need to set this first to disabled and write the settings. Otherwise the motor detection get's disturbed by the remote commands.
After the detection you can switch them on again.

And minimum input voltage should be at 8V and maximum input voltage at 57V.
Battery cutoff start and end depends on your battery.
For a **Li-Ion** it should battery cutoff start should be at **3.0V** a cell a and cutoff end at **2.8V** a cell.
So for a 10S Battery (10 cells in series) **3.0V * 10S = 30V** for cutoff start and **2.8V * 10S = 28V** for cutoff end.

For a **LiPo** it should battery cutoff start should be at 3.6V a cell a and cutoff end at 3.4V a cell.
So for a 10S Battery (10 cells in series) **3.6V * 10S = 36V** for cutoff start and **3.4V * 10S = 34V** for cutoff end.
```

---
## \#806 Posted by: etvoila Posted at: 2017-02-15T20:32:01.095Z Reads: 181

```
Thanks for your fast reply

I know the part with my own battery, good guy teach me that on the forum, i  was just saying that some had solved their problems with this 8 and 57V

I'm going to try with your tricks, Thanks a lot !!

Edit
I have read the configuration, change and write but That the same thing, 

I think the problem is elsewhere
```

---
## \#807 Posted by: Surfer Posted at: 2017-02-15T20:40:51.077Z Reads: 174

```
Hi @Duffman,  maybe you like the idea to try to install a custom ROM for your old android, in that way you can have android 5  that runs with the app. If you need help to choose one, let me know. But probably is good to have a look Cyanogenmod or similar. Cheers
```

---
## \#808 Posted by: SeanHacker Posted at: 2017-02-15T21:17:14.021Z Reads: 176

```
Or he could try out AOKP http://gerrit.aokp.co/#/q/status:merged. CyanogenMod has recently rebranded to LineageOS and are having some merge issues at the moment. @Duffman Let me know if you'd like to update your device and I should be able to get you up and running in no time. If we don't already support your device, I can usually get unsupported devices working in an hour or so.
```

---
## \#809 Posted by: etvoila Posted at: 2017-02-16T10:57:30.282Z Reads: 173

```
@Ackmaniac thanks a lot budy, i've resolved my problem, it was a 4R7 chip who was broken
So i've soldering a normal 4,7ohm resistance and that work.

Thx !
```

---
## \#810 Posted by: Chigzy Posted at: 2017-02-17T07:58:26.455Z Reads: 181

```
Guys, just got my Bluetooth module, but a little confused on where to connect what. Plus, what cable do I use. Is there a specific name for the wire with the slide on pin connectors. Is it called a servo cable or something. Sorry for the dumbass questions
```

---
## \#811 Posted by: Pimousse Posted at: 2017-02-17T08:17:20.930Z Reads: 189

```
http://www.electric-skateboard.builders/t/vesc-hm-10-bluetooth-wiring/12838/19?u=pimousse

Connector JST-PH 6 or 7 pin (depending on your VESC HW version).
Here's a tutorial (in french but pictures may help) : [http://e-sk8.fr/forum/viewtopic.php?f=8&t=1126](http://e-sk8.fr/forum/viewtopic.php?f=8&t=1126)
```

---
## \#813 Posted by: Pimousse Posted at: 2017-02-19T10:21:46.204Z Reads: 194

```
Quick test of the latest version off the app.
(I need to setup the battery capacity properly)

https://www.youtube.com/watch?v=zyAhUCl9VZg

I still have a problem : the camera is upside down.
Not very useful but maybe it's only with my phone (Nexus 5X).
```

---
## \#814 Posted by: Eboosted Posted at: 2017-02-19T17:07:55.467Z Reads: 195

```
Is there a way to adjust PPM settings via HM-10?

I tried to use VESC Connect from the Android Market but I'm getting this message:

[img]http://i.imgur.com/t19rG8A.png[/img]

I guess it's because the latest Ackmaniac FW is newer than the VESC Connect software, it wouldn't let me read or write any settings.

Is there a way around this?
```

---
## \#815 Posted by: yaca Posted at: 2017-02-19T22:51:21.314Z Reads: 180

```
Just tried to install BLDC-Tool 2.53. (I had 2.52 before.) It didn't work, because there are missing some things on my computer. Do I have to download all the files (about 20). If so, do I still need them after I installed BLDC-Tool 2.53? Thank you!
```

---
## \#816 Posted by: Ackmaniac Posted at: 2017-02-19T23:02:02.669Z Reads: 176

```
Unzip the windows file and start bldc-tool in the unzipped folder.
```

---
## \#817 Posted by: yaca Posted at: 2017-02-19T23:17:38.244Z Reads: 192

```
<img src="/uploads/db1493/original/3X/8/1/81bdcd54a85fa7e518ff27db389a26e50e53bfb8.png" width="650" height="500">

 I click on the first and I get this. What do I have to do now? With 2.52 it was just one file I had to unzip!?

<img src="/uploads/db1493/original/3X/9/3/939c679ae578f59033ade08866af40351ffecf4f.png" width="650" height="500">
```

---
## \#818 Posted by: Ackmaniac Posted at: 2017-02-20T07:14:28.969Z Reads: 168

```
You have to download the complete zip file and Unzip it in a new folder on your drive.
```

---
## \#819 Posted by: yaca Posted at: 2017-02-20T08:22:20.584Z Reads: 175

```
You talk about the first zip file on the first screenshot? I don't see a possibility to download it. If I click on it, then there should be a button for download, but it just opens the second screenshot. On the first screenshot it doesn't show the size of the zip file, is there something wrong?
```

---
## \#820 Posted by: mnelson3690 Posted at: 2017-02-20T09:24:17.768Z Reads: 179

```
Hi, I am new to E skating. I am trying to figure out good settings in the bldc tool for my setup. I have a vesc, 6374 motor, and 10s3p battery. Anything will help
```

---
## \#821 Posted by: yaca Posted at: 2017-02-20T10:06:58.444Z Reads: 179

```
I think it would be better to start your own thread and at first you should read a lot in this forum. This thread is more special not really made for beginners.
```

---
## \#822 Posted by: Deakbannok Posted at: 2017-02-20T13:16:10.747Z Reads: 185

```
@Ackmaniac Everything is working as normal; I had to flash the firmware back and reset all default settings. 
Do you know how to connect BLDC Tools via Bluetooth connection on windows?
I have HM-10 installed on VESC-X
The bluetooth installed on Windows 10, but it doesn't have COM Port service installed. 
Do you need to use 3rd party software for this?

Thank you.
```

---
## \#823 Posted by: Ackmaniac Posted at: 2017-02-20T17:02:43.526Z Reads: 197

```
My firmware mod doesn't support a bluetooth connection to a Windows PC. It only works with Android smartphones.
```

---
## \#824 Posted by: yaca Posted at: 2017-02-20T17:30:58.235Z Reads: 188

```
Please help! Do you mean the first file in the first screenshot (BLDC-Tool_ACKMANIAC_MOD_Windows 2_53.zip)? Why isn't it possible to download?
```

---
## \#825 Posted by: yaca Posted at: 2017-02-20T17:52:39.326Z Reads: 188

```
Ok I got it. I had to go to the second screen and found a download button on the right top.
```

---
## \#826 Posted by: yaca Posted at: 2017-02-20T22:05:47.077Z Reads: 188

```
I try to setup the VESC Monitor. At Drive Gear Setup how many magnets should I enter? Jacob's hub motor has 14 pairs of magnets. So is it 14 or 28 what I have to enter?
```

---
## \#827 Posted by: Ackmaniac Posted at: 2017-02-21T05:41:44.076Z Reads: 193

```
The number if poles. Most motors have 14
```

---
## \#828 Posted by: Maxid Posted at: 2017-02-21T06:43:47.466Z Reads: 187

```
28 for jacob's motors
```

---
## \#829 Posted by: yaca Posted at: 2017-02-21T21:25:18.324Z Reads: 189

```
Next app question: When do you enable "Connect by CAN to ID ." Is it just if I have connected the HM-10 with the Slave VESC and want to receive datas from the Master (ID 0) or are there other functions?
```

---
## \#830 Posted by: Ackmaniac Posted at: 2017-02-22T07:12:48.756Z Reads: 189

```
You are absolutely right. You can also use it to connect to the slave via the master if you want to check the data of the slave.
```

---
## \#831 Posted by: Deakbannok Posted at: 2017-02-22T09:42:01.973Z Reads: 183

```
One question for the Android app.
When I changed motor/batt, and throttle curve settings. 
It doesn't stay registered onto the VESC?! 
So each time if I turn off the board and open the Android apps. It resets back to default?
```

---
## \#832 Posted by: Ackmaniac Posted at: 2017-02-22T13:10:59.644Z Reads: 188

```
That is exactly how I want it to be. After you selected the new mode you can press longer on the mode box and the app will ask you if you want to use this mode as the new default mode.

Can be very useful when the police stops you or when your kids take your board when you don't know it.
```

---
## \#835 Posted by: Pimousse Posted at: 2017-02-23T13:15:19.526Z Reads: 188

```
@Ackmaniac, I have a little feature request, I need your opinion about it.
Could you add in the battery settings a voltage threshold under which the phone vibrates (or rings) ?

On the french eskate forum, a guy had an issue with his VESC which lost all its parameters.
The batt. cutoff was at 10V so it never cuts off. He ruined 2 lipos (2,6V/cell).

It's really a rare case but it adds a security and if set at a upper value, it can prevent to walk a lot if you reach the cutt off far away from home :smile: 

What do you think about that ?
```

---
## \#836 Posted by: Ackmaniac Posted at: 2017-02-23T15:52:19.338Z Reads: 183

```
I will think about it. Shouldn't be a big problem to add that feature.
```

---
## \#837 Posted by: ekitesurfer Posted at: 2017-02-24T01:50:21.280Z Reads: 186

```
What do I click on to upload the firmware? It seems my choices are:

hw_46_47
hw_48
hw_410_411_412
```

---
## \#838 Posted by: JLabs Posted at: 2017-02-24T02:01:59.350Z Reads: 182

```
You correspond that to you VESC hardware version. If you look on the VESC itself somewhere in white text it will say 4.10, 4.11, 4.12 etc so you just selec the firmware that applies
```

---
## \#839 Posted by: ekitesurfer Posted at: 2017-02-24T02:09:06.727Z Reads: 187

```
Cool, thanks! Now my choices are:

vesc 0005ohm.bin
vesc default.bin
vesc servout bin
vesc ws2811.bin
```

---
## \#840 Posted by: JLabs Posted at: 2017-02-24T02:21:34.715Z Reads: 187

```
I'm not sure man, I am not fimiliar with ackmaniac's software..
```

---
## \#841 Posted by: SeanHacker Posted at: 2017-02-24T02:26:11.233Z Reads: 196

```
If you're using this version of BLDC_Tool you'll want to use the custom firmware for this software. Otherwise you won't get to use the benefits of this modified software. 

<img src="/uploads/db1493/original/3X/3/f/3f9a7e4ab6344ce75b28e1a1426337ae21317860.png" width="281" height="500">
```

---
## \#842 Posted by: ekitesurfer Posted at: 2017-02-24T02:30:55.452Z Reads: 179

```
Oh, I thought it was built into the modified bldc tool software. Where can I find that link to the dropbox?
```

---
## \#843 Posted by: SeanHacker Posted at: 2017-02-24T02:37:03.425Z Reads: 180

```
It's in the same Dropbox as this bldc_tool. It's the file with the .bin extension. https://www.dropbox.com/sh/t7dl90owz5ccbyl/AADNOs3g9TfYw-VAyYey3hZNa/BLDC-TOOl%20and%20Firmware?dl=0
```

---
## \#844 Posted by: ekitesurfer Posted at: 2017-02-24T02:52:32.820Z Reads: 184

```
Thanks a lot man! 

But now my remote does not respond...
```

---
## \#845 Posted by: jaykup Posted at: 2017-02-24T02:56:48.043Z Reads: 196

```
Enable PPM, it's off by default

<img src="/uploads/db1493/original/3X/4/2/42e6f3d637f58a48fc88d6bf03007f732d967034.png" width="403" height="354">
```

---
## \#846 Posted by: ekitesurfer Posted at: 2017-02-24T02:58:57.282Z Reads: 188

```
I did that, it wasn't working, but after I rebooted, it works Thanks! I love this forum, you guys are a big help.
```

---
## \#847 Posted by: Deakbannok Posted at: 2017-02-24T06:46:01.726Z Reads: 195

```
What if I just changed only the battery and motor settings.

Do I have to select and change the [√] Use special ThruttleCurve?!?

What If I don't select it. Would it reset the Curve settings back to default? or the ThruttleCurve settings will remain as they were?

Thank you so much for the work and effort you done here for the community!
It may not be much for attribution but that will last you for a few beers @Ackmaniac
```

---
## \#848 Posted by: SeanHacker Posted at: 2017-02-24T06:56:18.461Z Reads: 192

```
You don't have to use the throttle curve. If you don't select it the settings will not be kept and will go back to default.
```

---
## \#849 Posted by: ekitesurfer Posted at: 2017-02-24T18:43:12.254Z Reads: 192

```
Wow, holy shit this turned my esk8 into a whole different beast! ackmaniac is a genius!!! Sending some duckets your way. Everybody should run this!!!!
```

---
## \#850 Posted by: Pimousse Posted at: 2017-02-27T18:43:50.882Z Reads: 187

```
@Ackmaniac, I told you about a case of a french guy who had a bad time with his VESC which lost parameters (actually, all came back to default values).
We concluded that he probably accidentally clicked on "Write default" on BLDC Tool.

BUT, a second guy had this issue as well, after switching off and on his board.
Hoppefully, he didn't draw too much from the batteries.
Both use FW 2.53.

Anyway, it's quite scary. 
Could you investigate on these issues on your side ?
```

---
## \#851 Posted by: Ackmaniac Posted at: 2017-02-27T19:43:06.219Z Reads: 188

```
Well, i think it is very easy to do a mistake there. Or maybe the storage has a issue. I realized that when i change the settings and directly switch off the VESC afterwards by pressing the reboot button then the VESC can become issues.
So i recommend to write the settings and wait a little before you press the reboot button. And best is to check the settings after the reboot to be absolutely safe.
So i think that user wrote the settings and immediately pressed the reboot button afterwards.
```

---
## \#852 Posted by: Pimousse Posted at: 2017-02-27T20:17:16.477Z Reads: 179

```
It happened after disconnect/reconnect the XT90s, no BLDC Tool connected.
That's why this time the issue seems more serious.
```

---
## \#853 Posted by: Ackmaniac Posted at: 2017-02-27T20:22:46.747Z Reads: 184

```
That's very hard for me to imagine. But maybe the storage of his VESC had an issue. I don't use anything else then the functionality of the standard Firmware to store the values.
```

---
## \#854 Posted by: Pimousse Posted at: 2017-02-27T20:28:59.342Z Reads: 189

```
But your firmware lets the user to use custom recipes of parameters.
Couldn't be a overwrite of the firmware with the defaults values ?
(sorry if it appears a dumb question, but without sources I can't precisely understand how works your firmware on this sides).

Anyway, thanks for your support.
The french guy wants also thank you for this amazing FW. ;)
```

---
## \#855 Posted by: Moja Posted at: 2017-03-01T22:50:04.337Z Reads: 181

```
I'm getting the "not a valid WIN32 application" error message when I try to launch the BLDC_tool.exe in Windows XP, is it compatible?
```

---
## \#856 Posted by: Ackmaniac Posted at: 2017-03-01T22:56:35.627Z Reads: 178

```
Did you extract all the files in the Zip folder and then start the exe file in the extracted folder? I never tested with windows xp. Maybe some other users got it running under windows xp.
```

---
## \#857 Posted by: Moja Posted at: 2017-03-02T00:05:19.510Z Reads: 174

```
I did extract the files, I'll try on another machine and see if i get lucky
```

---
## \#858 Posted by: Eboosted Posted at: 2017-03-02T05:23:46.610Z Reads: 180

```
I had this same exact problem not one but several times, I updated the motor settings clicked on write settings and went for a test ride, it wasn't runing correctly so I connected the USB again and found out the settings were completely reseted, cut off voltage was 10v and all motor settings and motor detection values were defaulted. 

This happened to me 4-5 times, unfortunately I still don't know how to trigger this error, so we could report it, but it only happens once in a while
```

---
## \#859 Posted by: Ackmaniac Posted at: 2017-03-02T08:38:35.398Z Reads: 177

```
This might happen when you write the settings and don't wait for the confirmation in BLDC-Tool. In the lower right of the screen you see a message popping up shortly that they have been written correctly. And don't press the reboot button to fast after the write. Just wait for like 5 seconds.
And you also can avoid it by double check the settings after you wrote them.

But i will also have a look into the code if there is something that i might missed.
@Eboosted did you change the settings only via the BLDC-Tool or also via the app?
```

---
## \#860 Posted by: yaca Posted at: 2017-03-02T09:25:29.682Z Reads: 181

```
I had this problem also a few times with firmware 2.18. Now I always double check after I wrote new values. I connect again and read and see if everything is alright.
```

---
## \#861 Posted by: Ackmaniac Posted at: 2017-03-02T10:53:41.231Z Reads: 187

```
I am adding extra checks if the VESC is connected correctly to the BLDC-Tool, so that you will see a message if the connection is lost. So i hope i can finish that over the weekend. Because the original doesn't inform you when the connection is not there. 

And i also recommend that when you write the settings that you wait for a while (like 5 seconds) before you press the reboot button or switch off the board. And check that the little green message on the bottom left blinks up after you wrote the settings.
```

---
## \#862 Posted by: Qwiksand Posted at: 2017-03-02T14:20:42.838Z Reads: 192

```
Fantastic work, just awesome! You've invested a ton of time, heart and soul into this project and it is obvious you are very passionate about this hobby as this project of yours is a real gem. Thank you!

Would it be possible to add support for the "ADC and UART"control mode via the app? I've got a scooter and a mountain bike project that would benefit greatly from being able to adjust settings/modes on the fly.
```

---
## \#863 Posted by: Eboosted Posted at: 2017-03-06T04:56:34.316Z Reads: 203

```
@ackmaniac is there anyway to change VESC settings loaded your latest firmware and a mobile BLDC tool?

1. VESC monitor - This is the only app that connects perfectly, but won't let me change VESC settings

2. Metr.at and Perimetr are closed versions and I will need to buy their own bluetooth module

3. VESC connect, is not compatible to your latest FW:

[img]http://i.imgur.com/t19rG8A.png[/img]
```

---
## \#864 Posted by: Ackmaniac Posted at: 2017-03-06T09:14:10.213Z Reads: 191

```
Which VESC settings to you want to change. 
With my app you can change 
Motor max and min, 
Battery max and min, 
Max Watts, 
Control mode for PPM, Nunchuk and NRF, 
max speed, 
throttle curve settings 
and Cruise control settings.

And you can save as many different mode setups as you like and switch with one click.
```

---
## \#865 Posted by: Eboosted Posted at: 2017-03-06T14:31:19.794Z Reads: 194

```
I'd like to change, start up current ramp, make motor detection, change hall sensors order and adjust ppm settings
```

---
## \#866 Posted by: Hillso Posted at: 2017-03-06T15:43:06.330Z Reads: 206

```
I get an error:

<img src="/uploads/db1493/original/3X/9/0/904708460a90a3174095a59b6fbf4974d25a2e56.png" width="657" height="423"> 

I did this:
<img src="/uploads/db1493/original/3X/9/2/9251ac8cb79900342147c0a46117d0af3bf83698.png" width="440" height="500">

and this:
https://launchpad.net/gcc-arm-embedded/+announcement/13824
```

---
## \#867 Posted by: Ackmaniac Posted at: 2017-03-06T16:06:32.435Z Reads: 184

```
Could it be that QT Creator isn't installed on your machine?

@Eboosted. If you want to make these changes then i am sorry to tell that my app can't do it, as you already know.
But motor detection should be done once and that's it.
hall sensor order should also be detected once.
PPM settings also need to be adjusted once because your remote doesn't change.
Only thing that really makes sense to me is the startup current ramp.
```

---
## \#868 Posted by: Hillso Posted at: 2017-03-06T17:57:42.951Z Reads: 186

```
I just installed QT Creator. again, same problem:
<img src="/uploads/db1493/original/3X/3/5/35e5e088928ac9086943ddd271467fcfed8a5d7e.png" width="657" height="423">

I'm new to linux :(
```

---
## \#869 Posted by: Pimousse Posted at: 2017-03-06T19:01:27.507Z Reads: 174

```
Erf, I had hard time with it as well.

Did you follow Vedder instructions ? 
http://vedder.se/2015/01/vesc-open-source-esc/

It helps a lot for me. ;)
```

---
## \#870 Posted by: Hillso Posted at: 2017-03-06T19:40:35.261Z Reads: 200

```
I only did this part (because I already uploaded the 2.53 firmware from windows):
<img src="/uploads/db1493/original/3X/1/2/12af8739e552b7dd32bc725613c555ef7eb40629.png" width="440" height="500">

It's really confusing for me, do I need a stlinkv2 programmer?
```

---
## \#871 Posted by: Pimousse Posted at: 2017-03-06T19:55:56.747Z Reads: 197

```
If you just want BLDC Tool, skip this part. It's for compliling the firmware.

Jump to the part begining by 

> Download, Compile and Start BLDC Tool

> From the BLDC directory that you created in the previous step, type:

> git clone https://github.com/vedderb/bldc-tool.git bldc-tool
> cd bldc-tool
> qmake -qt=qt5
> make
> ./BLDC_Tool

But instead using Vedder's one, just unzip Ackmaniac's one.
```

---
## \#872 Posted by: Hillso Posted at: 2017-03-06T20:21:41.135Z Reads: 206

```
I feel stupid, I already installed qt creator:
<img src="/uploads/db1493/original/3X/b/d/bd94e2ac2eff2f7f1b2c64a7c095c4879d4412a2.png" width="657" height="423">
```

---
## \#873 Posted by: Pimousse Posted at: 2017-03-06T20:34:21.350Z Reads: 210

```
Out of my knowledge. Sorry.
:neutral_face:
```

---
## \#874 Posted by: Ackmaniac Posted at: 2017-03-08T21:19:48.834Z Reads: 235

```
I made a update with some new features and improvements of the firmware.

**- Hysterisis added to BLDC mode in Sensored Hybrid mode.**
In FOC mode there is a hyterisis when the motor switches from sensored to unsensored mode which is at standard at 5%.
So if you set "Sensorless ERPM" parameter to 2000 then the VESC will switch to sensorless when it reaches 2000 + (2000 * 0.05) = 2100 ERPM and it switches back to sensored mode when it reaches 2000 - (2000 * 0.05) = 1900 ERPM. This is to prevent that the VESC switches hundrets of times a second between sensorless and sensored when you are directly at this ERPM speed.
This didn't exist in BLDC mode. So thanks to the hint of @Duffman i implemented this feature which hopefully solves his problem and makes the hybrid mode smoother and also causes less stress on the components. I made the hysterisys 10% of the "Sensorless ERPM" parameter and also changed it in FOC mode to 10%.

**- Bugfix for wrong Tachometer counting in FOC mode**
I analysed together with @Maxid the data of his ride. And he found out that the VESC reading is about 10 % off from reality. In my own readings at slow test rides it was about 5 % off.Sadly i never checked the distance in FOC (only verified it in BLDC). So i checked the source code and i am happy to tell that i fixed the issue.
Finally this is only really interesting for apps because there you need the distance to calculate the Wh consumption and the range. I made a couple of test runs and i am quite sure that the distance detection is now as good as in BLDC at riding situations.

**- Improved the writing and reading of settings**. 
@Pimousse mentioned that he saw a loss of settings. I had a look at the code and made a little impovement that trys to write the settings again if the first try failed. Hopefully this prevents that the VESC switches back to the default settings when something is wrong with the memory. I can't make sure that my changes really prevent that from happening but at least my changes don't hurt and i think that there is a chance to have that problem fixed. This is a problem that can occur also in the standard firmware. So there is no difference in my firmware mod.

This time i didn't give the firmware a new version number because of the following three reasons.

First of all the changes are not necessary and only really usefull if you use my android app and FOC or ride in BLDC mode with the hybrid sensor mode.

No new parameters are added. So BLDC-Tool is still the same.

And if you used already version 2.53 you only need to do the following steps to switch to the new firmware: **(do not close BLDC-Tool in between)**
1. connect to the VESC in BLDC-Tool.
2. read the motor settings
3. read the app settings
4. upload the new firmware file (VESC_Ackmaniac_2_53_new.bin)
5. connect to the VESC again 
6. write motor settings
7. write app settings
Finished
So you don't need to make all the settings again if you used already version 2.53. You simply first load them in BLDC-Tool, flash the new firmware and write the old settings to the new firmware.

[Windows BLDC-Tool, Modified Firmware, Ubuntu BLDC-Tool and Android app](https://www.dropbox.com/sh/t7dl90owz5ccbyl/AAANyC-yQCMeveA7errNRnYqa?dl=0)

Android App download in Google Play Store
[Android App](https://play.google.com/store/apps/details?id=ackmaniac.vescmonitor&hl=de)

[Bluetooth modules ca be ordered here.](https://de.aliexpress.com/item/HM-10-BLE-Bluetooth-4-0-CC2540-CC2541-Serial-Wireless-Module/32516357718.html?spm=2114.13010608.0.0.cbyTeS&detailNewVersion=&categoryId=400103)

Cable to connect the Bluetooth Module with the VESC easily
[Cable with Connector](https://www.aliexpress.com/item/2-0mm-PH-7-Pin-Male-Female-Connector-with-Wire-x-10-Sets/32616271304.html?spm=2114.01010208.3.18.RewfhB&ws_ab_test=searchweb0_0,searchweb201602_3_10065_10068_10000032_10000025_10000029_430_10000028_10060_10062_10056_10055_10054_10059_10099_10000022_10000012_10103_10102_10000015_10101_10096_10000018_10000019_10052_10053_10107_10050_10106_10051_10000007_10084_10083_10080_10082_10081_10110_10111_10112_10113_10114_10115_10037_10032_10000041_10000044_10078_10079_10077_10000038_429_10073_10000035,searchweb201603_1,afswitch_2,single_sort_2_default&btsid=0ef89f27-529d-4685-8740-13e10dbd5fcc)

And if somebody wants to honor all the work.
[Donations](https://www.paypal.com/de/cgi-bin/webscr?cmd=_flow&SESSION=-P6lRlkFOyJeroABtf7htelg80qLQk2pKvQD8dkA_L3ff5QSvJmz8Z0LeQK&dispatch=5885d80a13c0db1f8e263663d3faee8d333dc9aadeed3fe0b5b299d55fd35542)
When you want to send a donation then don't use dots. (Germany uses commas). So use full numbers or a comma.
```

---
## \#875 Posted by: Eboosted Posted at: 2017-03-09T00:27:27.307Z Reads: 208

```
@Ackmaniac you rock!

You are really keeping track of all users feedback, this is getting close to perfection.

I plan to keep ussing yout firmware when VESC 6 comes out, hope Vedder make mentions you
```

---
## \#876 Posted by: Plumb77 Posted at: 2017-03-09T01:29:08.481Z Reads: 203

```
Just to make sure this will work with @oriol360 Bluetooth module?
```

---
## \#877 Posted by: Eboosted Posted at: 2017-03-09T04:01:08.343Z Reads: 201

```
Is it possible to update your latest firmware via the android app?
```

---
## \#878 Posted by: Ackmaniac Posted at: 2017-03-09T09:08:00.066Z Reads: 194

```
@Plumb77 you can try the app with the standard firmware 2.18 to make sure that the bluetooth module is working. but to have the full functionality of the app you need my firmware mod.

@Eboosted no you can't
```

---
## \#879 Posted by: mmaner Posted at: 2017-03-09T17:22:50.801Z Reads: 194

```
[quote="Plumb77, post:876, topic:12286, full:true"]
Just to make sure this will work with @oriol360 Bluetooth module?
[/quote]

It does, I am using a MEB Bluetooth module in my dual motor build with @Ackmaniac F/W.
```

---
## \#880 Posted by: Pimousse Posted at: 2017-03-10T08:46:59.551Z Reads: 195

```
Thank you very much @Ackmaniac to listen closely to user's feedback !

BTW, how do you see things coming with the VESC 6 release ?
Will you still support v4, support both (or maybe only v4 and wait until first v6 issues will be fixed) ?
I assume re-writing all your amazing feature in the v6 firmware will be a ton of work !!
```

---
## \#881 Posted by: Ackmaniac Posted at: 2017-03-10T08:55:00.427Z Reads: 193

```
Vedder implemented already the most of my ideas in the VESC 6 firmware. For the rest I need to have a look but I am pretty sure that I will do the job. For the V4 hardware the changes also need to be done for VESC-tool.
```

---
## \#882 Posted by: Pimousse Posted at: 2017-03-10T10:14:48.322Z Reads: 197

```
Great !
Vedder mentioned that the new firmware is much more structured and oriented in a collaboration way.
Hope it will let you save time for future improvement. ;)

Are you in touch with Vedder ?
Do you know if UART communication will be also modified ?

I'd love to monitor VESC 6 behavior with your app, first for beta testing (I'm in the beta program) and then because the way I'm planning to use them is in a heavy duty conditions (mountainboard in Alps :smile:).
```

---
## \#883 Posted by: Ackmaniac Posted at: 2017-03-10T11:35:42.443Z Reads: 196

```
Sadly I don't stay in contact with Vedder. I tried once but he didn't reply. Guess he's too busy. 
I also would like to know if the communication changes. He had plans doing so.
```

---
## \#884 Posted by: Ackmaniac Posted at: 2017-03-10T13:36:24.881Z Reads: 202

```
I am working on a update of the app to have the data visualization in the video a bit nicer.

<img src="/uploads/db1493/original/3X/b/4/b4f2d77e11f531cf91265cb9aa830e02461acbf9.png" width="690" height="388">
```

---
## \#885 Posted by: fedestanco Posted at: 2017-03-10T13:41:47.563Z Reads: 197

```
Hi, have you ever thought of developing an android wear app? I have one lg smartwatch that I dont use much. I can borrow it to you for few months if it could help.
```

---
## \#886 Posted by: Ackmaniac Posted at: 2017-03-10T13:51:19.244Z Reads: 199

```
I am living in Germany. So i guess the shipping would be a bit of a hustle. 
I think the best option would be to have a standalone Smartwatch application where you don't need to connect to the Smartphone. So that the smartwatch has a direct communication with the VESC. At the moment i have no idea how many Smartwatches have Bluetooth low energy. But it's a nice idea.
```

---
## \#887 Posted by: fedestanco Posted at: 2017-03-10T14:07:47.244Z Reads: 191

```
I live in Italy so shipping will be pretty cheap. What about I pay the way to your house, and then you return the watch when you ll be done?

Btw it is about 150g for shipping purpose.
```

---
## \#888 Posted by: Maxid Posted at: 2017-03-10T14:10:48.635Z Reads: 189

```
Personally I have no need for a standalone watch app since the phone is always with me when riding anyway. I would love to see the battery voltage and maybe speed on my watch while riding - more is not even necessary. Much safer than getting the phone from your pocket everytime.
```

---
## \#889 Posted by: TarzanHBK Posted at: 2017-03-10T14:15:10.808Z Reads: 190

```
At the moment I use my Sony Smartwatch 3 with Google Fit "Skating" while i ride. It shows speed, riding time, and other things, which is really cool!
If I use your app, it would be awesome to have connection to my watch to show the same things like google fit but also things like battery stuff or something else board related :slight_smile:
```

---
## \#890 Posted by: Eboosted Posted at: 2017-03-10T14:23:50.917Z Reads: 192

```
If I would have worked a lot if time and accomplish great success on BLDC tool, I would feel really disappointed if Vedder didn't even mentions me. I know Vedder had done a lot for the community without and asking for anything but lack of mentions on both ways makes me a little bit uneasy. 

Anyways, seeing how close you follow the feedback from users, there wouldn't be a better FW than @ackmaniac on VESC 6, so you should be covered =)
```

---
## \#891 Posted by: Maxid Posted at: 2017-03-10T14:29:32.201Z Reads: 197

```
Nice watch ;)
https://www.dropbox.com/s/vxscv4cki2khgip/2017-03-10%2015.26.00.jpg?dl=0
```

---
## \#892 Posted by: Ackmaniac Posted at: 2017-03-10T14:35:38.868Z Reads: 196

```
Ok ok ok. I will read some more stuff and i need to buy a Smartwatch. But at the moment i don't have the time to develop it because i first need to finish some other stuff. But give me a couple of weeks to gain some knowledge about it.

@fedestanco thx for the offer but when i develop a app for the Smartwatch then i also need one that i don't have to send back. Because the development is a ongoing process. Seeing my current app has already 50 updates. 
And i hate it to wear watches because living without time is nicer. When i made a world travel i sometimes didn't even know which month it was (no drugs involved). But for riding it could be really usefull.

If somebody has a old smartwatch and doesn't need it anymore then feel free to send it to me to support the project. Donations are also welcome.
```

---
## \#893 Posted by: Ackmaniac Posted at: 2017-03-11T02:55:39.472Z Reads: 195

```
**IMPORTANT** **IMPORTANT** **IMPORTANT** **IMPORTANT** **IMPORTANT** **IMPORTANT**
I have a sleepless night, because i found out that i made a terrible mistake with the cruise control function.
When you enable braking under cruise control and use it at low speeds, then the VESC brakes very hard which is wrong. If you only used cruise control without braking then it was fine.

Please update your VESC to the new firmware file **VESC_Ackmaniac_2_53_cruise_fixed.bin** where this issue is fixed and cruise control works as gentle as it should.
Luckily not many people used cruise control yet.

Please don't add posts below this comment as long as they are not super important so that everybody can see it. If you have less important questions you can PM me.
```

---
## \#894 Posted by: Plumb77 Posted at: 2017-03-11T13:54:06.198Z Reads: 195

```
Not sure if I'm doing some wrong. I downloaded the Mac version from drop box and when I go to open it i keep getting a error for damaged and cannot be open
```

---
## \#895 Posted by: gaetjen Posted at: 2017-03-12T19:52:17.484Z Reads: 194

```
like your idea of adjusting the display. It would also be nice to have an option to reduce the data visualization and then only having a few informations like speed, distance or range during videotaping. Just an idea :slight_smile:
```

---
## \#896 Posted by: Eboosted Posted at: 2017-03-12T21:36:08.238Z Reads: 194

```
What app do you guys use to display the logs with Google maps integration? 

I'd like to use metr but the app it's locked by hardware
```

---
## \#897 Posted by: Ackmaniac Posted at: 2017-03-12T23:28:20.203Z Reads: 192

```
You have to upload the CSV file to this page http://www.gct-hp.de/VDLA/
```

---
## \#898 Posted by: kampfhahn Posted at: 2017-03-12T23:58:08.226Z Reads: 189

```
After @Maxid told me about your project a few weeks ago (i was a bit out of the esk8 game in the winter months), i finally installed your firmware on my VESC an hour ago. Setup (with FOC) worked well as well as the first two-meter-ride in my apartment :D . Can't wait to take the first ride with it. Thanks for your contribution to the esk8 community, i will definitely donate after my test rides!
```

---
## \#899 Posted by: Plumb77 Posted at: 2017-03-13T19:35:38.946Z Reads: 193

```
2 things where do I solder this to the enertion vesc ? Also I can't find the right download for the bldc tool. I download it and it says corrupt file on Mac OSX
```

---
## \#900 Posted by: Ackmaniac Posted at: 2017-03-14T00:15:16.753Z Reads: 199

```
I have no Mac so I can't really help you with it. Best would be if you send us a screen shot of the error message. I am pretty sure that @The_Dude can help you. 

Currently I am working on  a improvement of watt control. Because at the moment the power output of the slave motor is too much dependent on the masters speed. First tests feel really amazing. Difference is only a little but it smoothen's the ride when you accelerate and carve at the same time. 

And the new version would be a great control mode for 4wd. Because you could give more acceleration power to the back wheels and more brake power to the front wheels and have them all in one CAN bus.

Also the setup will become easier because the max_watt parameter isn't needed anymore.
```

---
## \#901 Posted by: jbruce Posted at: 2017-03-14T02:56:31.688Z Reads: 191

```
Will the board calculate its own max watt based on the pack voltage at the time and the max amps? Just a thought I had.
```

---
## \#902 Posted by: The_Dude Posted at: 2017-03-14T06:54:44.586Z Reads: 196

```
Which file did you download from dropbox (BLDC-Tool ACKMANIAC_Mod_MAC_2.53.pkg.zip)? If so, please try to download it once again. Maybe something went wrong during download. Corrupt file sounds not like an Mac OSx issue.
```

---
## \#903 Posted by: guyguy Posted at: 2017-03-14T20:44:54.179Z Reads: 199

```
Anybody notice a consistent gap between GPS speed and the speed calculated out of the app - my GPS speed keeps coming out around 10MPH faster than the regular speed calculation. I'm guessing the latter is more accurate. I'm curious because a lot of videos I've seen seem to rely on GPS speed overlays.

Example: 

<img src="/uploads/db1493/original/3X/7/3/73d7b308cc4daf3a7c4b1162c8d08469ee272be4.jpg" width="690" height="297">
```

---
## \#904 Posted by: Ackmaniac Posted at: 2017-03-14T20:57:31.386Z Reads: 187

```
Did you adjust you wheelsize an gearing ratio by setting the wheel and motor pulley in the app. You also need the correct number of magnets in your motor.
```

---
## \#905 Posted by: Pimousse Posted at: 2017-03-14T20:59:28.034Z Reads: 186

```
Mine are exactly the same.
There is just a little delay between both.
```

---
## \#906 Posted by: guyguy Posted at: 2017-03-14T21:04:11.331Z Reads: 188

```
Yes, gear size pulley size are all correct. Magnet is correct. I don't have issues with those calculated speeds, they seem accurate to me - it's more that the GPS seems pretty far off. I definitely wasn't going 38mph. 

I see the delay in the data file and visualization - more of a concern is the much higher speeds reported. I see a lot of videos of board companies using these GPS overlays to show speeds and it just doesn't seem very accurate to me.
```

---
## \#907 Posted by: Ackmaniac Posted at: 2017-03-14T21:23:53.788Z Reads: 185

```
Then I guess I have a error in the log files so that GPS shows km/h instead of mi/h. Will check that tomorrow.
```

---
## \#908 Posted by: jaykup Posted at: 2017-03-15T03:28:08.876Z Reads: 188

```
[quote="guyguy, post:903, topic:12286"]
Anybody notice a consistent gap between GPS speed and the speed calculated out of the app
[/quote]

I have the same issue - [posted here](http://www.electric-skateboard.builders/t/vesc-data-log-analyzer-vdla/16582/23)

When you set the app to MPH it just changes a flag at the top of the CSV file, the web app is expecting a different value and tries to convert.  Or something.

Quick fix set the app to kph then change the web site to mph.
```

---
## \#909 Posted by: Plumb77 Posted at: 2017-03-17T18:43:34.878Z Reads: 181

```
I'll check this weekend which file it was. And report back
```

---
## \#910 Posted by: yaca Posted at: 2017-03-18T18:19:38.832Z Reads: 184

```
[quote="Ackmaniac, post:900, topic:12286"]
Also the setup will become easier because the max_watt parameter isn't needed anymore
[/quote]
Isn't it possible then to set the max_watt anymore?
```

---
## \#911 Posted by: Ackmaniac Posted at: 2017-03-18T18:34:12.738Z Reads: 181

```
Right, the maximum power ouput is then controlled by the battery max. It still works and feels very similar.
```

---
## \#912 Posted by: bullrider12 Posted at: 2017-03-18T19:29:47.086Z Reads: 188

```
Hey, 
Im also using your Watt control Mode and the Installation Works perfectly. I  only got one Problem with the app and its ability to change modes. 

I set up a New Mode with the exact same parameters as the default mode except the speed (change to 6 kmh just to try it out). Everytime i try to change it to new Mode it go es back to the default mode. Even reconnecting doesnt help.

Do you have any idea how i can solve this?
```

---
## \#913 Posted by: Ackmaniac Posted at: 2017-03-18T19:34:09.725Z Reads: 179

```
Do you have the latest version of the app? Please have a look at Google play and check if there is a update
```

---
## \#914 Posted by: bullrider12 Posted at: 2017-03-18T19:41:19.653Z Reads: 185

```
Yeah, i got the latest version according to the playstore  (1.12)
Do in have to set something up in the bldc tool before i can make Those changes?
```

---
## \#915 Posted by: Ackmaniac Posted at: 2017-03-18T19:44:22.199Z Reads: 183

```
And you also got the latest version of the firmware?
```

---
## \#916 Posted by: bullrider12 Posted at: 2017-03-18T19:46:38.044Z Reads: 181

```
Should be 2.53 the fixed one, isn't it?
```

---
## \#917 Posted by: yaca Posted at: 2017-03-18T19:49:25.823Z Reads: 178

```
Do you switch off the board, because if you do that you will have always the default mode. You can make the new mode to the default mode if it should stay.
```

---
## \#918 Posted by: Ackmaniac Posted at: 2017-03-18T19:49:55.356Z Reads: 184

```
Yes but I provided already w upgrades for this firmware. The latest one about a week ago. I will check later on if there could be a issue in the app. But I am pretty sure that it works with the newest versions.
Version 2.54 is already on the way and should be ready in a couple of days.

And Yaca is absolutely right. To store the new settings you have to press longer on the mode box and the app will ask you of you want to set the actual settings as default.
```

---
## \#919 Posted by: bullrider12 Posted at: 2017-03-18T19:56:58.829Z Reads: 181

```
No I'm not switching off anything, just trying to change the default mode to the custom mode ^^ with some reconnecting in between.
```

---
## \#920 Posted by: Eboosted Posted at: 2017-03-18T20:04:16.080Z Reads: 180

```
I had a reseting to default values issue again yesterday. 

I changed some parameters make a reboot and motors did not spin, remote did not respond. 

I guess rebooting is not a good idea when setting up you VESC parameters
```

---
## \#921 Posted by: yaca Posted at: 2017-03-18T20:12:28.827Z Reads: 183

```
At your new Mode did you choose at "Modes Setup" the mode for example "Watt no Rev. with Break"? If you forget this it appears "disabled" and so the new Mode doesn't work.
```

---
## \#922 Posted by: Ackmaniac Posted at: 2017-03-18T20:27:24.154Z Reads: 176

```
@Eboosted i think i found the error for that in the code. But that is a issue from the original firmware. In my new version that comes in the next days i hope that this issue is a thing of the past.
```

---
## \#923 Posted by: Eboosted Posted at: 2017-03-18T21:08:10.252Z Reads: 174

```
That'll be awesome!
```

---
## \#924 Posted by: bullrider12 Posted at: 2017-03-18T21:39:13.482Z Reads: 172

```
Yeah, I even did that. It seems that the app isn't able to initialize the new mode
```

---
## \#925 Posted by: Ackmaniac Posted at: 2017-03-18T21:52:45.113Z Reads: 174

```
Please update the firmware to the latest version in the Dropbox link and try it again.
```

---
## \#926 Posted by: SageTX Posted at: 2017-03-19T21:28:29.953Z Reads: 176

```
[quote="bullrider12, post:912, topic:12286"]
Everytime i try to change it to new Mode it go es back to the default mode. Even reconnecting doesnt help.
[/quote]

@Ackmaniac I've been having this issue too. Upgraded to newest firmware, reinstalled app and re-setup modes.  
It just reselects default mode.  
Hope you have found the glitch.
```

---
## \#927 Posted by: Ackmaniac Posted at: 2017-03-19T21:54:35.251Z Reads: 183

```
Can you make a video of that behavior. But i think that this is because of the Bluetooth module that you use. But a video would help a lot. And also a picture of your Bluetooth module would be great and the info where you got it from.

A explanation for this is that with Bluetooth low energy you can only send 20 bytes in one transaction. So longer messages will be splitted in multiple packages of 20 bytes or less. So it seems that the split of the messages that are received is OK but maybe the sending has issues.
```

---
## \#928 Posted by: SageTX Posted at: 2017-03-19T22:59:11.691Z Reads: 185

```
https://youtu.be/FaxOnTvxkus
```

---
## \#929 Posted by: SageTX Posted at: 2017-03-19T23:02:20.543Z Reads: 183

```
(Bluetooth module) https://www.amazon.com/dp/B010SFF8QC/ref=cm_sw_r_cp_apa_A2WZyb9GKA75G
```

---
## \#930 Posted by: bullrider12 Posted at: 2017-03-19T23:08:38.918Z Reads: 185

```
This is exactly the same problem I have with the app. I got this Bluetooth module: https://www.amazon.de/gp/product/B00V07U93U/ref=oh_aui_detailpage_o07_s00?ie=UTF8&psc=1

PS.: I like that "Pussy"-Mode :D
```

---
## \#931 Posted by: SageTX Posted at: 2017-03-19T23:10:53.556Z Reads: 184

```
Lol. I was just setting them up to re try the modes. Going for something _descriptive_ .
```

---
## \#932 Posted by: Ackmaniac Posted at: 2017-03-19T23:22:19.539Z Reads: 188

```
I guess the standard configuration of the module isn't the same like my bluetooth modules.
Moe info how to programm the sunfounder module is here.
http://wiki.sunfounder.cc/index.php?title=Bluetooth_4.0_HM-10_Master_Slave_Module

Easiest way to solve this is to order the modules from my link in the first post which are pretty cheap. But they need a while to get shipped.
```

---
## \#933 Posted by: SageTX Posted at: 2017-03-19T23:37:43.937Z Reads: 189

```
What needs to be programed? Just a matter of setting a parameter?  
Which one?
```

---
## \#934 Posted by: SageTX Posted at: 2017-03-19T23:49:39.451Z Reads: 190

```
@Ackmaniac's link he referred to if anyone else was looking  


http://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286/260?u=sagetx  

But it links to German Ali express which is why i bought from Amazon
```

---
## \#935 Posted by: Ackmaniac Posted at: 2017-03-19T23:58:19.856Z Reads: 190

```
That's the same module at the english version of Aliexpress
https://www.aliexpress.com/item/HM-10-BLE-Bluetooth-4-0-CC2540-CC2541-Serial-Wireless-Module/32516357718.html?isOrigTitle=true

Tomorrow i will try to get some more knowledge about it but i guess most of you don't like to program the modules with a Arduino. Maybe somebody has some more knowledge and can help.
So i recommend to buy the modules in the link. If you need them quicker then try to order a module on ebay which looks exactly the same. You see the number "**ZS-040**" on the back of the module.
```

---
## \#936 Posted by: Pimousse Posted at: 2017-03-20T06:51:51.581Z Reads: 183

```
I did play a bit with AT commmands to customuze my HM-10, if I can help,
```

---
## \#937 Posted by: Ackmaniac Posted at: 2017-03-20T07:32:12.216Z Reads: 189

```
If the app works for you then it would be great if  you can check the settings on your module and then get in contact with @SageTX or @bullrider12 to figure out if there is a difference.
```

---
## \#938 Posted by: Ackmaniac Posted at: 2017-03-20T10:09:42.579Z Reads: 208

```
I uploaded a new Version of the app.
Now it is possible to choose between different realtime data layouts when you capture videos of your ride.

Here you can choose between the different Layouts
<img src="/uploads/db1493/original/3X/b/e/be3c9ca1622374b2a35606d6e57f2636b53c3903.png" width="281" height="500">

This is the Left and Right Layout
<img src="/uploads/db1493/original/3X/d/d/dde87c344d18eac1b2f5ecf4acbf21e04322e6c3.png" width="690" height="388">

This is the minimized Layout
<img src="/uploads/db1493/original/3X/3/b/3b0278e6e634631634d5bf24ca500180aa9a7d9e.png" width="690" height="388">
```

---
## \#939 Posted by: SageTX Posted at: 2017-03-20T12:24:21.739Z Reads: 190

```
@Ackmaniac @Pimousse  Just wanted to mention,  mode selection _used_ to work flawlessly.  Started getting glitchy a few updates ago.  Anyway, would love to program or check settings, but did order the other module as well.
```

---
## \#940 Posted by: Ackmaniac Posted at: 2017-03-20T12:34:52.286Z Reads: 192

```
Then i am pretty sure that this is because of the 20 byte limit of Bluetooth low energy. Because in the older versions it was only 17bytes that i send. But in the newer version it is more because of the throttle curve settings. So the message will be split in multiple parts of 20 bytes each.
I can try to add a parameter in the settings of the app and adjust the firmware so that the messages will be send in the old way. But then you loose the ability to adjust the throttle curve and PID settings via the app. Or it is necessary to send another message for these settings.
I will think about it.

But if you use the modules that i recommend then you do not have these issues.
So the standard setups of these modules seem to be different.
```

---
## \#941 Posted by: The_Dude Posted at: 2017-03-20T14:24:55.444Z Reads: 188

```
Hi @Ackmaniac,
I'm using the NRF-Controller of Vedder which ist adjusted in the Nunchuk tab. The driving mode for my eMTB is (or would be) watt + brake + reverse. Is it possible to select this mode via your app (can't find it in the menu selection). As always: appreciate your progress soooo much. THANKS!
```

---
## \#942 Posted by: Ackmaniac Posted at: 2017-03-20T14:28:28.605Z Reads: 192

```
Yes it works. But first you need a connection with the VESC via the App. then the app recognizes that the NRF or Nunchuk mode is active and it switches to these modes. If that doesn't work then please let me know. 
So long story short. The App detects by itself that you use a Nunchuk or NRF. But without a connection it can't detect it.
```

---
## \#943 Posted by: Plumb77 Posted at: 2017-03-20T15:19:48.986Z Reads: 185

```
Anyone know how to go about soldering this on and enertion vesc
```

---
## \#944 Posted by: The_Dude Posted at: 2017-03-20T15:56:08.111Z Reads: 186

```
Ok, then I have to give it another try. Current status: Dual VESC, Master uses NRF/Nunchuk, Slave has the BT successfully connected to the App. I see the values changing according to my throttle input - so the connection is working. But: Slave has only activated UART for the BT-Module, all other inputs are deactivated on the slave. Only the Master is connected to the NRF ... could this be the reason?
```

---
## \#945 Posted by: Ackmaniac Posted at: 2017-03-20T17:02:24.999Z Reads: 192

```
Let's have a Skype meeting this evening.
```

---
## \#946 Posted by: Ackmaniac Posted at: 2017-03-20T18:05:27.448Z Reads: 200

```
Ok i found the error. the check for NRF was wrong. New version is already in the dropbox link and in a couple of hours also in Google Play available. Thanks for the Report.
```

---
## \#947 Posted by: yaca Posted at: 2017-03-20T19:23:05.736Z Reads: 203

```
<img src="/uploads/db1493/original/3X/a/d/adc2e9babc949e1994af08e523518d6f639cc5a2.jpg" width="667" height="500">

At "Google Play Store" you will find with the app also a descripton how to connect.
```

---
## \#948 Posted by: Plumb77 Posted at: 2017-03-20T19:26:13.951Z Reads: 196

```
Do I need a special soldering device? I have a soldering pen and have only soldered wire never to a board. Can you send a pic of the back side of your vesc showing the pins and soldering?
```

---
## \#949 Posted by: yaca Posted at: 2017-03-20T19:35:44.770Z Reads: 191

```
You can see on the four wires where you have to solder. No special soldering device. If you don't know how to solder, for sure you will find some hints with google. Sorry I don't want to turn my vesc now, I'm busy right now and it is really no magic thing.
```

---
## \#950 Posted by: Fabian287 Posted at: 2017-03-22T13:11:53.308Z Reads: 190

```
I have also dual vesc. Master and slave. I also use my selfmade Nunchuck via Uart on my master vesc. So can i connect the Bluetooth module to my slave and it will work fine?
```

---
## \#951 Posted by: Maxid Posted at: 2017-03-22T13:14:17.466Z Reads: 187

```
Yes
10 characters
```

---
## \#952 Posted by: Fabian287 Posted at: 2017-03-22T13:33:01.808Z Reads: 186

```
So when i change some settings it will be changed on both vescs?
```

---
## \#953 Posted by: Ackmaniac Posted at: 2017-03-22T14:24:03.946Z Reads: 198

```
Yes but only when you are connected to the Master.
So if the bluetooth module is attached to the Slave you have to enable "Connect by CAN to ID" and select the Controller ID of the master like in the picture.
Because the master sends the new settings to all the slaves in the system. So that would also work for 4WD.

<img src="/uploads/db1493/original/3X/8/1/814e46780ef78a9d5f4da862dde100d733e53581.png" width="281" height="500">
```

---
## \#954 Posted by: Tuomalar Posted at: 2017-03-22T21:28:12.212Z Reads: 186

```
Some noob questions. Do i set vescs like Jacob firmware? And is that first post updated?
It's very hard to find CLEAR & SIMPLE instructions how to set vesc. @Ackmaniac
```

---
## \#955 Posted by: Ackmaniac Posted at: 2017-03-23T11:18:33.410Z Reads: 188

```
The positions of the parameter in the BLDC-Tool slightly changed. For example the Throttle Curve is in it's own tab now and not anymore in the PPM or Nunchuk tab.
```

---
## \#956 Posted by: kampfhahn Posted at: 2017-03-23T19:29:59.303Z Reads: 187

```
Just got myself a used Nexus 5 to test your app.

I set the mode to PPM+UART, baud rate is set to 9600, the bluetooth connection is established but there are no values in the app. I use the VESCs 5V port and the tx/rx ports are crossed.

I use [this](http://www.ebay.de/itm/172356090573?_trksid=p2060353.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT) HM10 controller.

Can anyone help?
```

---
## \#957 Posted by: Ackmaniac Posted at: 2017-03-23T19:35:13.722Z Reads: 185

```
Maybe make a picture of your wire connections to double check.
```

---
## \#958 Posted by: Maxid Posted at: 2017-03-23T19:36:09.080Z Reads: 184

```
firmware is updated to @Ackmaniac's version or are you still using the original one?
```

---
## \#959 Posted by: kampfhahn Posted at: 2017-03-23T19:37:31.386Z Reads: 176

```
Ackmaniac 2.53. Already enjoying the watt control mode :)
```

---
## \#960 Posted by: Lambjr088 Posted at: 2017-03-23T19:46:41.265Z Reads: 181

```
i have read the entire post  ALL OF IT! and i barely understood any of it does anyone know if there is a video on installing the modded bldc tool by ackmaniac and  how to flash the firmware not sure if it is for the vesc or something else? and how to set it up for beginners?  im a noob to all of this lol
```

---
## \#961 Posted by: kampfhahn Posted at: 2017-03-23T19:50:34.680Z Reads: 183

```
Wiring is definitely ok. I also tried to uncross the rx/tx ports but of course it didn´t help.

Strange thing is that i can use "VESC Connect" on my iPhone for accelerating/breaking. But the live data section is empty like in your app.
```

---
## \#962 Posted by: Ackmaniac Posted at: 2017-03-23T20:04:07.532Z Reads: 187

```
Seems that the Bluetooth module is setup with a different default configuration. To make thinks easy i can only recommend to buy the Bluetooth modules that I recommend. 
What could also help me is that you download this app and connect to the module and post the information you see via Screenshots here or by pm. 
https://play.google.com/store/apps/details?id=com.macdom.ble.blescanner
```

---
## \#963 Posted by: kampfhahn Posted at: 2017-03-23T20:39:15.386Z Reads: 183

```
Thanks, i´ll send you some screens i a second.

It´s really strange that accelerating/breaking is working with "BLDC Control" and the live data on both apps don´t. Maybe the rx-part of  the module is damaged. @Maxid did you also order your module in china? If not an ebay link to your module would be nice.
```

---
## \#964 Posted by: Maxid Posted at: 2017-03-23T20:42:36.886Z Reads: 181

```
I got it from a German ebay seller - the shop does not have it anymore unfortunately. With AT commands we should be able to get this running though. Try the app @Ackmaniac suggested to see what your BLE profiles look like.
```

---
## \#965 Posted by: kampfhahn Posted at: 2017-03-23T20:47:51.946Z Reads: 211

```
These are the screens that i´ve just sent @Ackmaniac
 
<img src="/uploads/db1493/original/3X/2/b/2b6eb4cc230b5a8327647ddb89337a100a291344.png" width="281" height="500"><img src="/uploads/db1493/original/3X/0/6/065108586736b9c8bc7afd23de1c6d5f5ca3fc56.png" width="281" height="500"><img src="/uploads/db1493/original/3X/e/9/e933f83ee48ee146cd1ddaf85d48e732c328daba.png" width="281" height="500"><img src="/uploads/db1493/original/3X/1/b/1b178f24b303d74088d9a79c46e5098050ad5dd7.png" width="281" height="500"><img src="/uploads/db1493/original/3X/4/1/41d15aabf624442269fdf7fc782a4b415db20518.png" width="281" height="500"><img src="/uploads/db1493/original/3X/e/1/e1acd18b4b1f9a0b2c2abe83c51cc2ec682556ba.png" width="281" height="500">
```

---
## \#966 Posted by: Maxid Posted at: 2017-03-23T20:50:34.384Z Reads: 178

```
that is a BT05 module - not HM10
http://www.martyncurrey.com/bluetooth-modules/
```

---
## \#967 Posted by: kampfhahn Posted at: 2017-03-23T20:55:27.573Z Reads: 184

```
[Ebay description](http://www.ebay.de/itm/172356090573?_trksid=p2060353.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT) claims it to be HM10. :confused:
```

---
## \#968 Posted by: Ackmaniac Posted at: 2017-03-23T20:58:12.527Z Reads: 183

```
Thx for the note. Your right.
```

---
## \#969 Posted by: Maxid Posted at: 2017-03-23T20:59:49.657Z Reads: 184

```
I'd say you got a free BT05 if you open a paypal dispute ;)

Edit: although in your case they already say that it is CC41-A based - which is a clone. When I ordered mine they even showed images with the oscillator on the board which is missing on the clones - thus I got a refund.
```

---
## \#970 Posted by: Maxid Posted at: 2017-03-23T21:07:54.430Z Reads: 191

```
I had the same issue
http://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286/291?u=maxid

try setting the Baud rate on the VESC to 115200 - that should solve it
```

---
## \#971 Posted by: kampfhahn Posted at: 2017-03-23T21:18:52.781Z Reads: 187

```
9600 should be ok for my module because when i change it to 115200 i can´t accelerate/break with VESC Connect anymore.
```

---
## \#972 Posted by: Maxid Posted at: 2017-03-23T21:20:35.310Z Reads: 188

```
then it is most probably your rx line - either not connected properly or damaged.
```

---
## \#973 Posted by: Ackmaniac Posted at: 2017-03-23T23:39:17.560Z Reads: 197

```
I read a bit more about your module and it seems that it is a clone of a clone.
Mine is a clone of the HM-10 and yours seem to be a clone of my clone.

http://blog.yavilevich.com/2017/03/mlt-bt05-ble-module-a-clone-of-a-clone/

Here are example pictures of the correct and the wrong module
**RIGHT****RIGHT****RIGHT**
<img src="/uploads/db1493/original/3X/4/5/45e84cbebd7ac2cf21b81af5cd24438a42feb92e.jpg" width="690" height="303">


**WRONG****WRONG****WRONG**
<img src="/uploads/db1493/original/3X/9/4/9442e7cf98f180e2545484cb6c9fcff6de23fd9a.jpg" width="690" height="309">


**RIGHT****RIGHT****RIGHT**
<img src="/uploads/db1493/original/3X/3/a/3aca216e4dfc213878c24dff1f9a93ff505e33bc.jpg" width="690" height="315">


**WRONG****WRONG****WRONG**
<img src="/uploads/db1493/original/3X/5/b/5b89192ca7bec53aa3c7756098a35b6beceec2ff.jpg" width="690" height="299">
```

---
## \#974 Posted by: Titoxd10001 Posted at: 2017-03-23T23:46:28.206Z Reads: 184

```
Do you have a tutorial on how to get started using your firmware and app. What connector can we use to connect Bluetooth module to vesc.
```

---
## \#975 Posted by: kampfhahn Posted at: 2017-03-24T07:32:45.030Z Reads: 184

```
There´s no really need for a tutorial if you are familiar with the origin BLDC tool. Just download ackmaniacs BLDC tool and Firmware, run the BLDC tool and use it to flash ackmaniacs firmware. Then you can choose watt mode, set a custom throttle curve and use the app.

The connector is called "JST-PH" with 2mm spacing either with 6 or 7 pins depending on your VESC Version. But you can also solder your wires directly to the pins on the opposite site of the VESCs jack.
```

---
## \#976 Posted by: Tuomalar Posted at: 2017-03-24T08:09:43.263Z Reads: 187

```
Where i can find that firmware? I downloaded BLDC for mac, but can't find any firmware.
```

---
## \#977 Posted by: bullrider12 Posted at: 2017-03-24T08:31:00.338Z Reads: 188

```
Have a look at the first post. There is a link to ackmaniacs dropbox folder. It contains the modified bldc tool and the firmware( something with .bin)

You can only use his firmware with the modified bldc tool.
```

---
## \#978 Posted by: Tuomalar Posted at: 2017-03-24T08:33:21.671Z Reads: 185

```
That's where i downloaded it but do i have to download this one too -> VESC_Ackmaniac_2_53_cruise_fixed.bin?
```

---
## \#979 Posted by: SeanHacker Posted at: 2017-03-24T08:33:58.494Z Reads: 189

```
Yes. That .bin is the firmware.
```

---
## \#980 Posted by: bullrider12 Posted at: 2017-03-24T08:39:20.578Z Reads: 190

```
Is there actually a mac version? Don't know if I'm blind, but I can't see a mac version of this tool :hushed:
```

---
## \#981 Posted by: SeanHacker Posted at: 2017-03-24T08:42:59.640Z Reads: 195

```
Yeah there is. 

<img src="/uploads/db1493/original/3X/6/6/66157d120b4daac9974152a914a930dd4ece4957.png" width="281" height="500">
```

---
## \#982 Posted by: bullrider12 Posted at: 2017-03-24T08:46:31.342Z Reads: 191

```
Nice, I need to update my Dropbox asap. :grinning:

Thanks!
```

---
## \#983 Posted by: Eboosted Posted at: 2017-03-24T21:34:17.327Z Reads: 189

```
@ackmaniac if I select a mode in VESC Monitor Define Max Watt is ticked again automatically, even though I deselected it via USB  BDC tool?

<img src="/uploads/db1493/original/3X/3/a/3a76d62e07d1b423f84cb250ef73eb666f81e171.png" width="681" height="108">
```

---
## \#984 Posted by: Ackmaniac Posted at: 2017-03-24T21:40:19.221Z Reads: 188

```
Yes you are right. In the new version of the firmware there will be no max watt value anymore. So I am not going to fix this. I am working on the watt with reverse function and I am very happy with the result. So I hope I can release the new version this weekend.
```

---
## \#985 Posted by: kampfhahn Posted at: 2017-03-24T21:43:12.941Z Reads: 183

```
But isn´t the max watt value essential to set up beginner modes for example?
```

---
## \#986 Posted by: Pimousse Posted at: 2017-03-24T22:07:46.494Z Reads: 182

```
Oh, it's a good point you mentioned !
I also define a very low max watt for the beginner mode.
```

---
## \#987 Posted by: Ackmaniac Posted at: 2017-03-24T22:10:05.823Z Reads: 184

```
It will be adjustable via the battery max. So if you have a 10s4P and want a power output of around 250W then you have to set 250W / 36V =7A for battery max.
```

---
## \#988 Posted by: Eboosted Posted at: 2017-03-25T06:10:33.044Z Reads: 186

```
I'd like that more than max watt, one less thing to worry about. When is the new version coming out?
```

---
## \#989 Posted by: rwxr Posted at: 2017-03-25T08:01:10.196Z Reads: 191

```
I have tried installing this firmware on two different maytech 4.12 VESC.

When I hit the upload button it uploads the firmware, then I get "unknown error" in the bottom right of BLDC Tool and the VESC becomes unresponsive and I have to reboot it by cutting the power. After reboot, it still has the 2.18 FW.

Am I missing something here?
```

---
## \#990 Posted by: kampfhahn Posted at: 2017-03-25T08:28:24.855Z Reads: 187

```
Are you using @Ackmaniac s BLDC tool?
```

---
## \#991 Posted by: PXSS Posted at: 2017-03-25T09:23:05.080Z Reads: 193

```
I disagree with getting rid of max power. 
40V * 50A = 2000W
36V * 55.5A = 2000W
30V * 66.6A = 2000W

Setting a max current is not the same as a max power. 

IMO. Power (Watt) control should seek a power condition and not a current condition at a specific voltage, otherwise what is the difference???

If I can set max power, and have the throttle be mapped from 0-max power then that would be ideal. The max battery current is for safety reasons. In my opinion it should be set once and never change and always override any other setting.
```

---
## \#992 Posted by: rwxr Posted at: 2017-03-25T11:37:06.664Z Reads: 180

```
Yes  (10char)
```

---
## \#1000 Posted by: Ackmaniac Posted at: 2017-03-25T12:34:26.265Z Reads: 197

```
There is still a difference. I make this because of different reasons. First of all i want to get rid of max watts because people mostly didn't really understand how to use it and it makes the code much more complicated. Secondly it works great when the max power is calculated by the actual battery voltage in combination with max amps. Because if you set the max watts to the calculation 36V * 30A = 1080W for a 10S battery then you loose throttle range when the battery is below 36V at 30A. All in all i want to have make it easier.

You won't get a precise watt output anymore but it makes it easier for me to provide the same power to the motors. And it gives me the possibility to setup different power output for the front and rear axle. So 4WD and Dual diagonal will have a big benefit from that. It's possible for example to use 30% at the front and 70% power at the back and for the brake 70% at the front and 30% at the back.
At the moment that isn't possible via CAN because the motors get the same current signal.

But i will give it second thought.

I see the chance to keep max watts but that would involve lot's of programming again and it give a higher chance for messing around with the setup.
```

---
## \#1001 Posted by: PXSS Posted at: 2017-03-25T13:13:10.426Z Reads: 215

```
[quote="Ackmaniac, post:1000, topic:12286"]
First of all i want to get rid of max watts because people mostly didn't really understand how to use it
[/quote]

No reason to cap the ability of your app just because people don't know how to use it! We would still be using rc ESCs if we limited ourselves to what we know how to use already...

[quote="Ackmaniac, post:1000, topic:12286"]
Secondly it works great when the max power is calculated by the actual battery voltage in combination with max amps. Because if you set the max watts to the calculation 36V * 30A = 1080W for a 10S battery then you loose throttle range when the battery is below 36V at 30A. All in all i want to have make it easier.
[/quote]

This is not a max power setup, it's a max current setup. If you set your max current to 30A then you get this:
40v * 30A = 1200W
36v * 30A = 1080W
30v * 30A = 900W
So throughout the trip you get less and less power of you hold full throttle. That means you loat 25% power from full to empty. 

Lets now assume you control power. Max power set at 1200W. 
1200W / 40V = 30A
1200W / 36V = 33.3A
1200W / 30V = 40A
Regardless of the voltage of your battery, you get the same power if you hold full throttle. This means that you don't need to adjust how much throttle you use on the same incline road as the battery discharges.

Now if your battery can only do 30A max for safety reasons then you get the same response as the current control mode since the max amps overrides. 

If your battery can do 60A and you're trying to do a beginner mode, the current control will have a varying max power as the battery discharges, whereas a power control would have the same max power throughout the whole range. 

---

The reason most rc escs use current control is because the discharge curve for LiPos is really flat 3.75v-3.65v from 10-80% used capacity with the drop being really pronounced near 90% used capacity but even then high end escs like kontronik Jives have a power control mode in which they do exactly what I described above but it comes at a really steep price. 

This isn't so great for Li-ions since the discharge curve has a constant slope from 3.9v to 3.2v from 10-85% used.

---
As for the 4wheel drive scenario, you would just offset your max power on the vescs. They get a throttle command from 1000pwm-2000pwm from the receiver. All you need is to pass that through the canbus. 

Rear ESC power limits: max 700W, min -300W
Front ESC power limits: max 300W, min 700W

10% throttle = 30W at front, 70W at rear. 
50% throttle = 150W front, 350W rear. 
100% throttle = 300W front, 700W rear
```

---
## \#1002 Posted by: Ackmaniac Posted at: 2017-03-25T15:31:23.295Z Reads: 197

```
Now you convinced me to add it again. 10 hours more work. Your lucky the the 96 30Q cells for my 12S8P haven't arrived yet.

But it will work a little different and should only be used by advanced users who know what they are doing. Because you have to set it up for each motor. Also if you want to have a equal power output.
```

---
## \#1003 Posted by: PXSS Posted at: 2017-03-25T15:59:11.826Z Reads: 189

```
Hehe. Sorry...
(Not really, I really really want power control)

Btw, is it a PID controller? Is there a way to adjust individual gains???
```

---
## \#1004 Posted by: rwxr Posted at: 2017-03-25T16:23:00.848Z Reads: 192

```
@Ackmaniac: Any idea why I get "unknown error" in your version of BLDC-Tool when uploading your firmware?
After upload it should reboot but it doesn't and when I manually reboot it still has FW 2.18.
```

---
## \#1005 Posted by: Ackmaniac Posted at: 2017-03-25T18:10:48.913Z Reads: 193

```
Where did you get your VESC from. Maybe the bootloader is missing. Best is you make a video it.
```

---
## \#1006 Posted by: rwxr Posted at: 2017-03-25T19:37:26.406Z Reads: 192

```
It's a maytech. It currently had fw 2.18 and it's working. 
It's just updating fw that's not working. I'll see if I can make a video tomorrow
```

---
## \#1007 Posted by: Ackmaniac Posted at: 2017-03-25T19:39:12.245Z Reads: 192

```
I think the maytech VESCs have no bootloader installed. So you need a programmer. there is more info on vedders website www.vedder.se
I don't really understand why so many buy the maytech VESCs in the last days.
```

---
## \#1008 Posted by: rwxr Posted at: 2017-03-25T19:45:54.117Z Reads: 198

```
I'll get a stlink and test, thanks for the info. 
Market is flooded with maytech parts so they are easy to obtain
```

---
## \#1009 Posted by: TarzanHBK Posted at: 2017-03-25T23:15:51.864Z Reads: 199

```
Cheapest on the market!
```

---
## \#1010 Posted by: Eboosted Posted at: 2017-03-26T05:51:08.060Z Reads: 199

```
BTW where are you guys getting your Maytech VESCs from in the USA?
```

---
## \#1011 Posted by: halifax21 Posted at: 2017-03-26T09:06:25.401Z Reads: 201

```
I've orderd mine from http://m.ebay.com/itm/302200711613?_mwBanner=1 (3)
So far 1 has a problem with getting info from the receiver
```

---
## \#1012 Posted by: Eboosted Posted at: 2017-03-26T15:12:56.613Z Reads: 211

```
Well the one @halifax21 pointed is not the cheapest in the market it has the same price than @torqueboards

@halifax21 is this VESC for your tramps build?
```

---
## \#1013 Posted by: halifax21 Posted at: 2017-03-26T15:51:02.500Z Reads: 205

```
Correct a mundo
```

---
## \#1014 Posted by: Tuomalar Posted at: 2017-03-26T19:35:50.799Z Reads: 215

```
Hi
I'm in really deep problems with vesc configuration. Can somebody tell me straight forward guidelines how do i setup my vescs. I bought two Enertion's vescs with 4.18 firmware. I connected first vesc and updated it to Ackmaniac's firmware, but i don't have no idea what i should do next. I just can't find any good instructions. 
And i'm going to run dual 6355 via canbus with 10s4p (25R cells).

EDIT: I ended up with this. Does these settings work? 
<img src="/uploads/db1493/original/3X/c/2/c2324a2eeb4fe4b2f7ebfb4ac7c37fdb822129de.png" width="690" height="446"><img src="/uploads/db1493/original/3X/7/7/7754e844d5154a68327052ac176bf0fb0390e74a.png" width="690" height="446">
<img src="/uploads/db1493/original/3X/1/4/145c387e7a551b22a89174191318a5c0e90b3edc.png" width="690" height="430"><img src="/uploads/db1493/original/3X/1/4/1497ee97ba48a081c6c259dafe22dd2718c25574.png" width="690" height="426"><img src="/uploads/db1493/original/3X/e/6/e62a9ab5df1171b79514f5f73d0c9867a436c099.png" width="690" height="426">
```

---
## \#1015 Posted by: Ackmaniac Posted at: 2017-03-26T20:32:57.712Z Reads: 183

```
That looks good.
You should set your batter cutoff strat to 30V and your cutoff end to 28V.
And you need to adjust the PPM pulsewith values. But for that you can use the wizard. just click on it and follow the instructions. But disable the control mode fisrt by choosing "Disabled" and write the configuration. Afterwards you can activate it again.
```

---
## \#1016 Posted by: Tuomalar Posted at: 2017-03-26T20:35:39.360Z Reads: 186

```
I'll do that. Any idea why second vesc show me blue and red light at same time?
```

---
## \#1017 Posted by: Ackmaniac Posted at: 2017-03-26T20:51:34.056Z Reads: 190

```
At the Slave VESC you have to activate "Send status over CAN" and set the Controller ID to 1.
```

---
## \#1018 Posted by: jmasta Posted at: 2017-03-27T01:01:20.666Z Reads: 191

```
[quote="Ackmaniac, post:973, topic:12286, full:true"]
**RIGHT****RIGHT****RIGHT**
<img src="/uploads/db1493/original/3X/3/a/3aca216e4dfc213878c24dff1f9a93ff505e33bc.jpg" width="690" height="315">
[/quote]

If anyone wants to buy this BT module, please PM me.  I just checked and I have this exact one.  But it's not very useful for me since I have an iPhone and can't use Ackmaniac's cool app
```

---
## \#1019 Posted by: jmasta Posted at: 2017-03-27T01:04:33.431Z Reads: 188

```
For anyone with experience with both, why do you prefer **Watt Control** over **Current Control**?
```

---
## \#1020 Posted by: makevoid Posted at: 2017-03-27T01:16:34.646Z Reads: 193

```
I haven't tried the firmware and watt control mode yet (but I will soon when I get some free time) but the primary feature (as far as I understand) is to be able to **control acceleration** (and braking) **more precisely** at mid-high speed - also you can draw the acceleration/braking curve which basically let you tune them as you want

also you will have no difference of the acceleration/braking at different voltages (between when your battery is fully charged and when it's almost at the cutoff)

then in the firmware there are a lot of features (better traction control and cruise control) and the integration with the android app so you can log your ride and it gets the data from all the vescs which is:  <img src="/uploads/db1493/original/3X/f/4/f4a344da968eed5fd36c003afc21a5d627c2c769.gif" width="80" height="80">
```

---
## \#1021 Posted by: jmasta Posted at: 2017-03-27T06:30:23.347Z Reads: 183

```
A cheap Android phone can be found for about $20 (maybe free).  How well would this work to exclusively run this app?  It would have no cell service, but you could feed it internet through a wifi tether if needed
```

---
## \#1022 Posted by: The_Dude Posted at: 2017-03-27T07:31:12.121Z Reads: 183

```
Works perfect for me - I'm using an old LG Spirit 4G only for this purpose, no cell service. Big advantage: doesn't matter that much if you hit the ground with your smartphone.
```

---
## \#1023 Posted by: yaca Posted at: 2017-03-27T18:40:31.479Z Reads: 180

```
So far as I know If you want to use the video function you need at least android 5.0.
```

---
## \#1024 Posted by: kampfhahn Posted at: 2017-03-27T18:55:02.355Z Reads: 175

```
If you normally use an iPhone i´d recommend getting a Google Nexus (model depending on your max. price). They run stock Android without ugly oem-themes or tons of bloatware. There´s also a huge community providing new versions etc.
```

---
## \#1025 Posted by: SeanHacker Posted at: 2017-03-27T18:59:52.110Z Reads: 183

```
Anyone that buys a cheap android phone or just needs to bring their device up to date just have a look here http://aokp.co/devices/. We support a ton of devices. Our main server is down for maintenance at the moment but you can use these links to check for your device https://sourceforge.net/projects/aokp-nougat/files/ or http://xfer.aokp.co/?developer=AOKP. This will bring the device up to 7.1.1 Nougat. I'll help anyone that needs it.
```

---
## \#1026 Posted by: jaykup Posted at: 2017-03-27T20:09:55.009Z Reads: 188

```
Is AOKP a light-weight version of an AOSP rom or is it modified Cyanogenmod?

I have a USC S4, jflteusc - I think this is the link but it looks like 4.2?  Do you have 5.1? 

http://xfer.aokp.co/?developer=AOKP&folder=jflteusc

Running CM12.1, but the bluetooth is a little buggy and the screen doesn't always turn off correctly.
```

---
## \#1027 Posted by: SeanHacker Posted at: 2017-03-27T20:16:22.480Z Reads: 187

```
CyanogenMod is dead. It's now LineageOS. We do track some repos from LineageOS because it's easier than having to update on our own and they take care of all the CAF merges and rebases. I just checked and it looks like we don't have a maintainer for the JF devices so it ended up dying on JellyBean. I still have an s4 (att) that I can get setup and build a unified device tree (bringup to 7.1.1) for if you'd like me to. Shouldn't take too long. I'll build on my personal machine tonight and then merge into our repos. I'll shoot you a pm later after I've tested it.
```

---
## \#1028 Posted by: Plumb77 Posted at: 2017-03-27T23:03:30.553Z Reads: 185

```
Does this work with vescx?
```

---
## \#1029 Posted by: Ackmaniac Posted at: 2017-03-27T23:10:57.914Z Reads: 194

```
Better than the standard VESC.
```

---
## \#1030 Posted by: Lambjr088 Posted at: 2017-03-28T05:43:52.772Z Reads: 191

```
So this won't work with maytech Vescs?
```

---
## \#1031 Posted by: Ackmaniac Posted at: 2017-03-28T06:06:58.601Z Reads: 189

```
It works also with the maytech. But they don't have a bootloader installed so you will need a programmer to install a new firmware.
```

---
## \#1032 Posted by: Lambjr088 Posted at: 2017-03-28T07:29:37.581Z Reads: 192

```
Now that's something way out of my skills lol
```

---
## \#1033 Posted by: Maxid Posted at: 2017-03-28T07:30:30.531Z Reads: 194

```
http://www.electric-skateboard.builders/t/vesc-installing-a-bootloader/752
```

---
## \#1034 Posted by: Lambjr088 Posted at: 2017-03-28T07:39:35.246Z Reads: 186

```
I read. The first 2 paragraphs and it might as well be written in an ancient language lost to time beacuse i didnt get it. All this programming is beyond me and this is where the "if i was rich" line would come in and just pay someone to do this for me lol hahaha
```

---
## \#1035 Posted by: Maxid Posted at: 2017-03-28T07:40:50.358Z Reads: 187

```
Well that is the price you pay for getting a Maytech VESC ;)
```

---
## \#1036 Posted by: Lambjr088 Posted at: 2017-03-28T07:41:34.104Z Reads: 183

```
Yea thats true go on a budget and you get what you paid for lol
```

---
## \#1037 Posted by: Lambjr088 Posted at: 2017-03-28T07:45:16.964Z Reads: 186

```
Does anyone have a "bootloading for dummy's" available? Ok serious question. Does anyone know why they do that with maytech vescs? And where can i purchase a vesc that has this done to already?
```

---
## \#1038 Posted by: treenutter Posted at: 2017-03-28T13:03:13.925Z Reads: 190

```
@Lambjr088 Installing a bootloader adds a step at the factory, so they can cut production time (and therefore cost) by skipping it. Or, they might have *intended* to install one but it failed. If users can't easily upload or modify the firmware, it makes it easier for the manufacturer to provide technical assistance because everyone will be using the same software platform. But in the case of MayTech, I'm guessing it's to reduce cost.

The thread @Maxid referenced above describes a problem that most people wouldn't have; the weirdly-lablelled programmer I ended up with. All of the script you need to install a bootloader is already written by Vedder, so you can cut-and-paste everything to get it done. You'd just need a programmer ($12usd) and some version of Linux.

If you decide to give it a try, I'm happy to help you out!

If all of that seems way too tough, I believe that all of the main VESC vendors ship with boot loaders installed (Ollinboards, DIYES, Enertion, Esk8.de, sorry if I've missed anyone).
```

---
## \#1039 Posted by: Lambjr088 Posted at: 2017-03-28T19:37:20.036Z Reads: 180

```
I did not know it was cut and paste. Thats awesome do you know where we can find that? Links?
```

---
## \#1040 Posted by: flatsp0t Posted at: 2017-03-28T19:55:38.273Z Reads: 179

```
Go to http://vedder.se/2015/01/vesc-open-source-esc/ and scroll sown to the "Download, Compile and Upload the Bootloader" section.
```

---
## \#1041 Posted by: Lambjr088 Posted at: 2017-03-28T20:08:38.935Z Reads: 180

```
U guys r life savers. Thank you
```

---
## \#1042 Posted by: Eboosted Posted at: 2017-03-29T05:15:25.892Z Reads: 196

```
After months riding my board on BLDC with @ackmaniac firmware with zero issues, I tested FOC today for the first time, holy sh!it this thing is smooth!

However, I had an issue, one motor stopped responding at full throttle (several times) giving me crazy wobbles, it felt like it disconnected and connected back again, I guess VESC resetted itself due overcurrent, it never happened to me before on BLDC mode.

Here is the log:
[img]http://i.imgur.com/RsqTqgT.jpg[/img]

Here are the errors:
[img]http://i.imgur.com/9NCVrLz.png[/img]
[img]http://i.imgur.com/3OPGsTz.png[/img]

An overcurrent followed by dreaded DRV8302,however after the disconnection board worked again perfectly.

I guess FOC is still not safe to use after all
```

---
## \#1043 Posted by: Ackmaniac Posted at: 2017-03-29T06:40:08.106Z Reads: 184

```
You should not continue in FOC. Otherwise the VESC will be killed very soon. I had the same problems and also a bad crash at 40 km/h when one of the motors were cutting out. With my Vesc-X I can do whatever I want with my motors in FOC. Never had any error. Not even when I tried my changes for the firmware development and had some bugs which let the motor do crazy stuff.
```

---
## \#1044 Posted by: Eboosted Posted at: 2017-03-30T16:49:53.824Z Reads: 187

```
I wonder what I did wrong, I installed an HM-10 yesterday on my second board, I'm able to read all parameters but I'm not able to switch modes, it always selects "default" even though I click on different modes. I used baud rate 9600, 115200 won't even connect with the app.

[img]http://i.imgur.com/bVAUz6h.png[/img]

On the other hand, as you can see on the faults, I'm getting ABS over current fault, it happened when trying to launch from stand still at only 25% throttle.

I wonder if it might have been related to this setting, as I set it to 0.030

[img]http://i.imgur.com/vSVJmTs.jpg[/img]
```

---
## \#1045 Posted by: SageTX Posted at: 2017-03-31T00:18:40.825Z Reads: 182

```
Probably the _wrong_ module. I have the same issue.  
Start here -  

http://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286/926?u=sagetx
```

---
## \#1046 Posted by: Eboosted Posted at: 2017-03-31T02:03:32.788Z Reads: 186

```
The first module I purchased for my old board works perfectly
```

---
## \#1047 Posted by: SageTX Posted at: 2017-03-31T02:39:32.227Z Reads: 189

```
Did you update the firmware on the old board?  After the updates to include throttle curves in the app is when I started having issues with mine
```

---
## \#1048 Posted by: SeanHacker Posted at: 2017-03-31T06:19:03.245Z Reads: 197

```
Nice. Zoom in on the performance phone app :slight_smile:
 
<img src="/uploads/db1493/original/3X/4/b/4b82a34618f476b706d26d3a684240ad256f3086.png" width="281" height="500">
```

---
## \#1049 Posted by: Eboosted Posted at: 2017-03-31T06:35:16.450Z Reads: 191

```
Is enertion at least paying @ackmaniac to use his software? Hope so, otherwise it won't be ethical
```

---
## \#1050 Posted by: Ackmaniac Posted at: 2017-03-31T08:10:30.215Z Reads: 196

```
Is there anybody who has a Dual Diagonal Drive or a 4WD where all VESCs are connected by CAN and uses my firmware mod.
Because i want to know if my new firmware mod improves the acceleration and brake behavior of those boards.
```

---
## \#1051 Posted by: guyguy Posted at: 2017-03-31T13:53:06.472Z Reads: 204

```
What does the new firmware do? 

I've noticed the slave lags on acceleration.
```

---
## \#1052 Posted by: Ackmaniac Posted at: 2017-03-31T13:55:09.548Z Reads: 210

```
What do you mean exactly by lags on acceleration?
```

---
## \#1053 Posted by: guyguy Posted at: 2017-03-31T14:02:07.861Z Reads: 214

```
I had the belt break on the back drive (master) and was only on the front drive (slave) during a ride - that's when I was able to notice it, otherwise it's a bit hard to tell. There was a noticeable delay on trigger pull vs motor response when I was only on the front motor. I'm not sure if this was due to traction control or something else (back motor was spinning freely) and the it just felt a little slower in acceleration than with the only the master enabled.
```

---
## \#1054 Posted by: Ackmaniac Posted at: 2017-03-31T14:09:35.443Z Reads: 211

```
that is a exceptional case where the traction control has a hard time and of course you have less grip on the front so you could not accelerate as hard as if the motor is in the back.
more interesting to me is to have 30/70 acceleration power and 70/30 brake power. Because it is easy for the front wheel to slip during acceleration. And the Backwheel can easily slip during braking.
So i think it would make sense to have a different power delivery to each axle.
```

---
## \#1055 Posted by: guyguy Posted at: 2017-03-31T14:15:23.983Z Reads: 205

```
When you say different power delivery - do you want me to test vesc settings that reflect the 30/70 : 70/30 - Front/Back?
```

---
## \#1056 Posted by: Ackmaniac Posted at: 2017-03-31T14:28:17.402Z Reads: 200

```
Exactly. But this can only be achieved by the new version which I haven't released yet. But if you want test it let me know.
```

---
## \#1057 Posted by: Paulf Posted at: 2017-04-04T11:09:16.994Z Reads: 200

```
I'm having the issue where the app can collect data but can't properly set modes (sometimes works once out of 20 tries) has one of you guys found a solution for this problem?  
@Ackmaniac , you talked about maybe adding a parameter to send data the "old way " and sacrifice throttle curve data... I think that would be pretty cool for some of us having what seems to be Hm10 clones... :smile:

Btw: amazing software man, both the Android app and the molded firmware
```

---
## \#1058 Posted by: Ackmaniac Posted at: 2017-04-04T11:25:42.971Z Reads: 203

```
I think i managed to get the mode change working also on the other HM-10 modules, But this requires changes in the firmware and in the app. I hope i can release the new version in this week. But by the tests it looks very good. When i am closed than 5 meters to the board it workes more or less every time.
```

---
## \#1059 Posted by: Paulf Posted at: 2017-04-04T11:36:40.487Z Reads: 204

```
Cool! That's good news, thank you for your work
```

---
## \#1060 Posted by: Eboosted Posted at: 2017-04-04T15:54:06.806Z Reads: 207

```
Awesome, I hope it works on all HM-10 versions, the last one I got does not work for changing modes, only the first one for most other board
```

---
## \#1061 Posted by: SeanHacker Posted at: 2017-04-05T19:44:10.195Z Reads: 199

```
I'm bumping this thread only because it's my favorite here. Thanks for all the work you've done here @Ackmaniac. It made my entrance to esk8'ing way better than it would have been without.
```

---
## \#1062 Posted by: The_Dude Posted at: 2017-04-08T21:28:11.516Z Reads: 197

```
FW2.53 & HW4.7 - @Ackmaniac I compiled your FW for my VESCs 4.7 that I use for my eTrampa featuring Nowind. So far I only bench tested the setup but it works fine, as expected! Ready for some offroad stuff with ampere footage.
Nevertheless I discovered something new: when I push the button for cruise control at stilstand a small amount of duty cycle (less than 1%) is applied and the wheels start to turn very slow in a steady state. As far as I remember, this was not the case with FW2.18 and it is also not the case with my longboard  running FW2.53. Stillstand stays stillstand if only the cruise control button is pressed. Anyone else having the same issue? Ideas?
```

---
## \#1063 Posted by: Ackmaniac Posted at: 2017-04-08T22:06:52.634Z Reads: 194

```
You should also bet test my new firmware mod 2_54. In PPM it works very nice. For the Nunchuk i think that i also works as expected bit i need somebody to verify. It also would be awesome if you can compile it again for OSX.
```

---
## \#1064 Posted by: The_Dude Posted at: 2017-04-08T22:09:28.079Z Reads: 193

```
For sure!
10 chars
```

---
## \#1065 Posted by: Plumb77 Posted at: 2017-04-09T02:34:09.042Z Reads: 190

```
Sorry newb with all of this. Is there anyway to download the firmware through osx? Also is there kind of a step by step process to set this up I just got my vescx. Thanks in advance
```

---
## \#1066 Posted by: Ackmaniac Posted at: 2017-04-12T07:53:28.760Z Reads: 198

```
## UPDATE

I released my new Firmware Mod **Version 2.54**. I updated the first post where i explain what changed. So please read it completely before you upgrade.
```

---
## \#1067 Posted by: Maxid Posted at: 2017-04-12T08:09:29.713Z Reads: 198

```
You should also mention that we can now switch the C and Z buttons on the nunchuck :heart_eyes:
```

---
## \#1068 Posted by: ekitesurfer Posted at: 2017-04-12T09:19:18.459Z Reads: 197

```
When I try to open up the new bldc tool on ubuntu it does not do anything. Anyone have any advice?
```

---
## \#1069 Posted by: Ackmaniac Posted at: 2017-04-12T09:30:58.539Z Reads: 197

```
You have to build it.
```

---
## \#1070 Posted by: Ackmaniac Posted at: 2017-04-12T11:33:09.441Z Reads: 207

```
The app is also already adapted to the new Version. But i will create a new thread to explain the features in more detail and how to use it. 
Hopefully it workes now with all bluetooth modules. But you need the new Firmware file for that. If you test it with the old firmware you won't see a difference. 
We made tests with Bluetooth modules that had problems and could fix the issues. In the new one the timing for the incoming messages changed a little which should fix the issue. Also the possibility of lost settings on the VESC should not exist anymore.

The biggest change in the app that a lot of you will notice is the possibility to setup different settings for the front axle in case you have a Dual Diagonal or a 4WD. For all others just simply don't enable that option.
Also when you create a new mode it will take the last default settings as basis parameters which should make the setup easier.
```

---
## \#1071 Posted by: jacobbloy Posted at: 2017-04-12T13:21:40.966Z Reads: 201

```
hey guys, i am going to try and make some install builds for the latest version of the extended BLDC TOOL ASAP.
if it is needed. if not its all cool. just when every there is a stable build that you want done i will do it and post the google drive links.
```

---
## \#1072 Posted by: bullrider12 Posted at: 2017-04-12T13:35:47.242Z Reads: 199

```
Hey Ackmaniac,

I would like to say thank you for your effort in improving this BLDC-Tool.
With the  new upgrade everything works flawlessly. Now I can drive through the city with 6 km/h :joy:
```

---
## \#1073 Posted by: Ackmaniac Posted at: 2017-04-12T13:38:49.027Z Reads: 194

```
Glad that your happy with your 6 km/h limit.:joy:
```

---
## \#1074 Posted by: Maxid Posted at: 2017-04-12T13:41:02.062Z Reads: 196

```
maybe we should use the nunchuck Z button to unlock speed instead of having the reverse function ;)

Actually - is there a way to, let's say, have the VESC fallback into the 6km/h mode as soon as the remote disconnects? that would be super stealthy if the police ever stops you while you are in the fast mode.
```

---
## \#1075 Posted by: Ackmaniac Posted at: 2017-04-12T13:45:35.558Z Reads: 194

```
That would be hard to identify because the receiver sends a default signal when it looses connection. So for the VESC it looks like everything is ok. But it depends on the receiver. If you have a on off switch instead of a loop key it should be easy to switch back to default.
```

---
## \#1076 Posted by: Eboosted Posted at: 2017-04-12T16:05:05.125Z Reads: 194

```
@Ackmaniac is there a way to update your firmware via bluetooth via the HM-10 module?
```

---
## \#1077 Posted by: Ackmaniac Posted at: 2017-04-12T16:09:19.320Z Reads: 197

```
No. And I also think it will cause issues because of the 20 Byte restriction of Bluetooth low energy. For 200 Kb you need to send 10000 individual packages. And if one of them is missing the upload would fail. And you also need to adjust the settings after you flashed the firmware.
```

---
## \#1078 Posted by: bullrider12 Posted at: 2017-04-12T16:19:09.547Z Reads: 199

```
If I want to drive it with 6 km/h. What settings would you suggest me? The actual setting is:

Motor Max: 50 A
Motor Min: -50A
Batt Max: 40 A
Batt Min: -12 A
Watt max: 250 W with 6 km/h

When I reach that speed limit there is a srange noise coming from the motor. It sounds like "I want to drive faster, but im limited" :grin:
```

---
## \#1079 Posted by: Ackmaniac Posted at: 2017-04-12T16:24:28.036Z Reads: 201

```
I would limit the Motor max to 20A or even less and the max watts to 75 watts if you have a dual drive. It should be that low because when the motor is slower than 6 km/h it trys to accelerate to full speed immediately. But you wnat it to be soft in this case. Otherwise it always switches between full power, minimal power, full power, minimal power. It has a ramping in between so the best would be to set the ERPM limit start in the PPM settings to 0 or 1000 ERPM and the end to a the speed where you reach 6 km/h. This way it ramps slowly.
The Battery min and motor min should be as always because you still want strong brakes.
```

---
## \#1080 Posted by: bullrider12 Posted at: 2017-04-12T16:26:31.093Z Reads: 203

```
Nice, thank you. I will try that out :)
```

---
## \#1081 Posted by: Titoxd10001 Posted at: 2017-04-13T16:04:21.110Z Reads: 205

```
Is there a way to set reverse so that when you press the brakes it doesn't go to reverse automatically when rpm is low enough, like double tapping brakes to go backwards. Also is there a way to set up max watt for reverse for example on car ESCs I can set to 25% of total power.
```

---
## \#1082 Posted by: Ackmaniac Posted at: 2017-04-13T17:33:10.331Z Reads: 207

```
A max watt limit for reverse isn't there. But with a nice throttle curve it shouldn't be a issue.
And there is the possibility with the double reverse. It is a new feature of the newest version of the Mod. It is described in the first post of this thread. 

[quote="Ackmaniac, post:1, topic:12286"]
Watt (also exists for Nunchuk)"Watt" Control Mode works like "Watt no reverse with Brake" with the difference that you also have a reverse. The only problem with the standard reverse function is that when you brake hard the wheels can start to spin backward while you still move forward..To avoid that i added the parameters "Enable maximum ERPM for direction switch". ........
[/quote]
```

---
## \#1083 Posted by: Titoxd10001 Posted at: 2017-04-13T17:53:31.736Z Reads: 207

```
I downloaded the firmware​ yesterday and put it in watt mode and on the bench the brakes went straight to reverse. Let me try it again

Okay I'll adjust throttle curve. I only need reverse to bring the board back to me, don't need to go 30mph in reverse.
```

---
## \#1084 Posted by: Ackmaniac Posted at: 2017-04-13T18:46:15.008Z Reads: 196

```
Just read the first post in this Thread. There i explain how to setup reverse so that you have to brake twice for reverse. And if you want that the board comes back then just simply only use a little throttle.
```

---
## \#1085 Posted by: Titoxd10001 Posted at: 2017-04-13T23:27:50.409Z Reads: 201

```
Okay, thanks forgot to check the box for max erpm for direction switch. My main concern for not having a max watt for reverse is if I lend the board to someone I'm pretty sure they're going to launch it in reverse. I still do that sometimes in my car esc, but max speed is 5mph since I can set it to 25% power.
```

---
## \#1086 Posted by: jbruce Posted at: 2017-04-14T02:24:28.150Z Reads: 202

```
I think the question is if you limit the max watt normally, will it also limit it in the reverse direction.
```

---
## \#1087 Posted by: The_Dude Posted at: 2017-04-14T07:43:25.255Z Reads: 198

```
Hi Ackmaniac,
do you think, it's possible to add the "Enable maximum ERPM for direction switch" option also for Nunchuks?
```

---
## \#1088 Posted by: Ackmaniac Posted at: 2017-04-14T08:18:41.614Z Reads: 200

```
You mean you want to get rid of the reverse button and just press the brake twice instead? I think the reverse button is more advanced. One thing that is nicer in ppm is the ability that when you move already quick in the reverse direction you don't need to press anything. That is good for tricks where you do 180s withe the board.
```

---
## \#1089 Posted by: The_Dude Posted at: 2017-04-14T09:01:01.538Z Reads: 201

```
No, keep the reverse button but as a safety feature when riding at higher speed. Just an add on, sort of deactivate the reverse button above a certain erpm treshold. Do you think this would make sense?
```

---
## \#1090 Posted by: Maxid Posted at: 2017-04-14T09:08:58.552Z Reads: 205

```
Doesn't the VESC do this already? I am pretty sure I have already accidentally hit the reverse button and the VESC did not try to go backwards while going forward - but I might be wrong here.
```

---
## \#1091 Posted by: The_Dude Posted at: 2017-04-14T09:18:03.769Z Reads: 207

```
Benjamin showed that it works on the workbench - nice feature for copters when you reverse from full throttle in one direction to the other. I don't have the balls to try it in full speed on the road - maybe you will give it a try 😇
```

---
## \#1092 Posted by: jaykup Posted at: 2017-04-14T13:55:04.387Z Reads: 211

```
Any way to have the android app show total distance traveled when reviewing the recorded logs?  Right now it shows total time.
```

---
## \#1093 Posted by: Maxid Posted at: 2017-04-14T15:44:36.354Z Reads: 215

```
theres should be a distance column
```

---
## \#1094 Posted by: jaykup Posted at: 2017-04-14T16:01:06.899Z Reads: 220

```
This is all I see - is it somewhere else?

<img src="/uploads/db1493/original/3X/5/5/5523a2450c5a5b4395d1a80e98939ad663479db8.png" width="281" height="500">

At the bottom - looking for distance as well as time
```

---
## \#1095 Posted by: Maxid Posted at: 2017-04-14T16:13:08.318Z Reads: 205

```
Copy the log file to excel and you'll see - or upload to http://www.gct-hp.de/VDLA/
```

---
## \#1096 Posted by: jaykup Posted at: 2017-04-14T16:58:24.238Z Reads: 212

```
Sure - I love that tool, but after a ride I'd like to quickly see how many miles I went, and since this app is recording that it would be nice to display it right in the app, instead of having to upload onto the site later on to see.
```

---
## \#1097 Posted by: Eboosted Posted at: 2017-04-14T17:27:15.053Z Reads: 214

```
I'd love to get the VDLA tool on Android  :heart_eyes:
```

---
## \#1099 Posted by: Wubbalubbadubdub Posted at: 2017-04-16T09:17:22.206Z Reads: 213

```
I just tried to flash the firmware, but all it does is disconnect the VESC from BLDC tool. I cycle the power off/on the board. When I reconnect, it shows the same firmware is present, and if I try to use the ackmaniac BLDC tool, it says it has limited connectivity. I am using a windows 10 computer, and a VESC hardware 4.12. Am I missing something?
```

---
## \#1100 Posted by: Lukas Posted at: 2017-04-16T09:27:12.408Z Reads: 212

```
@Wubbalubbadubdub
Is it a maytech vesc?
```

---
## \#1101 Posted by: Wubbalubbadubdub Posted at: 2017-04-16T09:34:18.219Z Reads: 206

```
Yes, it is. Nuts. I just looked it up. :(
```

---
## \#1102 Posted by: landonkun Posted at: 2017-04-16T21:54:44.412Z Reads: 210

```
What was the issue? I'm having the exact same issue with my Maytech as we speak, but couldn't find the solution with the search function.
```

---
## \#1103 Posted by: Eboosted Posted at: 2017-04-16T21:56:23.304Z Reads: 210

```
You need a programmer to upload the the bootloader, only after that you will be able to upload the Ackmaniac firmware. 

Look for bootloader programmer
```

---
## \#1104 Posted by: landonkun Posted at: 2017-04-16T21:57:17.550Z Reads: 206

```
Thank you, I am dumb and didn't check "search in this thread" and just found the solution. Seems simple enough.
```

---
## \#1105 Posted by: Wubbalubbadubdub Posted at: 2017-04-17T16:54:32.538Z Reads: 210

```
No boot loader. Not a difficult fix, but la-aame.
```

---
## \#1106 Posted by: ryny24 Posted at: 2017-04-21T01:08:15.285Z Reads: 211

```
+1 Maytech VESC user; could not upload firmware. I grabbed a cheap [ST-Link V2](http://www.ebay.com/itm/112353490837), and I'm now running 2.54!!  Thank you thank you thank you! Off to configure...
```

---
## \#1107 Posted by: lowGuido Posted at: 2017-04-23T20:54:56.686Z Reads: 204

```
@Ackmaniac is there any chance you could code up the VESC so that the C button on the nunchuck uses perpetual steeze and the Z button does cruise control?
```

---
## \#1108 Posted by: Ackmaniac Posted at: 2017-04-23T21:07:44.917Z Reads: 208

```
Perpetual steeze? 
If you only want to switch the button functions there is a checkbox for that in the Nunchuk settings of my firmware mod.
```

---
## \#1109 Posted by: jbruce Posted at: 2017-04-24T05:20:12.739Z Reads: 213

```
@Ackmaniac have you found an iphone yet to work on the iphone app?
```

---
## \#1110 Posted by: Titoxd10001 Posted at: 2017-04-24T07:51:56.094Z Reads: 219

```
After accidentally hitting reverse full throttle into my fence dislocating it from the rail I've limited my minimum erpm to -10000. Is that okay or there a potential issue I'm not seeing

Also on dual drive I have each vesc batt min set at -10 but on the app it reaches -20. Not sure if I'm reaching -20 per vesc and if I lower batt min will I have potential brake failure?
```

---
## \#1111 Posted by: Ackmaniac Posted at: 2017-04-24T08:00:10.561Z Reads: 217

```
In the app you can adjust how many VESCs you have in your board. Power, motor current,  battery current and the Wh and ah calculations is multiplied by this number. So it is correct that you see 20 amps in the app when you set it to 10 amps for each VESC.
```

---
## \#1112 Posted by: jul88 Posted at: 2017-04-24T08:59:04.218Z Reads: 214

```
Hello,
first test for me with this app on my mountainboard.

I always have a crash of the app if I switch between an another app like Locus Map pro.
See below a video.
https://youtu.be/siCb3eA9UYk

An idea to solve this issue ?
Thanks
```

---
## \#1113 Posted by: Ackmaniac Posted at: 2017-04-24T09:30:51.500Z Reads: 197

```
You have a crash while you are recording a video and change to another application. Didn't even think about that. Have to check myself what can be the issue.
I guess in when you don't record a video it works normally. Or do you still have a crash when you change the app?
```

---
## \#1114 Posted by: jul88 Posted at: 2017-04-24T09:45:26.307Z Reads: 196

```
In order to record all the datas in csv file, must I record a video too ?
```

---
## \#1115 Posted by: lowGuido Posted at: 2017-04-24T10:17:51.363Z Reads: 193

```
I know you jave a check box to disable the braking but could you make it so that Z button still brakes and C button doesn't?
```

---
## \#1116 Posted by: The_Dude Posted at: 2017-04-24T12:17:10.684Z Reads: 188

```
Hmmm ... what about reverse, then?
```

---
## \#1117 Posted by: Ackmaniac Posted at: 2017-04-24T12:27:10.977Z Reads: 195

```
In the PPM settings there is this possibility by turning the steering wheel in one or the other direction for cruise with and without braking.
For the Nunchuk this possibility doesn't exists and it would involve a lot of coding because then reverse needs to be handled like in PPM. And i am also not planning to provide such features.
Of course it would be possible but it's hard for the users to understand how it works and the whole setup process is already complicated enough.
```

---
## \#1118 Posted by: lowGuido Posted at: 2017-04-25T02:47:38.389Z Reads: 194

```
Screw reverse.  I never go backwards. 
But fair call. You dont wanna have to code it up. 

I guess ill just stick to perpetual steez and screw cruise control.
```

---
## \#1119 Posted by: jbruce Posted at: 2017-04-25T03:39:51.443Z Reads: 191

```
[quote="lowGuido, post:1118, topic:12286"]
I guess ill just stick to perpetual steez and screw cruise control.
[/quote]

arent those the same things?
```

---
## \#1120 Posted by: lowGuido Posted at: 2017-04-25T04:07:18.993Z Reads: 187

```
No. perpetual steez has no brakes.
cruise control regulates your speed.

two totally different animals.
```

---
## \#1121 Posted by: jbruce Posted at: 2017-04-25T04:08:43.561Z Reads: 185

```
ahh gotchya, wouldnt perpetual steez be best most of the time then so that the board is not constantly braking and accelerating?
```

---
## \#1122 Posted by: lowGuido Posted at: 2017-04-25T04:10:20.215Z Reads: 197

```
well yes, I only ever use perpetual steez. never cruise control.

but I thought seeing as there is a check box in the software it might be nice to have the option of both..

either way. its no big deal.
```

---
## \#1123 Posted by: Lambjr088 Posted at: 2017-04-28T17:32:36.917Z Reads: 199

```
Does anyone have a tutorial on how to flash the vesc 4.10 to be able to use the extended bldc tool or is it just a plug and program like the regular bldc?
```

---
## \#1124 Posted by: caustin Posted at: 2017-04-28T20:28:04.346Z Reads: 201

```
Following up on your suggestions on cheap android phone for use with VESC, looking for something cheap used w/camera and screen (smaller to midsize better form factor than large).  Would something like this work, without activating carrier network or anything (BLE to VESC, maybe Wifi for getting things onto or off the phone?).  Not sure what version of Android it needs to be, though I guess 5.0 for video?

https://www.amazon.com/Samsung-Google-Android-Smartphone-Sprint/dp/B006YG7ZMU/ref=sr_1_13?s=wireless&ie=UTF8&qid=1493410654&sr=1-13&keywords=google+nexus&refinements=p_36%3A14674872011
```

---
## \#1125 Posted by: E-Boarding Posted at: 2017-04-28T20:37:14.857Z Reads: 198

```
I use a Samsung Ace2 with CyanogenMod for Andoird 5, it works fine except the video-feature, the phone freezes when trying to make a video

I do use a USB-Cable to update the phone and copy the csv-files from the app, no wifi etc.
```

---
## \#1126 Posted by: caustin Posted at: 2017-04-28T21:27:58.350Z Reads: 199

```
Excellent, I will check that out too though look s like not upgradeable past 4.1 or so, maybe because hw specs don't support the video. Not sure if I need to pay extra for an unlocked or rooted phone particularly, if it works without accessing or activating carrier network?
```

---
## \#1127 Posted by: emmaanuel Posted at: 2017-05-01T16:21:37.146Z Reads: 196

```
Hi @Ackmaniac, 
Congratulation for your work, it's a great improvement of the original software.
Have you plan to shared your code on GitHub ?
Maybe some of us, can help you improving your soft, your firmware and even more with a iOS app. 
Github let you decide which modification you want to include, so you'll not loose the control of your work.
```

---
## \#1128 Posted by: Alan_Smithee Posted at: 2017-05-02T17:37:54.598Z Reads: 197

```
I have [this VESC.](http://e-greenmotion.com/index.php?route=product/product&product_id=282)

when I connect to the esc via the extended bldc too it says I have an old version (2.18) but can update via the firmware tab. When I do that, the green bar goes to the end and it says firmware update complete and the vesc disconnects. I then have to power it off and on again, but when reconnecting it shows the same message, that I have an old version. It appears the firmware upgrade process didn't do anyting.

is there a fix for that?
```

---
## \#1129 Posted by: NAF Posted at: 2017-05-02T17:43:30.677Z Reads: 198

```
Guys can someone explain to me ..if I had first used Extended BLDC tool on WINDOWS to set my VESC ...can I use BLDC app on MAC OSX as well  and it will detect my vesc or it wont recognize the vesc settings ??
```

---
## \#1130 Posted by: Plumb77 Posted at: 2017-05-03T01:31:11.549Z Reads: 197

```
I connected my Bluetooth module and it will not connect to my phone says pairing rejected. So I have a 10s3p with 25r Samsung's also a polar 6374 190kv motor I set up watt control and this motor spins entirely too fast I set it up for 750 watts too. Is this normal? I'm used to standard bedder settings and it's the first time using BLDC.
```

---
## \#1131 Posted by: Ackmaniac Posted at: 2017-05-03T07:27:22.116Z Reads: 210

```
@Alan_Smithee When the update is complete then the VESC automatically starts again. It takes around 10 seconds to come alive again. So please don't power it off and on again. Just wait.

@NAF yes it will work on windows and OSX

@Plumb77 Please write me in a PM what you think is wrong and add Screenshots of all the motor settings and also the PPM tab. But i guess you have the wrong PPM Pulsewidth settings, So please use the setup wizard for the Pulsewidth adjustment.

@E-Boarding please try the new Version of the app in my Dropbox link. Maybe that solves your problem.
```

---
## \#1132 Posted by: rwxr Posted at: 2017-05-03T07:31:53.867Z Reads: 210

```
@Alan_Smithee: E-greenmotion are rebranded Maytech VESC's and they don't come with a bootloader unfortunately. 

https://www.electric-skateboard.builders/t/vesc-installing-a-bootloader/752
```

---
## \#1133 Posted by: PetreyTee Posted at: 2017-05-05T02:30:44.926Z Reads: 208

```
If I adjust the throttle/brake curve on the master vesc, do I need to send that to the slave vesc at all?  I am having a problem where no matter how soft I set the curve my brakes will almost lock up when I press the brake down to ~30% or so and cause the belt to skip. 

I'm not feeling very confident when I ride and I'm not having much fun :frowning:
```

---
## \#1134 Posted by: Eboosted Posted at: 2017-05-05T02:44:30.090Z Reads: 202

```
What remote are you using?

You should calibrate your remote via PPM settings on BLDC tool, have you done that?
```

---
## \#1135 Posted by: PetreyTee Posted at: 2017-05-05T03:02:37.604Z Reads: 196

```
Sorry, I thought about that as I was writing, but totally forgot when I posted. 

I have a Raptor 1 with the Nano-X controller. I thought I had my controller calibrated pretty well, but I suppose I can play around with that setting. Thanks for the suggestion!
```

---
## \#1136 Posted by: Ken Posted at: 2017-05-05T03:03:27.803Z Reads: 197

```
There's way too many posts for me to follow this properly, but I have a few questions:
Will this BLDC tool work with the Enertion VESC-X?
If so, where do I find the Firmware to update the VESCX? I'm using a MAC, and I did find the BLDC-TOOL for MAC, but not the firmware update.
Thanks!
```

---
## \#1137 Posted by: Eboosted Posted at: 2017-05-05T03:06:20.747Z Reads: 201

```
@PetreyTee
If you still have the same issues after recalibrating ,hit me up, I might know what's going on and how to fix it

@Ken
Everything you are looking for is in the first post
```

---
## \#1138 Posted by: PetreyTee Posted at: 2017-05-06T03:26:52.854Z Reads: 201

```
Recalibrating the remote seems to have worked. I made it so that it doesn't go all the way down to zero when the brake is fully depressed. That way I have a gentle brake until I really need it. 

Thanks a lot!
```

---
## \#1139 Posted by: DilatedPupils Posted at: 2017-05-06T03:40:16.913Z Reads: 200

```
This is awesome. 
Would this work on dual on splitter? Or only on canbus?
```

---
## \#1140 Posted by: Tuomalar Posted at: 2017-05-06T06:53:48.742Z Reads: 205

```
Just rode few km with my new board noticed that my brakes are way too powerfull. It's very scary to brake at hi speed. What would be best way yo soften that brake? I'm using nano-x remote, my motor min is 30A and i haven't touch braking curve.
```

---
## \#1141 Posted by: Eboosted Posted at: 2017-05-06T07:15:40.669Z Reads: 196

```
Did you adjust the ppm settings?
```

---
## \#1142 Posted by: Tuomalar Posted at: 2017-05-06T08:06:01.201Z Reads: 196

```
No i didn't. I just made that "auto wizard" and used those values.
```

---
## \#1143 Posted by: Tuomalar Posted at: 2017-05-06T12:55:20.025Z Reads: 203

```
Any idea what are good values? I would like very soft throttle and brakes in both modes.
```

---
## \#1144 Posted by: pyttroll Posted at: 2017-05-06T13:09:52.759Z Reads: 214

```
Here is a throttle curve that should give you smooth acceleration / brakes:

<img src="/uploads/db1493/original/3X/e/b/eb60915ca24912e16aa3f5c0cb7b70c9a98b0f99.png" width="690" height="417">
```

---
## \#1145 Posted by: Tuomalar Posted at: 2017-05-06T13:15:52.887Z Reads: 206

```
So i don't have to change PPM values? Only throttle curve.
```

---
## \#1146 Posted by: pyttroll Posted at: 2017-05-06T13:17:05.406Z Reads: 207

```
Make sure your PPM value are also set correctly, yes.
```

---
## \#1147 Posted by: Tuomalar Posted at: 2017-05-07T08:10:20.652Z Reads: 220

```
Brakes are still crazy. Throttle is fine but brakes are like on/off. I move that throttle pot 2-3mm and i can stop at steep hill and i weight 90kg so what should i do? Here is my settings. <img src="/uploads/db1493/original/3X/d/5/d547cdaab339c60939b0ae6da97543d0ae90d632.png" width="690" height="388"><img src="/uploads/db1493/original/3X/d/9/d9143c142ff26a8fdda9b880984bdadf39b1a61a.png" width="690" height="388"><img src="/uploads/db1493/original/3X/0/f/0f36f55f9894f811a778282086969e7ca83c1bb8.png" width="690" height="388">
```

---
## \#1148 Posted by: yaca Posted at: 2017-05-07T09:35:04.202Z Reads: 191

```
For better testing make the brake curve linear. If you pull the trigger slowly does the green bar follow it in the same time from 50 to 0%? 0% should be reached when the trigger is at the end of his way not earlier. If this is alright try to set Motor min to 20 and Batt min to -5. Do you feel a difference now or same hard braking?
```

---
## \#1149 Posted by: Tuomalar Posted at: 2017-05-07T11:55:21.574Z Reads: 193

```
Yes green bar do follow. I changed motor min to -20 and its little better but but still way too powerfull. Now i can use sbout half throttle. I think i try -15 or more linear brake curve.
```

---
## \#1150 Posted by: Plumb77 Posted at: 2017-05-07T14:45:46.042Z Reads: 195

```
Got everything working except the Bluetooth is not connecting to my phone. Any tips?
```

---
## \#1151 Posted by: Eboosted Posted at: 2017-05-07T15:53:00.595Z Reads: 201

```
Here is the trick to fix your brakes. 

1. Turn on your remote first, not your board
2. Press the throttle all the way up
3. Press the brakes all the way down
4. Turn on your board
5. Ride with the brakes working fine
```

---
## \#1152 Posted by: Michael319 Posted at: 2017-05-07T16:25:57.919Z Reads: 198

```
Does that actually work? Sounds interesting
```

---
## \#1153 Posted by: Tuomalar Posted at: 2017-05-07T17:19:52.979Z Reads: 203

```
I thought that works only with car escs? Because in vesc you have PPM settings.
```

---
## \#1154 Posted by: Eboosted Posted at: 2017-05-07T18:10:04.917Z Reads: 202

```
Let me know if it works
```

---
## \#1155 Posted by: Tuomalar Posted at: 2017-05-07T18:37:49.802Z Reads: 202

```
Yes it did! Awesome.Now i just have to add some brake power :D
```

---
## \#1156 Posted by: oxi Posted at: 2017-05-08T13:54:29.830Z Reads: 204

```
Just one word about your work! It is awesome !!! 

I have just build my board with dual 6375 and vesc-x and never use the original vedder firmware but your's and it is perfect :slight_smile:
Thanks you for all !

I have seen that you provide source code for your modified firmware. Is it possible to share your android app too ? i wan't to create a application in my raspberry for transmit information via GSM and i think i will use bluetooth for communicating with my rasp because i wan't to keep it in my bag :slight_smile:

So if it is possible juste said me , it can be very usefull for me.

Sincerely
```

---
## \#1157 Posted by: caustin Posted at: 2017-05-08T21:49:07.455Z Reads: 213

```
I tracked down an android device to try and use for this, but it is only a Nexus S 4G w/Android 4.1.2 build JZ054K.  Looks like I need at least Android 4.4?  I am having a hard time finding the right android update to sideload, can you point me in the right direction?  I was able to sideload the Vesv Monitor app but got the expected parse error when trying to install on unsupported older hw and OS.  Any help much appreciated, I just want to get something up and running (Wifi no wireless carrier) just for Vesc Monitor app!
```

---
## \#1158 Posted by: oxi Posted at: 2017-05-08T22:44:56.990Z Reads: 210

```
Personally, i have to smartphone, a galaxy s4, and a "ELEPHONE S7".

Since the last update only my S4 is ok with the vesc monitor application. The 2 phones are on android 6. Perhaps you can upgrade your phone with a cyanogenmod ?
```

---
## \#1159 Posted by: SeanHacker Posted at: 2017-05-09T05:51:05.198Z Reads: 217

```
PM me and I'll get your device added to our supported list. I've been really busy with work and my wife was just diagnosed with MS so I've been dealing with that. But it should be no problem updating your device. We specialize in Nexus and open source devices.
```

---
## \#1160 Posted by: gaetjen Posted at: 2017-05-10T07:07:16.879Z Reads: 230

```
@Ackmaniac I have been using your firmware for quite a while now and it's perfekt. I have the latest version, the 2,54. But today, I wanted to check the reverse mode with no weight, it spinned for a couple of seconds full speed and then stopped I tried it again and the same thing happend. The third the motor didn't spin at all, neither backwards nor forward. I connected it to my laptop and damnit...
Fault            : FAULT_CODE_DRV8302
Current          : 0.4
Current filtered : -0.0
Voltage          : 30.88
Duty             : 0.00
RPM              : -0.1
Tacho            : 849
Cycles running   : 3
TIM duty         : 32
TIM val samp     : 5
TIM current samp : 8398
TIM top          : 8400
Comm step        : 0
Temperature      : 29.81
Any ideas what could be the reason for this?
I have a sk3 6364 with a 8s Lipo and a esk8.de VESC and I run it in FOC
<img src="/uploads/db1493/original/3X/4/3/4314a2a875213dfcb8e872b4d6303a55c3f7e4ad.png" width="690" height="387">
<img src="/uploads/db1493/original/3X/6/e/6e058b26a068b816d0efa7c750ace5679487763e.png" width="690" height="387">
```

---
## \#1161 Posted by: Maxid Posted at: 2017-05-10T07:53:06.933Z Reads: 233

```
I guess you know what happened - Fried DRV in FOC mode.
The classic
```

---
## \#1162 Posted by: Ackmaniac Posted at: 2017-05-10T08:13:57.025Z Reads: 235

```
FOC on the bench can cause issues. Especially at full speed. Some motors run flawlessly and others are very sensitive. I guess it is because you give the signal to open the door for the current but the motor can't consume it because it is already at max speed. But it also can be another reason. 
Best is to prevent the full speed issue when you reduce the limit ERPM start and end value in the PPM settings. When you set this  to nearly full speed then the VESC will try to reduce the current when it reaches this speed.
So for example when your motor reaches 55000 ERPM on the bench then you can set the ERPM limit start to 50000 and the end to 55000.
For example when i go down a hill with my R-SPEC 6355 then my motors start to go crazy at full speed. They can't go any faster and only produce like 300 watts even if i give full throttle. Because they are already close to their maximum speed. This starts at around 57 km/h for me. So i set the maximum speed to 58 km/h and say that it should start to reduce the power output at around 52 km/h. So i have no trouble with the motors anymore. But i also have to run them at a switching frequency of 30000 (normally 20000). Otherwise they are gittering so that my whole board vibrates and they also killed a DRV. Since i have them at 30000 everything is fine (Only the max speed issue which i solved by the settings above).

Also when you try to keep a slow speed on the bench by giving very little power can also cause issues.

On the other side the R-SPEC Ghost prototypes (Raptor 2 Motors) run without any issues in FOC.
I think that the distance of the magnets to each other is important for the FOC capability. I could be wrong but this is the biggest difference between the motors physically (apart from the amount of magnets 14 / 28).
```

---
## \#1163 Posted by: guyguy Posted at: 2017-05-10T16:08:20.613Z Reads: 217

```
Hey Ackmaniac - where do you adjust setting to have it backoff power at 52km/h in the tool? Sorry if this has been answered elsewhere.

[edit] ignore this question  - I was only thinking of the motor config tabs, I'm assuming you limit this under the PPM soft ERPM limits section
```

---
## \#1164 Posted by: TranxFu Posted at: 2017-05-10T16:30:45.578Z Reads: 214

```
Same thing happened to me :) FOC was running wonderful before. Updated to 2.54 and tried reverse mode on the bench. Was fine when I stood on the board tho.
Got the DRV fried. Its currently undergoing repair :smile:
```

---
## \#1165 Posted by: TarzanHBK Posted at: 2017-05-11T07:52:42.169Z Reads: 213

```
A good advice would be: Don't run Foc on the bench . People keep frying their vescs with it.
```

---
## \#1166 Posted by: yaca Posted at: 2017-05-11T20:02:04.586Z Reads: 209

```
Maybe it's just a problem with unsensored motors?
```

---
## \#1167 Posted by: Ken Posted at: 2017-05-12T19:24:33.793Z Reads: 211

```
Hopefully this will be my last stupid question on this. I have 2 VESCX's in CANBUS. Do I need to update the firmware on each one, or will they both update if I install the firmware on one? The second one is stuck down with adhesive tape, and doesn't want to come out, and I don't have room to fit a USB cable into the port.
Ken
```

---
## \#1168 Posted by: Eboosted Posted at: 2017-05-12T19:26:20.394Z Reads: 206

```
You need to update both and also make motor detection on each individual one. Thus step is important in order to rise smoothly and avoid issues
```

---
## \#1169 Posted by: Ackmaniac Posted at: 2017-05-12T19:33:55.463Z Reads: 219

```
But you can update the VESC via the CAN bus. Just below the connect button you can select which controller id the slave vesc has and choose "CAN Fwd"
```

---
## \#1170 Posted by: Ken Posted at: 2017-05-12T22:49:20.549Z Reads: 218

```
Thanks, hopefully one last question....In your install instructions, it says: "Be aware that this is only for Hardware Version 4.10 or above (VESC-X as well).
Where do I find the hardware version on my VESCX? All I can find is it's firmware version 2.18, and I received these brand new in March 2017.
Ken
```

---
## \#1171 Posted by: Ackmaniac Posted at: 2017-05-12T22:56:48.461Z Reads: 207

```
Every VESC-X works.
```

---
## \#1172 Posted by: Ken Posted at: 2017-05-12T22:57:49.318Z Reads: 208

```
Thanks! Wish me luck as I'm diving in now!
Ken
```

---
## \#1173 Posted by: Ken Posted at: 2017-05-12T23:24:56.999Z Reads: 206

```
Using a MAC, the firmware quit unexpectedly. Every time I try to reboot it, I get the same error, although it does say I'm on Firmware version 2.54
```

---
## \#1174 Posted by: Ackmaniac Posted at: 2017-05-12T23:26:15.483Z Reads: 202

```
Just simply reboot by powering the VESC off and on again. It's the same. But just wait 5 seconds in between.
```

---
## \#1175 Posted by: Ken Posted at: 2017-05-12T23:29:30.997Z Reads: 202

```
OK. I thought I had everything configured correctly, but my remote isn't making the wheels turn
```

---
## \#1176 Posted by: Ackmaniac Posted at: 2017-05-13T00:39:08.847Z Reads: 204

```
Did you setup the correct application. i guess you need to choose PPM in the App configuration Gnernal Tab.
```

---
## \#1177 Posted by: Ken Posted at: 2017-05-13T01:02:41.007Z Reads: 202

```
Yes, that was my issue. Now I'm trying to figure out how to detect the second motor in BLDC mode. I have all boxes checked for multiple ESC's over CAN...
Figured it out...it was the CAN FWD box to get to motor #2.
```

---
## \#1178 Posted by: Ackmaniac Posted at: 2017-05-13T01:38:02.852Z Reads: 202

```
You have to be aware that you also need to flash the slave vesc with the firmware.
```

---
## \#1179 Posted by: Ken Posted at: 2017-05-13T03:00:10.261Z Reads: 210

```
I got it all sorted out, and thanks for your help! I'm not sure what was happening, but for some reason, the remote wouldn't work, or one wheel wouldn't turn. I had to keep disconnecting and reconnecting everything from time to time, and all is good. Now I just need to figure out which remote to use with the CC.
Thanks again!
Ken
```

---
## \#1180 Posted by: Fabian287 Posted at: 2017-05-13T17:21:57.593Z Reads: 214

```
Hey i connected my ArduBoardController (Nunchuck with Oled) and i get wrong values. For example is my battery voltage x 10 for example the real voltage is 31V but after flashing your firmware my oled shows 310V?!  :smiley:

PS: Its no problem for me i just divided the VESCinput voltage in the libarie by 10^^. If you are interested to fix this ^^

PPS: sry for my english im german :smile:
```

---
## \#1181 Posted by: gaetjen Posted at: 2017-05-13T18:18:54.460Z Reads: 203

```
Do you know of a place in Europe where you can repair a fault DRV chip?
```

---
## \#1182 Posted by: TranxFu Posted at: 2017-05-13T20:06:38.684Z Reads: 203

```
I've send mine to Lucas at LP-Electronics in Germany. However its been almost 3 weeks since it has arrived there. I have not gotten any updates or replies when asking about the current situation... So I can't really advise you to sent it there yet. :/
```

---
## \#1183 Posted by: DeathCookies Posted at: 2017-05-14T00:07:36.383Z Reads: 201

```
I had several times personal contact with Lukas. He is a kind and skilled dude. His Equipment is excellent :heart_eyes: (i was at his Office). 

I would definitivly recommend him!
```

---
## \#1184 Posted by: JanarR Posted at: 2017-05-14T05:15:12.111Z Reads: 197

```
Same here. No response from Him. Over 2 weeks here.
```

---
## \#1185 Posted by: venti2k Posted at: 2017-05-15T10:52:01.929Z Reads: 205

```
Hey,
I'm currently using a steez remote. Is it somehow possible to change the riding modes via remote? I'm from Germany as well and especially interested in the "police" mode ;)
regards
```

---
## \#1186 Posted by: Ackmaniac Posted at: 2017-05-15T10:55:26.673Z Reads: 212

```
In theory it would be possible. First i switched the mode when i press the brake for 3 seconds fully. Problem is that it would be necessary to store the other modes on the VESC as well. And change the BLDC-Tool to have the possibility to setup different modes. That all is possible but i think it's much easier via the app. 
Cool would be a remote with display where i can change the modes.
```

---
## \#1187 Posted by: venti2k Posted at: 2017-05-15T11:03:27.673Z Reads: 218

```
Yeah, right. 
A smartphone/remote combination would be nice ;)
```

---
## \#1188 Posted by: Ken Posted at: 2017-05-15T22:44:03.551Z Reads: 224

```
It took me a while to get all of this done, as I had my VESCX's configured wrong, which was causing all of my above issues. I had both VESCX's set at 0, instead of 0 and 1. 

The throttle curve works splendidly, and I originally set it up like the pic below. Acceleration used to be twitchy, and now it's very smooth. I hated the braking on the settings below, and have since changed it back to the standard linear setting. I don't feel a need to change the brakes at this time. 

Thanks for building this BLDC tool...I sent some dollars you way today! Now if somebody could just build the APP for my iPhone...

<img src="/uploads/db1493/original/3X/e/7/e7b67966a07eb4a9d9302a0c7b0759ff66ee1922.png" width="671" height="500">
```

---
## \#1189 Posted by: rtasca Posted at: 2017-05-15T23:47:34.940Z Reads: 216

```
amazing work !!! I do have some HC-05 modules lying around but I guess they won't work... certainly gonna give it a try especially because centering the PPM is a PITA on Vedder's BLDC tool.
```

---
## \#1190 Posted by: Achmed20 Posted at: 2017-05-19T06:17:24.036Z Reads: 215

```
so i just tried flashing my vesc (4.12 @fw 2.18) with this firmware  and it just keeps the 2.18 one.

guess i am missing a bootloader right?
```

---
## \#1191 Posted by: TarzanHBK Posted at: 2017-05-19T06:27:35.868Z Reads: 217

```
yep you do. For instructions go here:
https://www.electric-skateboard.builders/t/vesc-installing-a-bootloader/752
```

---
## \#1192 Posted by: Achmed20 Posted at: 2017-05-19T16:53:59.346Z Reads: 214

```
ok thx,
i've seen that link allready, just missing my programmer ^^
```

---
## \#1193 Posted by: dino15309 Posted at: 2017-05-20T03:16:05.722Z Reads: 209

```
Hello! I was wondering if I could use your mod to adjust my failsafe? My remote does not include one and I do not want to ride if it puts me in danger (well... more than normal :wink:)

also, could you please include a download link for this mod?

Thanks!!!
```

---
## \#1194 Posted by: Titoxd10001 Posted at: 2017-05-20T04:04:32.004Z Reads: 204

```
That could potentially work because you can adjust center pulsewidth. Download links are in the first post
```

---
## \#1195 Posted by: Ackmaniac Posted at: 2017-05-20T11:13:25.466Z Reads: 206

```
@dino15309 You can't do this by software. And you can find the link in the first post of this thread. Which remote do you use?
```

---
## \#1196 Posted by: dino15309 Posted at: 2017-05-20T12:40:15.581Z Reads: 212

```
I use the Quanom pistol grip. I didn't know much about RC remotes and how bad this one was until it was too late...
```

---
## \#1197 Posted by: Pimousse Posted at: 2017-05-23T18:41:15.172Z Reads: 216

```
@Ackmaniac, where can we find the changelog of your app ?
It seems that Play store often updates the app, but no way to find out what has been changed. :wink:
```

---
## \#1198 Posted by: Ackmaniac Posted at: 2017-05-23T18:51:21.705Z Reads: 211

```
Usually I don't update the change log. So the best information you can get about changes is here in this thread.
```

---
## \#1199 Posted by: Deakbannok Posted at: 2017-05-24T19:36:00.660Z Reads: 211

```
The changelog of the app
* improvement of the sound and graphic
* now you can view your speed in full 4k resolution.
```

---
## \#1200 Posted by: Titoxd10001 Posted at: 2017-05-27T08:17:10.952Z Reads: 213

```
Any chance of duty cycle with nuetral? Watt mode is cool, just favor duty cycle and think other people might to.
```

---
## \#1201 Posted by: Ackmaniac Posted at: 2017-05-27T13:18:42.578Z Reads: 212

```
Not at the moment. Want to finish some other stuff first and i think i will add my modifications to the VESC-Tool when it comes out so it makes more sense to implement it there. I still think current or watt control is still much more controllable. And if you think the power is too weak then simply raise the settings. Duty Cycle control makes only sense to me when you ride offroad and change the surface you are riding on. For example when you change from tarmac to wet grass or sand. Because then the power output would be raised automatically when the wheels stat to spin slower.
```

---
## \#1202 Posted by: Titoxd10001 Posted at: 2017-05-28T06:13:12.406Z Reads: 208

```
Yeah, waiting on vesc tool, but it's always being delayed and with all the bad publicity I wouldn't be surprised if it it's not compatible with anything besides vesc6. In app weekly firmware updates I think?

It's all preference, but I want duty cycle to have more control. For example I measured 3000watts+ on accelerations on flats. So if I set max watts at 1500 per vesc to have that power on reserve. Once I reach my max speed of let's say 30mph it only takes 750watts or 1/4 throttle to stay there. So going 15mph it only takes 1/8 throttle to maintain speed. If it was duty cycle, in theory I would use 1/2 throttle for 15mph and full throttle for full speed. 

The way I see it current/watts is not leanier how you said when switching surfaces, also if theres hills, a small driveway, if theres a small rock in front of the wheel, if you want fast acceleration. With speed you want to increase linearly​ if you're going slow, fast, up a hill, off road. And what happens if I want to pull 6000 watts I would use 1/16 throttle for 15mph? Duty cycle from my understanding would still be 1/2 throttle. Duty cycle is not perfect or for everyone, but I like that it's predictable
```

---
## \#1203 Posted by: Ackmaniac Posted at: 2017-05-28T07:22:24.661Z Reads: 195

```
And there is the problem. It is not predictable. In theory it simply says that you want a specific speed. And it uses all the power that is allowed to get there. Even if you only give 1/4 throttle from a standstill then it does full power till you reached 1/4 speed. There is a bit more to it but basically that is how it works.
```

---
## \#1204 Posted by: Eboosted Posted at: 2017-05-28T07:23:58.873Z Reads: 188

```
That's why the Evolve remote is so damn touchy and can't be adjusted
```

---
## \#1205 Posted by: Titoxd10001 Posted at: 2017-05-28T08:21:44.172Z Reads: 196

```
I understand your concern of pulling infinite amps, but I don't think that would be the case. Especially with vesc because you can set  limits on amps. The thing that will change is the way you control those amps. With a decent long through remote you can still get up to speed smoothly and not use all those amps. And if you want to accelerate faster, youll have all the power in reserve, you just move your finger faster. It's not as bad as you make it out to be, I think you should try duty cycle.

@eboosted I tried a evolve and yeah it's a bit touchy. Not sure if it's remote not having much range or because with escs you can adjust the punch level to your liking.
```

---
## \#1206 Posted by: Jinra Posted at: 2017-06-03T08:39:18.936Z Reads: 192

```
Hey @Ackmaniac,

I'm gonna try out your custom f/w and had a question in regards to throttle. Does your predictable throttle mean that 50% throttle = 50% speed as well? With current control, I have a decent understanding that once current overcomes load, the motor will try to rev at its rated kv. However, I don't think I'm fully understanding the intricacies of watt control.
```

---
## \#1207 Posted by: Ackmaniac Posted at: 2017-06-03T11:15:14.478Z Reads: 203

```
No it doesn't mean 50% of speed. It is also a bit strange that everybody wants that behavior. Your car also doesn't work like that. When you give half throttle in the first gear then you also easily reach full rpm. And not half speed of that gear. The problem in current control is that you loose throttle range at higher speeds when your battery max and motor max is different. Because you control the motor current with the throttle.
Watt control still gives you full control over the power even at higher speeds. Explained it a couple of times but for that you need to understand how duty cycle works.
But long story short. Just give it a try, i guess you like it. And with the app you can change from current control to watt control in a second. And by the quick change you can really compare the 2 control modes. 

Finally makes your board more controllable. You don't have these moments anymore where the board power let's you loose balance and gives you the feeling that you are a passenger instead of the pilot. Especially when you use high current settings with lot's of power.
```

---
## \#1208 Posted by: Jinra Posted at: 2017-06-03T19:54:02.260Z Reads: 195

```
Thanks. I'm not saying I'd like throttle based speed control, just simply trying to understand, in finer detail, how it's different than current control. Still don't have a clear idea, but maybe it's something I have to try to understand.
```

---
## \#1209 Posted by: Ken Posted at: 2017-06-03T22:52:55.803Z Reads: 184

```
FWIW, I've been using the Watt mode, and it works great!
Ken
```

---
## \#1210 Posted by: Youssless Posted at: 2017-06-04T15:20:34.173Z Reads: 198

```
Hi guys, 

@Ackmaniac, you've put in crazy amounts of work and I'm excited to use this but have run into a wall...

I'm trying to flash my VESC (4.12) with your modded firmware (V2.54) but I get an error where it says connected initially then 'no firmware read response'. 

I've skimmed through all 1,176 posts above but nothing solves the issue. Even pressing connect and upload immediately after. What am I doing wrong?

Everything is connected and turned on, I just can't get a response from my remote and figured it might need a setting changed in the BLDC Tool (not used this VESC nor configured it previously). 

Thanks for any help,

Youssless
```

---
## \#1211 Posted by: Ackmaniac Posted at: 2017-06-04T17:41:51.544Z Reads: 191

```
So you didn't flash it with my firmware mod. Seems that the VESC has problems and that the original firmware isn't even flashed correctly. You can try to upload it via a Stlink programmer. But maybe this VESC has bigger problems.
```

---
## \#1212 Posted by: jbruce Posted at: 2017-06-04T17:44:47.565Z Reads: 189

```
Let me explain how I believe watt control works, @Ackmaniac correct me if I'm wrong. It seems to be a combination of current control and duty cycle control. When you first begin to accelerate it controls the watts by controlling the current however once you have reached a speed where the current drops and the duty cycle is constant, it controls the watts by changing the duty cycle. This leads to fine control of acceleration using current control during startup and then fine control of speed using duty cycle when going at faster speeds. I hope that makes sense.
```

---
## \#1213 Posted by: Jinra Posted at: 2017-06-04T18:13:16.241Z Reads: 183

```
If that were the case wouldn't speed by limited by throttle position. He said in his last post that it wasn't.
```

---
## \#1214 Posted by: Youssless Posted at: 2017-06-04T18:51:21.775Z Reads: 182

```
I bought the VESC from @WARMAN but everything else I got from him works fine and the VESC itself is from DIY. I've asked and they've told me that it comes flashed with firmware already. 

Say I do need to flash it, do I need to do anything else other than get a Stlink programmer or am I good to flash it with your custom firmware?
```

---
## \#1215 Posted by: Jinra Posted at: 2017-06-04T18:55:36.649Z Reads: 182

```
DIY *should* come with a bootloader so you wouldn't even need STlink to flash the firmware, just make sure to use the modified BLDC tool.
```

---
## \#1216 Posted by: Ackmaniac Posted at: 2017-06-04T18:58:15.794Z Reads: 188

```
As i understood he can't even geta connection to any BLDC-Tool. Correct would be when it shows the text that there is a too old firmware installed on the VESC when you open it with my BLDC-Tool mod.
```

---
## \#1217 Posted by: Youssless Posted at: 2017-06-04T19:07:11.797Z Reads: 197

```
@Jinra This is also what I've been told.

@Ackmaniac I can't get a connection with your BLDC tool. Yours is the only one I've tried as I've had trouble finding anything else that isn't 2 years old and works on Windows. If you know of a BLDC tool that will work with the standard firmware then I'd love to download it and flash my VESC with your modded one.
```

---
## \#1218 Posted by: Ackmaniac Posted at: 2017-06-04T19:07:49.115Z Reads: 199

```
Watt mode is a modified current control. In current control you control the motor amps.
So when your motor max is set to 80A then 15% throttle is 20A, 50% throttle is 40A and 75% throttle is 60A.
The problem is that when your battery amps are at for example 40A then your VESC can't reach the motor amps after 50% duty cycle anymore. Because with 50% duty cycle the 80A at the motor are 40A at the battery. So the maximum for the battery is reached. But normal current control doesn't care. So the faster you go the higher get's the duty cycle and the less throttle you need to throw full possible power. So at full speed you only need roughly 50% throttle to give full power. 
That means the faster you go the more you loose throttle range and the board becomes less controllable via the remote.

In watt control the you still have the full throttle range at high speeds to control the speed. And it can take the battery max as upper limit or a specif watt value. When it is controlled by the watts then it has the advantage that the power output will be the same no matter which voltage the battery is at.
```

---
## \#1219 Posted by: Ackmaniac Posted at: 2017-06-04T19:09:18.252Z Reads: 198

```
If you can't get a connection to mine then i doubt you will get a connection to any. Maybe the USB on your computer has wrong drivers installed or the VESCs are faulty.
```

---
## \#1220 Posted by: Youssless Posted at: 2017-06-04T19:11:24.079Z Reads: 201

```
Thank you for responding so quickly, I haven't installed any drivers, just tried pressing connect after powering it up. 

Are there drivers I need to get? if so, could I trouble you to point me in the right direction?

Thanks again
```

---
## \#1221 Posted by: Youssless Posted at: 2017-06-05T17:03:32.636Z Reads: 202

```
<s>Hey Ackmaniac, 

<s>With the help of </s>@sayreul <s>today we managed to connect to the VESC and upload your custom firmware without issue. However, now at home again I still get the same error and fail to connect. Are there any drivers I may be missing? my PC automatically configures the VESC as a COM device (not that I will pretend to know what that means).

<s>Thanks for your help,</s>

<s>Youssless </s>

Nevermind, it continued to configure and then the option of connecting to COM5 came up and I'm all good now.
```

---
## \#1222 Posted by: Guacamoleface Posted at: 2017-06-05T18:10:32.305Z Reads: 193

```
Still in love with this application. I have one problem tho. I cant see my files when plugged into computer(clicked save on folder in application and folders are there but no items in it, not hidden either) Also I cant send them to my drive etc in the application.


edit: I just realised I didnt post this in the android application thread, hope its allright anyway ;)
```

---
## \#1223 Posted by: Ackmaniac Posted at: 2017-06-05T22:44:04.962Z Reads: 189

```
Did you try to send it via the app to any other place? Like Dropbox or store it in another location or send it via email. And can you click on the files on the app so that it shows you the graphs or the the video?
```

---
## \#1224 Posted by: gaetjen Posted at: 2017-06-09T21:16:21.509Z Reads: 182

```
Shit. Another fried DRV-chip in FOC. Didn't use reverse or applied full power on the bench. It happend while driving in Watt-mode. I`m done with FOC...
```

---
## \#1225 Posted by: Pimousse Posted at: 2017-06-09T21:18:44.188Z Reads: 182

```
Doing test bench in FOC often kills the DRV.
What is your voltage ? just for information.
```

---
## \#1226 Posted by: Jinra Posted at: 2017-06-09T21:29:28.131Z Reads: 186

```
What VESC were you using?
```

---
## \#1227 Posted by: Guacamoleface Posted at: 2017-06-09T21:31:46.668Z Reads: 190

```
Hey, Yeah I tried it. the only thing I can do is send Videos to "Photos" on my cloud. But I cant send them nor the CSV files to any other place, not even my drive. I tried Email aswell. it just say the file failed to send or that it could not be found. I cant find it while plugged in either. 

I can see the graphs with no problems
```

---
## \#1228 Posted by: bardialongo Posted at: 2017-06-10T07:00:05.477Z Reads: 189

```
First of all I want to personally thank you for the efforts and the great work you did @Ackmaniac! I was wondering if, using a hm-10 bluetooth module, I can connect the vesc to BLDC tool on my pc.. It still works flawlessly using the android app, but would be much easier, for bench tests and configurations, to work on pc :)
```

---
## \#1229 Posted by: gaetjen Posted at: 2017-06-10T07:25:32.900Z Reads: 192

```
8s lipo 8000mah
```

---
## \#1230 Posted by: gaetjen Posted at: 2017-06-10T07:26:06.669Z Reads: 201

```
Esk8.de and enertion.
```

---
## \#1231 Posted by: Ackmaniac Posted at: 2017-06-10T09:06:23.839Z Reads: 206

```
I made the experience that the reliability of FOC depends very much on the motor you are using. For example my Enertion R-SPEC 6355 i have to run at 30000 switching frequency instead of 20000 to get them running properly. At 20000 they throw sometimes errors and let the board vibrate at higher speeds. But changed to 30000 (experience of endless tests) they run fine and more efficient than BLDC. With the FOCBOX they run even better.
So which motor are you using?
```

---
## \#1232 Posted by: gaetjen Posted at: 2017-06-10T09:38:58.006Z Reads: 199

```
I'm running a sk3 6364 with 245kv. In current mode it used to run flawless in FOC, but it seems to have a problem in watt mode. Before the chip fails, the vesc restarts a couple of times and I can ride again and then nothing.
```

---
## \#1233 Posted by: E-Boarding Posted at: 2017-06-10T10:21:16.122Z Reads: 207

```
[quote="Ackmaniac, post:1231, topic:12286"]
For example my Enertion R-SPEC 6355 i have to run at 30000 switching frequency instead of 20000 to get them running properly
[/quote]

never seen that, what is this frequency and where/why to adjust?
```

---
## \#1234 Posted by: Ackmaniac Posted at: 2017-06-10T10:59:40.640Z Reads: 210

```
Marked it on the upper right in the picture.
<img src="/uploads/db1493/original/3X/b/2/b26be4a9aefa808ca859365624edc8c23b70472b.png" width="690" height="463">
But to make it correct you should do a complete motor detection again and change the TC value to 750 so that the values get calculated correct for the faster switching.

And it is no garanty that it works better. The motor will become more silent but it is also more stress for the mosfets. So in theory they should become a little warmer and be less efficient. But i couldn't experience a difference in temperature or efficiency. But the motors run much better. But this is at your own risk and i only can recommend it for 63 motors. No experience with other motors.
```

---
## \#1235 Posted by: E-Boarding Posted at: 2017-06-10T12:09:00.941Z Reads: 199

```
think I'll try it soon, VESC-X is really reliable so far
```

---
## \#1236 Posted by: Ackmaniac Posted at: 2017-06-10T12:11:46.882Z Reads: 196

```
If your motors don't have any issues then you should not change anything. Mine had faults and vibrated. With the new values i never had a single fault. But i think that really depends on every different motor.
```

---
## \#1237 Posted by: Achmed20 Posted at: 2017-06-10T13:38:42.106Z Reads: 201

```
tested your app and firmware a bit and so far i realy like the watt mode. feels so much more natural and my baord doesnt want to throw me off just when starting anymore. those nano remotes can be real twitchy ^^

a donation is almost mandatory here ;)
```

---
## \#1238 Posted by: Jinra Posted at: 2017-06-12T15:08:02.488Z Reads: 206

```
I know what you mean, I used a nano v2 and when compared to my benchwheel using the exact same settings, braking on the nano nearly throws me off every time I engage it where as the benchwheel is smooth sailing. I think I need to increase my deadband and decrease my motor min. Unfortunately, switching over to watt mode didn't change anything in regards to braking for me.

I haven't really noticed a difference with watt mode yet, though I haven't been anymore than 1/3 throttle since I'm simultaneously testing the nano v2 remote and don't want to street my face. I'm glad this F/W has throttle curve support though so if my setting adjustments don't help with the braking, I'll simply adjust the curve.
```

---
## \#1239 Posted by: Ken Posted at: 2017-06-12T23:21:50.616Z Reads: 199

```
I just received my HM-10, and the 7 pin connector will arrive this Thursday, so I'm getting ready for the app. A few questions:

I read from 2 different people on which V to use. Is it 5V or 3.3V?

I need to buy an Android phone, as I have an IOS. Can anybody recommend a good cheap android 5 or higher phone? Will an android tablet work just the same? I found this at Best Buy for $50 and it has Android 6.0 Marshmallow. Will it work?
<img src="/uploads/db1493/original/3X/5/f/5f778cc906b9e9e2bf246fc1f8dcc739a31334a7.jpg" width="623" height="500">
```

---
## \#1240 Posted by: Ackmaniac Posted at: 2017-06-12T23:25:15.274Z Reads: 191

```
Just have a look at the backside of the Bluetooth module. Mostly they have the writing on them that they work from 3.6V till 6V. So you need to connect them to the 5V in most cases. If ou see 3.3V then connect it to 3.3V on the VESC. But most modules only work at the 5V pin.
```

---
## \#1241 Posted by: Ken Posted at: 2017-06-13T00:25:25.142Z Reads: 206

```
I bought the HM-10 that you shared the link with above. I can figure out the 5V and ground, but what about the other 2 wires? Here's the best pic I have of the Enertion VESC-X, and it's not labeled RXD and TXD

<img src="/uploads/db1493/original/3X/8/5/85b7587b18b094e34e24ee56d49bacae2a5cba3d.png" width="690" height="336"><img src="/uploads/db1493/original/3X/c/a/ca1670d8f739a4a02b389f1433bb2c24252d4e88.jpg" width="556" height="500">
```

---
## \#1242 Posted by: Jebe Posted at: 2017-06-13T00:31:58.322Z Reads: 192

```
Second from the top is rx, 3Rd from the top is tx
```

---
## \#1243 Posted by: Ken Posted at: 2017-06-13T00:35:59.915Z Reads: 193

```
Thanks! It's nice to know how to connect everything before the parts arrive and I tear into everything.
```

---
## \#1244 Posted by: Jebe Posted at: 2017-06-13T00:36:40.145Z Reads: 208

```
Am having trouble getting the app version 1.30 to display values. Have tried 2 Bluetooth modules on a vesc x and a vesc 4.12. Initially this worked, now the app connects, but displays no data. :( 
Have ordered more Bluetooth modules to try but can anyone suggest anything?  
Connected to 3.3 volt supply.
Rx and tx are crossed. 
Restarted phone.
Updated app. 
Tried different Bluetooth units. 
Vesc is running acks firmware.
App is set to ppm and uart - tried uart only
baud rate is 9600

really doesn't help that the pinouts are different between the enertion vesc and vesc-x

Darn. Looks like it's an issue with my sony xperia z2 -  vesc x works on an old samsung note 3
Vesc 4.12 doesn''t. :confused:

@Ackmaniac is it possible to get an older version of your app ?
```

---
## \#1245 Posted by: Ackmaniac Posted at: 2017-06-13T06:38:47.486Z Reads: 210

```
Connect the module to the 5V pin and restart the phone. My phones Bluetooth also only worked again after a restart. But had that only once.
```

---
## \#1246 Posted by: Eboosted Posted at: 2017-06-13T06:41:28.075Z Reads: 216

```
@Jebe check this:

http://www.electric-skateboard.builders/t/vesc-hm-10-bluetooth-wiring/12838/20
```

---
## \#1247 Posted by: Jebe Posted at: 2017-06-14T00:26:08.235Z Reads: 208

```
Got it. App wouldn't update on my sony so uninstalled, re-installed, It then worked on the vesc-x.
Faulty bluetooth module on the vanguard. They both show up as BT05 so when I thought I had tested both I must have mixed them up. Just having trouble changing from the default mode now.
```

---
## \#1248 Posted by: Eboosted Posted at: 2017-06-16T08:40:17.300Z Reads: 211

```
Yesterday I was helping a friend to connect his hm-10 module to his board, I tried to do it first from my phone, I was, at the moment, connected to my own board via vesc monitor and at the same time tried to connect to his HM-10 right away my master VESC was blown, not even the blue or pink light flashing. 

Has anyone got a similar problem, blowing a vesc because of strange behavior of the hm-10 module?
```

---
## \#1249 Posted by: Pimousse Posted at: 2017-06-16T09:22:17.674Z Reads: 209

```
Maybe it's not blown but just the STM32 messed up.
@hexakopter had the same issue IIRC on the VESC 6 and recovered it using a STLink.
```

---
## \#1250 Posted by: Ackmaniac Posted at: 2017-06-16T10:36:51.553Z Reads: 204

```
Please give a detailed description what you did. But you can't connect to 2 modules via my app. Because when you go back from the realtime screen to the devices screen you close the connection to the previous module. So you can't be connected to 2 devices at the same time. And there isn't a chance to kill anything by only being connected.
```

---
## \#1251 Posted by: Ackmaniac Posted at: 2017-06-17T22:38:26.185Z Reads: 206

```
I made a change to the firmware bin file which fixes a glitch in the sources that also exists in the original software. When the motor max is set to a very low value in FOC and the motor min is set to a high value the maximum brake power is the moor max value instead of the motor min value.
This is fixed in this version. this way you can give the board to beginners and allow only very little power while the brakes still can be strong.
For example in my Police mode i want the power to be extremely weak while i still want full brake performance if something stupid happens.
If motor max is higher or the same as motor min you won't have issues with the old version. But if you use modes like i described then it would be useful to change.

The version number is still the same and also BLDC-Tool did not change.
```

---
## \#1252 Posted by: markyoe Posted at: 2017-06-18T06:17:31.742Z Reads: 201

```
How do you change to your Police mode? Through your controller or through the app?
```

---
## \#1253 Posted by: Ackmaniac Posted at: 2017-06-18T10:24:56.750Z Reads: 216

```
With the app of course. That's how the mode looks like as a example. But you can crate your own modes to whatever you like.
But in FOC if you set the motor min lower than motor max (ignore the - sign) then you need the latest change i released yesterday. This bug that motor min can't be lower than motor max in FOC also exists in the original firmware. In BLDC mode it works fine.
<img src="/uploads/db1493/original/3X/9/9/99c53239117512649e85b88cf24f16cb707e862b.png" width="281" height="500">
```

---
## \#1254 Posted by: Jinra Posted at: 2017-06-19T18:44:16.999Z Reads: 226

```
The braking on my Nano v2 is SUPER sensitive, I know this is the remote since my Benchwheel remote didn't have this problem. I'd like to use throttle curve to adjust this, but had a question.

If I wanted to reduce the braking power at X throttle I'd assume I'd have to make the curve go above the default linear line right? Like so...

<img src="/uploads/db1493/original/3X/0/4/0480d597b6c95b33aafe9096b4a28edcdeec5943.png" width="603" height="500">
```

---
## \#1255 Posted by: SageTX Posted at: 2017-06-19T18:47:20.834Z Reads: 219

```
That is correct.
```

---
## \#1256 Posted by: NAF Posted at: 2017-06-20T15:14:21.334Z Reads: 220

```
Holly molly ..this is the first time I am trying to play with EXTENDED BLDC TOOL on my mac and it works perfect !! ..One question @Ackmaniac from your experience what would be the best THROTTLE CURVE settings for mini remote ?
```

---
## \#1257 Posted by: Ackmaniac Posted at: 2017-06-20T20:13:17.871Z Reads: 222

```
I can recommend to start with these settings and then it is up to your taste.
<img src="/uploads/db1493/original/3X/4/9/49eb8b9e0898cdb68fe4845db0befe0a34190d5a.png" width="686" height="499">
```

---
## \#1258 Posted by: nikoli280 Posted at: 2017-06-21T18:32:56.919Z Reads: 229

```
Is there a guide for the setup? and is this the components i need?

https://goo.gl/6yf1Ki

and

https://goo.gl/komw2j
```

---
## \#1259 Posted by: Pimousse Posted at: 2017-06-22T10:42:59.111Z Reads: 228

```
What do you want these components for ?
If it's for using the app, use the one recommended by Acmaniac himself :
http://www.electric-skateboard.builders/t/vesc-monitor-android-app/20888?u=pimousse
```

---
## \#1260 Posted by: rpn314 Posted at: 2017-06-23T11:05:38.571Z Reads: 218

```
Anyone else who uses this BLDC-Tool on a mac, do you have issues with the application crashing when you have to reboot the VESC?
```

---
## \#1261 Posted by: Ken Posted at: 2017-06-23T14:41:06.172Z Reads: 218

```
I believe I had that issue. I just re-connected, and all was good.
Ken
```

---
## \#1262 Posted by: Jinra Posted at: 2017-06-23T14:48:03.429Z Reads: 214

```
Yes indeed, gave me quite the scare when i first flashed the fw. Thought i bricked the vesc.
```

---
## \#1263 Posted by: rpn314 Posted at: 2017-06-23T22:17:09.221Z Reads: 212

```
Yeah. I've had the issue for a while (things randomly crashing don't usually phase me...), I was just curious if it was just my system or the entire mac build. Sounds like it's an issue with the program interacting with the mac and not just my machine.

@Ackmaniac, I can send you some debug information about this crash. I can reproduce it on demand, just so you know. I believe it may be related to the mac app trying to access the port after it's no longer available (since the VESC has rebooted and not reconnected yet or the VESC has powered off)
```

---
## \#1264 Posted by: mptrs Posted at: 2017-06-25T19:37:52.934Z Reads: 212

```
@Ackmaniac this is great! Donation made!

I hope you can help me out with some settings cause I'm kinda scared I created an uncontrollable rocket (I'm not that fast and not the best at a human powered skateboard).

I already put it in Sensored mode so it won't go super fast. But I would like it to be in newbie mode if possible. I've seen the Soft RPM limit but not sure what to fill in.
Adjusted the acceleration throttle curve to match the number you posted a few posts back. But is it possible to get it a bit more like the starter mode from the boosted board.

Would love to have a no broken bones first ride, so hope you can help me out hehe.
```

---
## \#1265 Posted by: Ackmaniac Posted at: 2017-06-25T19:50:34.796Z Reads: 205

```
Just post Screenshots of you Motor Tab. Then i can give the best advice's.
Or send be Screenshots of all your setting via PM. Then  i can tell you my 2 cents.
```

---
## \#1266 Posted by: gaetjen Posted at: 2017-06-26T14:11:56.601Z Reads: 217

```
@Ackmaniac. I keep getting these faults, which I haven't gotten with version 2.53. Do you know what the fault could be? 
<img src="/uploads/db1493/original/3X/d/5/d582dcba74da0021562723b4f788d142a0965d9d.png" width="281" height="500"> 

<img src="/uploads/db1493/original/3X/7/f/7f4a83431d05b70009cc41c15a9b450debc5a4dc.png" width="281" height="500">

Checked the cables and everything. I run a dual unsensored setup.
Edit: Just saw that my Motor Max is at 120A, changed that to 70A. Hope that changes it.
```

---
## \#1267 Posted by: Ackmaniac Posted at: 2017-06-26T14:42:31.319Z Reads: 198

```
To set the motor max lower should fix the issue. With 120 Motor amps you are very close to the Absolute max of 130. This is also the value that exceeded. The reason is that the VESC always trys to adjust itself to achieve the wanted amps. So it can happen that it overshoots a little bit. So it is always good to have enough wiggle room to the Absolute max limit.
```

---
## \#1268 Posted by: mptrs Posted at: 2017-06-27T20:57:17.417Z Reads: 202

```
When there is weight on the board it works good. Will try it for now cause it feels very smooth.
Thanks again for the extended BLDC tool!
```

---
## \#1269 Posted by: lrdesigns Posted at: 2017-06-29T01:34:38.447Z Reads: 217

```
I just want to drop some love :heart_eyes: here. I have been using this firmware for a couple weeks now and its sooo awesome! My most favorite feature is that you can set the end points (& mid point) for the PPM signal. Before I could not get all the travel for my brake on a GT2B remote. If you pulled the brake all the way the vesc would stop breaking, its actually dangerous. :scream: 

Every feature in BLDC tool has a mouse over info tip which is so nice to have. The watt mode gives much more linear control at high speed. On top of all that adjustable throttle curves. Its only missing one thing, an icon. :blush: 

It took me a while to get on board as I have maytech vesc without a boot loader. So had to get a programmer and make up cable. The first time I put on the boot loader it was scary as I didnt want to brick it, but its actually really simple. There was just no clear concise instructions on how to do it, just bits of information here and there. <img src="/uploads/db1493/original/3X/5/6/565354fef10edbc407380d525184afe7c3d0522c.jpeg" width="666" height="500">
```

---
## \#1270 Posted by: bdohler Posted at: 2017-07-03T20:02:52.960Z Reads: 196

```
Flashing my 4.12 from FW version 2.18 to 2.54 throws an unknown error with your tool. Any advice on resolving this?
```

---
## \#1271 Posted by: Ackmaniac Posted at: 2017-07-03T20:05:03.277Z Reads: 193

```
Do you have a Maytech VESC? And when does this error appear? And for flashing you can also use the old BLDC-Tool if a bootloader is installed.
```

---
## \#1272 Posted by: bdohler Posted at: 2017-07-03T20:15:19.584Z Reads: 196

```
@Ackmaniac himself! Thanks for the help. 

I believe it's a Vedder original. It says "VESC 4.12 Benjamin Vedder" next to the uC. Not sure of it's origin.

Error message appears after clicking "Upload" and the progress bar reaches 100%. I then lose connection to the VESC until I power cycle.
```

---
## \#1273 Posted by: Ackmaniac Posted at: 2017-07-03T20:17:07.540Z Reads: 192

```
And does it tell that the Firmware is too old the next time you connect to the VESC?
```

---
## \#1274 Posted by: bdohler Posted at: 2017-07-03T20:26:57.432Z Reads: 194

```
Yes. It reads again that the firmware is 2.18, so the flash isn't happening.
```

---
## \#1275 Posted by: Ackmaniac Posted at: 2017-07-03T20:46:21.160Z Reads: 194

```
Did you order that VESC in China? The bootloader is missing. You need to get a StLink to flash it to the VESC. Just search a bit in this forum for more information.
```

---
## \#1276 Posted by: bdohler Posted at: 2017-07-03T20:52:43.595Z Reads: 195

```
No, I doubt it's a knockoff. It's just more than likely been sitting in a box for two years. Thanks for the help.
```

---
## \#1277 Posted by: bdohler Posted at: 2017-07-03T21:46:50.915Z Reads: 196

```
@Ackmaniac, any idea where I can find a prebuilt version of the bootloader? I'm not running Linux...
```

---
## \#1278 Posted by: Ackmaniac Posted at: 2017-07-03T22:00:28.328Z Reads: 201

```
In my Dropbox link i added a hex file at BLDC-TOOl and Firmware\oldVersions which is called BootloaderAndFirmware2_18.hex
You can upload this via the stlink. It includes the original 2.18 firmware and the bootloader for 4.10, 4.11 and 4.12 VESCs.
This is not my modified firmware. But afterwards you should be able to flash the VESC to my firmware mod.
```

---
## \#1279 Posted by: bdohler Posted at: 2017-07-03T22:06:39.683Z Reads: 207

```
@Ackmaniac 

I've flashed the device, and now the modified BDLC_Tool is unable to locate the VESC. Not encouraging. I should be able to reflash with the STLink. I'll try again.

Edit: The VESC blinks three times blue/red, and then settles to blue. I've tried flashing twice now.

Edit 2: I simply flashed 2.54 with my STLink setup, and now it's working. Thanks again for all your help!
```

---
## \#1280 Posted by: rich Posted at: 2017-07-05T16:52:50.465Z Reads: 208

```
This is so awesome @Ackmaniac, can't wait to test it! :heart_eyes:
I just have problems with my vescs due to weird mosfet temperature real time data.
Both vescs weaving between -70 and -75 degrees!! That's too cold :joy:
Any idea what's wrong with my vescs?
```

---
## \#1281 Posted by: Ackmaniac Posted at: 2017-07-05T17:59:56.742Z Reads: 209

```
Seems that the resistors that are used to detect the temperature have issues. Think @Blasto can help you with that. But if tue temperature increases the Same amount like the real temperature increases then you can Set the temperature cutoff with a offset. But if both have the Same issue then it is very likely that the manufacturer used wrong resistors also at other places
```

---
## \#1282 Posted by: rich Posted at: 2017-07-05T18:30:23.950Z Reads: 215

```
What i did right now is i took my heatgun and heatened up the whole vesc to 60 degrees.
No increase of temperature at all in the real time data! So i think the temp sensor is broke.
I bought them last summer from scramboards, think i should contact them.
```

---
## \#1283 Posted by: Maxid Posted at: 2017-07-10T09:41:26.792Z Reads: 207

```
Not sure if bug or if I am missing something:
I set up a FOCBOX on the bench and adjusted the GT2B limits.
Then, in watt mode with reverse, I wanted to test the change of direction.
I don't want the board to inverse the speed directly but only brake until stopped and then wait before allowing the change in direction (= that is how my Car ESC does it as well).
So I activated "Enable maximum ERPM for direction switch".
This works when going forward and then brake. The motor will brake until stop and only when I release the throttle I am able to reverse.
However when going backwards and pulling the throttle, instead of gradually becoming slower and stop, the motor goes into forward direction super fast without resting first. Is that intended behavior @Ackmaniac ?
```

---
## \#1284 Posted by: Ackmaniac Posted at: 2017-07-11T07:19:24.674Z Reads: 199

```
Yes that behavior is how it should work. Because when you start on a hill while you roll a bit backwards you don't want to brake first.
```

---
## \#1285 Posted by: Titoxd10001 Posted at: 2017-07-11T07:24:53.477Z Reads: 199

```
I think most of us push off first. Seems like it would fry something going from reverse to forward so quickly
```

---
## \#1286 Posted by: Maxid Posted at: 2017-07-11T07:35:43.391Z Reads: 203

```
But I thought that is what the erpm limit is for. When being slow I don't mind it going directly into forward but if you are going fast it should also require to brake first. Who is going down a hill so fast and wants to go directly into forward? The wheels would just start slipping or the motor cogging no?
```

---
## \#1287 Posted by: Ackmaniac Posted at: 2017-07-11T07:42:00.882Z Reads: 206

```
And the ERPM limit works like that but only in one direction. Normally you don't go fast backwards. And if you do you brake gently. So this mode is mainly for going forward with the possibility to go backwards if you need it. But for forward it feels like the normal mode without reverse.
```

---
## \#1288 Posted by: Maxid Posted at: 2017-07-11T07:48:17.682Z Reads: 204

```
I don't understand why there should be a difference between forward and backwards regarding that limit. How do I brake gently? When going backwards I have to pull the trigger and that will cause the motor to also go directly into forward. Or is that only an issue on the bench?
```

---
## \#1289 Posted by: Titoxd10001 Posted at: 2017-07-11T07:50:55.572Z Reads: 202

```
That's exactly how it is while riding and is such a hassle going in reverse knowing it's going to shoot from under you if you hold brake which is suddenly forward
```

---
## \#1290 Posted by: Maxid Posted at: 2017-07-11T07:58:26.509Z Reads: 207

```
@Ackmaniac reading @Titoxd10001 post on the issue I feel the limit should really be applied for both forward and backwards.
```

---
## \#1291 Posted by: Ackmaniac Posted at: 2017-07-11T08:51:30.031Z Reads: 213

```
It doesn't shoot. If you accelerate gently it will brake gently and then smoothly start to accelerate. Only when you make a hard brake (acceleration at the trigger) it will start to spin in the opposite direction.
I wanted to add the reverse to be able to go smoothly backwards and not to use it as the normal riding direction.

And if the limit would exist in both directions you have the issue that when you roll a bit backwards on a hill and want to accelerate that you have to pull the trigger 2 times to accelerate.
```

---
## \#1292 Posted by: Titoxd10001 Posted at: 2017-07-11T09:06:26.988Z Reads: 201

```
Im exaggerating a little but I'm trying to say it doesn't feel predictable when switching directions so I mostly just coast to a stop when I'm nearing slow speed. If we had the option to double tap to go forward that would be cool but maybe a solution would be if there was a slight delay from going reverse to foward
```

---
## \#1293 Posted by: Ackmaniac Posted at: 2017-07-11T09:08:57.018Z Reads: 201

```
That would make it much more unpredictable. Because you don't know when it starts. If it doesn't feel predictable then i guess you have huge differences between the motor max value and the motor min value.
```

---
## \#1294 Posted by: Titoxd10001 Posted at: 2017-07-11T09:12:38.877Z Reads: 201

```
I mean the slightest delay so it's not instant power. I don't have sensors so it stutters when trying to change direction at times also. Motor values are 80a -45a dual
```

---
## \#1295 Posted by: Ackmaniac Posted at: 2017-07-11T09:13:43.190Z Reads: 200

```
Without sensors it is of course a pain in the A..
```

---
## \#1296 Posted by: Titoxd10001 Posted at: 2017-07-11T09:18:19.228Z Reads: 202

```
If I'm stopped it starts going forward well most of the time. But when I'm reversing and press brake which then turns into forward I'm still going in reverse slightly which causes stutters.
```

---
## \#1297 Posted by: Maxid Posted at: 2017-07-11T09:26:48.161Z Reads: 205

```
I think most people are using unsensored motors.
```

---
## \#1298 Posted by: Maxid Posted at: 2017-07-11T09:30:05.856Z Reads: 211

```
Predictable would need that it is the same no matter the direction. Making a difference in behavior for forward and reverse seems highly unpredictable to me. I was surprised when testing the function and the motor suddenly spinning even though I had it enabled and it was supposed to just stop. The natural assumption is that it should work the same both ways. How it is now is unpredictable.
```

---
## \#1299 Posted by: bdohler Posted at: 2017-07-13T16:16:22.548Z Reads: 215

```
Why is not the number of poles or pole pairs of the motor a parameter??

Can this firmware run a four pole motor?
```

---
## \#1300 Posted by: E-Boarding Posted at: 2017-07-13T17:50:33.776Z Reads: 206

```
@Ackmaniac, can you tell whats the default settings of the Raptor 2, what are the limits for Amps and Watts and total Watts, Reverse, TractionControl etc.?
```

---
## \#1301 Posted by: tvidotto Posted at: 2017-07-14T07:06:19.843Z Reads: 225

```
I decided to give a try with Watt control but for some reason, my remotes don't work in this mode.
I tried repairing multiple times and nothing.


I reverted the firmware and used the old BLDC tool and they started working again.

The new bldc-tool was working fine and with the new firmware. I could test the motor and even control with the keyboard. Everything looked fine except the remotes

I must be doing something wrong, but I don't know why. Any have an idea what it could be?

I have a nano remote and a gt2e remote
my vesc is from Diyelectric skateboards and on their site the description for firmware and hardware are:

VESC Hardware v4.12
VESC Firmware v2.18
```

---
## \#1302 Posted by: rich Posted at: 2017-07-14T10:10:12.640Z Reads: 233

```
Well, i did a test at home with watt mode to check the reverse function. It worked but too much throttle :joy:
<img src="/uploads/db1493/original/3X/5/a/5a56a7db0f3ccc7f111d6d16e88cac3e92ad6d48.jpg" width="281" height="500">
```

---
## \#1303 Posted by: rpn314 Posted at: 2017-07-14T13:35:41.496Z Reads: 217

```
Can you be more specific on "don't work work in this mode"? Screenshots of your app configuration tab in BLDC tool would be helpful
```

---
## \#1304 Posted by: Titoxd10001 Posted at: 2017-07-14T17:33:39.753Z Reads: 218

```
You can limit reverse speed with the min erpm I think I have it at about -10k. Also unchecked limit erpm with brake. Still not ideal but works okay
```

---
## \#1305 Posted by: rich Posted at: 2017-07-14T17:43:47.860Z Reads: 227

```
My description was confusing...
I accelerated forwards a little bit, then full brake (small room) and then i put unintended full throttle in reverse ( in my head it was still the brake). As a reaction of this happening i gave full throttle forwards. This is the forward burnout on the picture. DON'T TRY THIS AT HOME.
I am scared for now but i'll try to tweak the reverse speed as you mentioned when i go watt mode again.
Thanks!
```

---
## \#1306 Posted by: Titoxd10001 Posted at: 2017-07-14T17:48:57.883Z Reads: 228

```
Oh okay that makes more sense. Make sure you check box that says enable maximum erpm for direction switch. Idk why it's not checked as default but I think that may have contributed to the confusion
```

---
## \#1307 Posted by: tvidotto Posted at: 2017-07-15T09:15:12.144Z Reads: 238

```
[quote="rpn314, post:1303, topic:12286, full:true"]
Can you be more specific on "don't work work in this mode"? Screenshots of your app configuration tab in BLDC tool would be helpful
[/quote]

I redid everything and started taking print screens of all the windows
found the problem here
<img src="/uploads/db1493/original/3X/8/a/8a7980008783dedc60fd9420f64934350bfe1ba5.png" width="427" height="235">

I changed from UART to PPM and now it recognizes the controller input
```

---
## \#1308 Posted by: scepterr Posted at: 2017-07-23T09:41:38.422Z Reads: 222

```
Would it be possible to program a button on a controller turn on and off 5V output pin on vesc?

Also is the Android app open source? If not are there plans to add Android Wear support? 

Are there any vesc apps with Android Wear support?
```

---
## \#1309 Posted by: rpn314 Posted at: 2017-07-24T13:38:04.048Z Reads: 237

```
[quote="scepterr, post:1308, topic:12286, full:true"]
Would it be possible to program a button on a controller turn on and off 5V output pin on vesc?

Also is the Android app open source? If not are there plans to add Android Wear support? 

Are there any vesc apps with Android Wear support?
[/quote]



I don't see why you couldn't add an output like that. You'd have to get into the code though ;)

But it really just depends on what you're using it for. The 5v line on the VESC is limited to 1 amp max (and i'd keep it under that). So if you're just driving a switch or communicating with another board, you're probably fine. If you're looking to run an LED or something, you may blow something

I haven't seen the source, so I don't know if it's quite open source

I'm not aware of any apps that have android wear support that I can recommend. I heard of one app that may support it, but due to some poor behavior by the developer here, I don't recommend using the app so I won't link to it. Feel free to search around for it though :slight_smile:
```

---
## \#1310 Posted by: SilentException Posted at: 2017-07-24T13:49:12.649Z Reads: 237

```
Hi there. Noticing you did some great improvements here! As I'm waiting for my FOCBOX to arrive I was wondering if the following would be possible to do or implement.

Both Nano v2 and Nano-X have the "feature" where you need to go full throttle and full brake before you can use full range of the stick. Otherwise, a small stick movement results in a massive PPM movement which could mean a harsh brake or very fast acceleration, both not very good for rider :slight_smile:

Coming from the quad world, there is this "arming" procedure where the motors will not start until a arm switch is turned on or there is certain stick movement triggered. I don't know about the Nano-X but Nano v2 had a 2nd channel that could perhaps act as a arming switch?

Or better yet, set up arming trigger where throttle switch has to go full up and full down at least once (twice preferred) before motors would "arm".

I hope you can understand what I'm trying to say here, I suck at explaining my thoughts to others ("I swear, it was so clear in my head" haha) xD
```

---
## \#1311 Posted by: rich Posted at: 2017-07-25T02:14:42.570Z Reads: 243

```
[quote="Ackmaniac, post:1, topic:12286"]
To drive backward you have to release the throttle and brake again
[/quote]

When i brake in watt mode it drives backwards after full stop without releasing the throttle!
I have steez remote...

......... meanwhile i clicked "enable maximum ERPM for direction switch" it works now as described.
```

---
## \#1312 Posted by: TarzanHBK Posted at: 2017-07-25T11:41:43.064Z Reads: 245

```
Works like a charm :slight_smile: 
<img src="/uploads/db1493/original/3X/2/7/27bcee02b566c4a2d3464677571120bd6083c590.jpg" width="374" height="500">
```

---
## \#1313 Posted by: Maxid Posted at: 2017-07-25T11:42:52.138Z Reads: 227

```
how? :heart_eyes:
```

---
## \#1314 Posted by: TarzanHBK Posted at: 2017-07-25T11:45:14.327Z Reads: 232

```
that was a really hard task of coding:

1. Power your board
2. Run Ack´s app
3. Enjoy status over smartwatch

:monkey:
```

---
## \#1315 Posted by: Ackmaniac Posted at: 2017-07-25T11:46:39.918Z Reads: 226

```
Haha. I call that a lucky one. 
It wasn't my intention to show the notifications on the Smartwatches. But good to know that it works. So i think i should extend the info a bit. For example the distance and time.
```

---
## \#1316 Posted by: TarzanHBK Posted at: 2017-07-25T11:49:01.580Z Reads: 225

```
I´d love to have the speed there!
Also what I missed yesterday was the km i´ve ridden. Did i drink to much or is the app not showing the trip distance?
```

---
## \#1317 Posted by: Eboosted Posted at: 2017-07-25T15:02:34.697Z Reads: 219

```
@ackmaniac are you planning to add motor detection funcionalitity in the future?
```

---
## \#1318 Posted by: Achmed20 Posted at: 2017-07-25T17:31:13.684Z Reads: 220

```
[quote="Eboosted, post:1317, topic:12286"]
are you planning to add motor detection funcionalitity in the future?
[/quote]
pretty sure its in there isnt it?
```

---
## \#1319 Posted by: Eboosted Posted at: 2017-07-26T01:59:10.191Z Reads: 218

```
I'm sorry, I made the wrong question. 

Are you planning to add motor detection functionality via HM-10 Bluetooth module on order to be performed by an android app?
```

---
## \#1320 Posted by: scepterr Posted at: 2017-07-29T09:23:52.243Z Reads: 214

```
Can you add the ability to configure what shows up in notifications, motor amps, batt amps, etc
If you could also add the ability to change modes from notifications and have it work on Android Wear that would be awesome 😀
```

---
## \#1321 Posted by: thetechtrader Posted at: 2017-07-29T17:20:49.854Z Reads: 217

```
I will donate if you can help me get my first vesc running with my controller. My remote seems to be all or nothing, no feathering of speed in trigger.. and when I change any of the ERPM's speed is always the same I have the Alien Power system remote.

Can we do a screen share in skype and you walk me through it? PLEASE :)
```

---
## \#1322 Posted by: Trdolan03 Posted at: 2017-07-30T02:18:36.093Z Reads: 208

```
Has anyone tried to use the bldc tool with the APS dual esc?
```

---
## \#1323 Posted by: rpn314 Posted at: 2017-07-30T02:56:48.033Z Reads: 213

```
[quote="Trdolan03, post:1322, topic:12286, full:true"]
Has anyone tried to use the bldc tool with the APS dual esc?
[/quote]

...I think you're a little off topic, and I have no idea how that could work. The VESC and BLDC-tool use their own parameters and communication protocols that are entirely different than any other ESC that I'm aware of.
```

---
## \#1324 Posted by: mmaner Posted at: 2017-07-30T03:01:09.300Z Reads: 209

```
Keep in mind that you have to have a load on the board to see the acceleration accurately.
```

---
## \#1325 Posted by: i2oadsweepei2 Posted at: 2017-07-30T12:15:02.415Z Reads: 211

```
Mmaner is 100% right. When I first pulled the trigger on the bench and even today on the bench it just goes one speed. When it's loaded it behaves properly. Did you set up the remote using the wizard? Have you tried standing on it yet? Give a slight push and feather in the throttle. If you are new to esk8 be careful these things can pull harder then you think. I tested mine in my driveway and pointed the board toward a wooden fence just in case. All went well. Watt control is absolute control through the throttle range.

Good luck.
```

---
## \#1326 Posted by: andchiang Posted at: 2017-07-30T17:32:56.597Z Reads: 199

```
Is there any way the android app would be able to monitor the total miles that you have ridden on your board? Like a lifetime odometer?
```

---
## \#1327 Posted by: Ken Posted at: 2017-07-30T18:34:27.320Z Reads: 200

```
The app does tally board miles. Click on  the pencil Icon, and select board info. I'm at 260 miles since installing the app. 
Ken
```

---
## \#1328 Posted by: TarzanHBK Posted at: 2017-07-31T12:54:56.580Z Reads: 201

```
[quote="andchiang, post:1326, topic:12286, full:true"]
Is there any way the android app would be able to monitor the total miles that you have ridden on your board? Like a lifetime odometer?
[/quote]

@Ackmaniac we need km! :grin:
```

---
## \#1329 Posted by: andchiang Posted at: 2017-07-31T13:43:51.764Z Reads: 196

```
Does it only count the miles when the board is connected to the phone?
```

---
## \#1330 Posted by: Maxid Posted at: 2017-07-31T13:53:48.319Z Reads: 199

```
how else is it supposed to count?
```

---
## \#1331 Posted by: Michael319 Posted at: 2017-07-31T13:57:02.349Z Reads: 196

```
I don't believe there's any on board memory to store anything.
```

---
## \#1332 Posted by: Ackmaniac Posted at: 2017-07-31T14:36:50.316Z Reads: 196

```
Yes it only count's when it is connected. Thought already about the a possibility to store the data if you connect only at the end of your ride. But that would require new firmware changes. So at the moment it only tracks the miles or kilometers while the app is connected.
```

---
## \#1333 Posted by: Eboosted Posted at: 2017-07-31T18:16:47.515Z Reads: 197

```
It would be awesome to just plug an SD card that loop datalog all channels. It's doesn't seem to be a bad idea.

I een ha the idea to mount a dashcam on my board that records everything since I turn it on.
```

---
## \#1334 Posted by: Maxid Posted at: 2017-07-31T19:26:44.252Z Reads: 203

```
sure - but the question was related to the app and without the app connected there is no way for it to know when and how far you have ridden.
```

---
## \#1335 Posted by: jdyer8989 Posted at: 2017-08-01T21:51:08.454Z Reads: 197

```
Quick question. I am going to try this firmware out and need to load the firmware to both of my vescs. I have them connected with the canbus cable and the cable is held in with some hot glue on each connector. Is it alright to leave the canbus cable connected while updating the firmware?  Or is it possible to upload the firmware to the slave through the canbus? I tried looking through the thread but had no luck finding an answer.
```

---
## \#1336 Posted by: Eboosted Posted at: 2017-08-01T22:03:33.183Z Reads: 198

```
Just flash the firmware on each VESC individually
```

---
## \#1337 Posted by: jdyer8989 Posted at: 2017-08-01T22:16:42.247Z Reads: 191

```
Alright, will do. Is it ok to leave the canbus cable between the two vescs connected while uploading the firmware? I just want to be sure I don't cause any damage to the vescs.
```

---
## \#1338 Posted by: Ackmaniac Posted at: 2017-08-01T22:30:06.017Z Reads: 182

```
You can also upload the firmware via the canbus. After the flash be aware that the controllerid of the slave is 0 again. So you need to connect via can to 0.
```

---
## \#1339 Posted by: Guacamoleface Posted at: 2017-08-02T19:44:19.351Z Reads: 180

```
Its probably up there somewhere in the thread but couldnt find it so asking 
 In Watt mode - Is the reverse delivering the same speed / power as going forward?
```

---
## \#1340 Posted by: MrHappy Posted at: 2017-08-02T19:52:55.100Z Reads: 181

```
The power will be linear for reverse, and however you set it for forward. but they should be pretty close. they have the same start/ending points on the power vs throttle graph.
```

---
## \#1341 Posted by: jbruce Posted at: 2017-08-02T19:55:49.555Z Reads: 183

```
@Ackmaniac is there any new hope of an iPhone vesc monitor app?
```

---
## \#1342 Posted by: Titoxd10001 Posted at: 2017-08-02T20:26:09.735Z Reads: 185

```
The power will be the same but you can limit speed with negative erpm about -12k for me. Remember to uncheck apply brake to limit erpm
```

---
## \#1343 Posted by: Guacamoleface Posted at: 2017-08-02T20:29:47.028Z Reads: 186

```
@MrHappy @Titoxd10001
All right, thanks guys!

One more thing, I wonder in a scenario where if I slide - And end up in a switch position. Would the board go into reverse on brake or would it brake?

edit: Brake not break :joy:
```

---
## \#1344 Posted by: Titoxd10001 Posted at: 2017-08-02T20:38:00.972Z Reads: 192

```
I think it will brake not sure. Also make sure to check the box that says minimum erpm for direction switch in the ppm tab.
```

---
## \#1345 Posted by: Guacamoleface Posted at: 2017-08-02T20:39:33.783Z Reads: 186

```
Yeah I kept it on 4k RPM, Didnt get to test it much as the weather here let me down.
```

---
## \#1346 Posted by: MrHappy Posted at: 2017-08-02T20:43:36.068Z Reads: 188

```
you should test that. but do it with a helmet.
```

---
## \#1347 Posted by: Guacamoleface Posted at: 2017-08-02T20:52:10.285Z Reads: 189

```
I could do a safe test, by hand rolling it backwards and brake.
```

---
## \#1348 Posted by: Ackmaniac Posted at: 2017-08-02T21:14:31.701Z Reads: 198

```
If you are faster backwards than the min ERPM for Braking value then it doesn't brake. So if the value is at 4000 ERPM (with most gearings roughly 4 km/h) and you are faster backwards than 4000 ERPM (correct would be -4000 ERPM) then it will not brake. I did this especially for this kind of tricks.
```

---
## \#1349 Posted by: Guacamoleface Posted at: 2017-08-02T21:17:18.331Z Reads: 195

```
:heart_eyes:
```

---
## \#1350 Posted by: pshaw Posted at: 2017-08-07T16:19:03.272Z Reads: 192

```
@Ackmaniac if you select watt mode braking no reverse but forget to check the box to limit watts to the motors are you still in watt mode (just with no limit) or do you just stay in current mode?
```

---
## \#1351 Posted by: Jinra Posted at: 2017-08-07T16:32:24.443Z Reads: 188

```
watt mode but no limit. I don't use a watt limiter.
```

---
## \#1352 Posted by: GrecoMan Posted at: 2017-08-08T13:48:30.899Z Reads: 195

```
@Ackmaniac What do you recommend for the GT2B? Ive messed around with the throttle curve for about and when I hit 63% of my throttle, I hit top speed. 37% of my trigger is unusable! This was a problem with the standard BLDC Tool but I was hoping to fix it with your firmware
```

---
## \#1353 Posted by: Ackmaniac Posted at: 2017-08-08T13:53:35.867Z Reads: 190

```
You do not control the speed with the throttle. You control the power. It's the same as in a car.
```

---
## \#1354 Posted by: GrecoMan Posted at: 2017-08-08T13:54:38.299Z Reads: 191

```
Still, shouldn't I be able to get more usable throttle room?
```

---
## \#1355 Posted by: DeathCookies Posted at: 2017-08-08T13:55:07.184Z Reads: 193

```
Setup watt control and you are good to go
```

---
## \#1356 Posted by: GrecoMan Posted at: 2017-08-08T13:55:26.661Z Reads: 192

```
I am using watt control
```

---
## \#1357 Posted by: DeathCookies Posted at: 2017-08-08T13:57:54.670Z Reads: 194

```
Adjusted the Transmitter Settings (max, low and **mid** bandwidth)?
```

---
## \#1358 Posted by: GrecoMan Posted at: 2017-08-08T13:58:42.318Z Reads: 189

```
Yup ive got the pulsewidth set perfectly and my throttle trim adjusted too
```

---
## \#1359 Posted by: Ackmaniac Posted at: 2017-08-08T14:03:34.334Z Reads: 190

```
Lets say for example you setup the gearing of your board to 25 km/h. For that speed you only need around 250 Watts.
But settings of the VESC allow 2500 Watts. then even at 10 % throttle you would be able to reach top speed. The difference in Watt control is that before you reached the max speed which depends on your motors KV you are able to control the power output. But once you reached the max speed you can only control the power which is less to hold that speed. Every throtlle input that allows more power will only hold the max speed.
```

---
## \#1360 Posted by: GrecoMan Posted at: 2017-08-08T14:05:06.639Z Reads: 184

```
huh, that's disappointing.  I'm still gonna use the your firmware tho
```

---
## \#1361 Posted by: Jinra Posted at: 2017-08-08T14:37:37.450Z Reads: 182

```
If you're used to or expecting position based speed control, you may initially be disappointed in how current control works just as i was. However, over time i realized that it's just as good a control mode if not better than position based speed control.
```

---
## \#1362 Posted by: pshaw Posted at: 2017-08-08T15:10:36.686Z Reads: 183

```
I'm trying to figure out if traction control is for me or not. Would this help for an even push when carving at high speeds? 

Is there a downfall if any?
```

---
## \#1363 Posted by: Jinra Posted at: 2017-08-08T15:13:55.802Z Reads: 186

```
Traction control made things a bit rough (stuttering motors) when blasting full throttle from standstill for me, so I turned it off. The only downside in turning it off is that if your wheel lifts it can free spin, but it doesn't really affect anything. If anything it helps me know when I'm losing traction.
```

---
## \#1364 Posted by: pshaw Posted at: 2017-08-08T15:34:36.253Z Reads: 191

```
I just wanted to post this here so @Ackmaniac could see this as I posted this in my boost thread here but not sure if he will see it. 

Concerning the noise on the current sensor creating a bad reading and a "boost" at high throttles.... 

 The current default control loop is 2000hz I believe. Do you think we can lower the control loop time so that we can increase the sample rate? This in theory should smooth everything out and reduce the noise on the current sensor and hopefully get rid of the high duty cycle boost everyone is experiencing. 

Thoughts?
```

---
## \#1365 Posted by: Ackmaniac Posted at: 2017-08-08T15:39:12.603Z Reads: 185

```
I have good experiences with setting the switching frequency to 30000 for FOC. Exspecially on 6355 Motors this improves the smoothness of the motor a lot. Exspecially at higher speeds the motors start to vibrate with a switching frequency of 20000. At 30000 this is gone. But not sure about the power boost. I mainly use the FOCBOX and with this the issue is still there but you don't really recognize it. On my single drive with 4.10 HW it is very strong.
```

---
## \#1366 Posted by: Jinra Posted at: 2017-08-08T15:40:41.583Z Reads: 188

```
Do you think the higher switching frequency has any bearing on probability of burning the DRV?
```

---
## \#1367 Posted by: Ackmaniac Posted at: 2017-08-08T15:45:58.023Z Reads: 199

```
I personally think that you put a bit more stress on the mosfets. Could be that they get a little hotter. But didn't have any issues with that. And i think it protects the drive because the current reading becomes much better.

To say it short. My 6355 Motors killed a VESC 4.12 in FOC with 20000 and were undrivable because of the strong vibrations at high speed. (the whole board vibrated)
With 30000 Hz i never had a issue and the motors run buttery smooth. It's also a bit more silent. And in the analyse graph of bldc-tool it get's the best results. Above 30000 it becomes worse again.

At the weekend i drove @Nowind board and it had the same issue. Even with Vedders new Vesc-Tool firmware for Hardware version 4. Setting the frequency to 30000 also fixed that issue. 
With 28 pole motors like the Enertion Ghost of the Raptor 2 it didn't really make a difference.
```

---
## \#1368 Posted by: Jinra Posted at: 2017-08-08T16:15:27.419Z Reads: 192

```
Thanks a lot for the knowledge bomb! I'll try this out when i get my chaka vesc back from repair. I had stuttering and over current issues when i hit 47k erpm on that build.
```

---
## \#1369 Posted by: pshaw Posted at: 2017-08-08T16:27:52.185Z Reads: 202

```
I wish there was more data out there for 6374. So little info makes me a bit uneasy being Magellan testing things never done before on this setup. Many say 12S in FOC with 6374 is really playing with fire :/ 

Think bumping to 30,000 in hybrid mode would be risky for this setup? 

Oh BTW here are the graphs to show you just how bad the power boost is on a 6374 setup. You can see it jump from 89% duty cycle straight to 95% :scream: quite terrifying to have happen at 32mph!!! 


<img src="/uploads/db1493/original/3X/9/6/96a49a97316d8e474f48fcea3e209495a79edc96.PNG" width="281" height="500"><img src="/uploads/db1493/original/3X/f/d/fdda1f6529968415deb52ce447186fb8e8143d44.PNG" width="281" height="500">
```

---
## \#1370 Posted by: Ackmaniac Posted at: 2017-08-08T16:32:27.964Z Reads: 191

```
That 12S in FOC doesn't work is a myth. I run it like that all the time. Seems like many say what one guy imagined.
```

---
## \#1371 Posted by: pshaw Posted at: 2017-08-08T16:35:14.987Z Reads: 199

```
Not that the doesn't work but just that you'll have a much higher chance of blowing the chip. Do you have some settings you could suggest for my setup? Here is my main motor settings which seem to be working ok for hybrid mode.... I'm running torque vescs and 6374

<img src="/uploads/db1493/original/3X/9/c/9c12f23c1c4c02d651c49e99e7c8025f030decf6.jpg" width="281" height="500">
```

---
## \#1372 Posted by: Ackmaniac Posted at: 2017-08-08T19:29:59.768Z Reads: 193

```
What should I suggest? What Do you want. If it is fine for you then leave it as it is
```

---
## \#1373 Posted by: pshaw Posted at: 2017-08-08T22:37:39.926Z Reads: 193

```
I meant a starting point to try FOC mode as I've never tried it.
```

---
## \#1374 Posted by: Titoxd10001 Posted at: 2017-08-09T17:08:32.407Z Reads: 195

```
I'm pretty sure without traction control if you break a belt on one motor you lose brakes/power on both motors. Not sure if there is another way to prevent this and idk if this happens also if say you break a phase somehow. Considering going back to Y for this reason
```

---
## \#1375 Posted by: Jinra Posted at: 2017-08-09T17:09:25.944Z Reads: 192

```
Hm why would it behave like that? If traction control is off, it should ignore whatever the other VESC is doing in terms of RPM
```

---
## \#1376 Posted by: Titoxd10001 Posted at: 2017-08-09T17:20:34.284Z Reads: 188

```
Disconnected a belt and that's what happened. My guess is since throttle is current based the master doesn't need many amps with no load. Traction control makes it rpm based so it functions
```

---
## \#1377 Posted by: Jinra Posted at: 2017-08-09T17:27:31.777Z Reads: 189

```
Did you disconnect the slave or master belt?
```

---
## \#1378 Posted by: Titoxd10001 Posted at: 2017-08-09T17:34:18.033Z Reads: 190

```
The masters belt
```

---
## \#1379 Posted by: Jinra Posted at: 2017-08-09T17:36:41.530Z Reads: 193

```
Ah, does it behave similarly if you disconnect the slave?
```

---
## \#1380 Posted by: Titoxd10001 Posted at: 2017-08-09T18:09:55.917Z Reads: 193

```
I don't think I tried that, to lazy now. Give it a try when you get the chance
```

---
## \#1381 Posted by: Jinra Posted at: 2017-08-09T18:12:11.701Z Reads: 191

```
I use split PPM so i won't get too. Also my CAN pins ripped off my chaka VESC
```

---
## \#1382 Posted by: Titoxd10001 Posted at: 2017-08-09T18:58:21.250Z Reads: 200

```
I just switched to traction control. Wondering if it would have helped me the other day. Not sure if this is how it happened, but I was going over a slippery surface (handicapped sign freshly painted black @ night) only on one side and my wheel must have spun out and once I hit traction I was on the ground. 
Also wonder if it helps under braking on on low traction areas like dirt trails with urethane wheels
```

---
## \#1383 Posted by: scepterr Posted at: 2017-08-09T19:53:40.892Z Reads: 201

```
Just wanted to post a little warning to people with FOCBOX, do NOT flash any firmware while you are still under warranty, Enertion says that voids your warranty and will only help you if buy the plat warranty for $80. The DRV fried on mine in under a month and enertion is blaming the firmware. I know the firmware was not at fault, I hadn't even gotten around to tweaking settings yet, everything stock with motor detection, batt max 28 and min -12. I was running FOC sensored on a 400 watt motor, battery is 7S3P panasonic 18650. I'm never buying enertion products again.
```

---
## \#1384 Posted by: Jinra Posted at: 2017-08-09T19:54:55.172Z Reads: 195

```
This is the first time I've heard of a burnt DRV on the FOCBOX, interesting.
```

---
## \#1385 Posted by: guyguy Posted at: 2017-08-09T19:57:33.102Z Reads: 196

```
I've broken belts on both the slave motor and master motor while riding with traction control. From my experience, when the slave belt breaks it still works fine. When the master belt breaks, it's pretty dangerous and unpredictable - sometimes applying brakes to the slave at weird times and it's unable to go full rpm..
```

---
## \#1386 Posted by: scepterr Posted at: 2017-08-09T19:57:47.252Z Reads: 200

```
HW version on mine is 1.6 if that makes a diff
```

---
## \#1387 Posted by: Maxid Posted at: 2017-08-09T20:12:49.356Z Reads: 204

```
Why would you not just revert back to the standard firmware before contacting the support? Doesn't the VESC allow that when the DrV is burned? I thought it's possible.
```

---
## \#1388 Posted by: scepterr Posted at: 2017-08-09T21:36:38.102Z Reads: 208

```
Don't know, maybe. I was just being honest with them. Guess that was my mistake, I believed the hype in all their videos about quality and customer service. I think regardless of what I said they would've found a reason to make me buy the plat warranty.
```

---
## \#1389 Posted by: Titoxd10001 Posted at: 2017-08-10T08:17:33.542Z Reads: 216

```
So the question becomes is traction control a feature worth having since Y splitter would probably be safer.
```

---
## \#1390 Posted by: philvanzu Posted at: 2017-08-10T09:12:12.942Z Reads: 228

```
First a big thank you for this awesome firmware. I installed 2 vescs on my Leiftech, set it up in watt no reverse with break  mode and I must say it really unleashed my riding.

When I first set it up I had a weird issue though, not sure if it could be due to the firmware or something else but since I resolved it by tweaking just one firmware setting I thought it would probably be good to let you know about it.

My master motor was stuttering a bit at low throttle while the slave motor was running smoothly. Increasing the throttle past a certain point and both motors were running right.
[https://youtu.be/Ln4v_Jo1ETs](https://youtu.be/Ln4v_Jo1ETs)


This was with traction control disactivated. The issue disappeared when I tried to activate it. I then rode one hour with traction control, then I disactivated it again and the problem did not reappear. I've ridden for 5 days now without any other issue.

some screenshots from the master vesc settings : 
[https://s1.postimg.org/7uv5ucle4v/motor.png](https://s1.postimg.org/7uv5ucle4v/motor.png)
I'm aware I'd forgotten to setup the battery cutoffs
[https://s1.postimg.org/4awgqdc633/bldc.png](https://s1.postimg.org/4awgqdc633/bldc.png)
[https://s1.postimg.org/4ktrr6edov/app.png](https://s1.postimg.org/4ktrr6edov/app.png)
[https://s1.postimg.org/72v1qsbaof/ppm.png](https://s1.postimg.org/72v1qsbaof/ppm.png)

I did not try running the motors with the stock firmware previously so I have no Idea if this is firmware related. Just wondering where this could be coming from.
```

---
## \#1391 Posted by: caustin Posted at: 2017-08-10T13:06:15.675Z Reads: 215

```
Shot in the dark as dont see all your settings, if using Canbus instead of split PPM did you set slave VESC to send status over CAN?
```

---
## \#1392 Posted by: philvanzu Posted at: 2017-08-10T13:16:51.514Z Reads: 223

```
Yes the slave sent status over can and no split PPM. The issue only appeared on the motor connected to the master VESC. I did not think about filming the realtime plot, I would have if the issue had not disappeared after my first shot at troubleshooting, which was to enable traction control. There was no fault reported. At the time I thought it more probable that it was caused by a bad slipring connection (I had just sanded and painted the extension patch right next to the slipring cover), but since the issue disappeared just by enabling traction control I think that hypothesis less probable.
```

---
## \#1393 Posted by: MontPierre Posted at: 2017-08-10T15:47:32.725Z Reads: 225

```
Donated ! Amazing work @Ackmaniac ! Thanks !
```

---
## \#1395 Posted by: pshaw Posted at: 2017-08-13T18:10:56.476Z Reads: 222

```
Can someone clarify why you would want to limit watts? Right now I have mine maxed at 1300w and I wonder if I'm hindering my top speed. 

Also on hybrid mode I'm getting one motor spinning up way slower than the other. I'm fairly sure that I calibrated correctly. Maybe just motor positioning in between the phases creating a discrepancy? Maybe activating traction control would help?
```

---
## \#1396 Posted by: Jinra Posted at: 2017-08-13T18:13:38.170Z Reads: 216

```
You're capping your max power output, but not top speed (unless power is not sufficient to get to said speed). I don't see any reason to cap power output myself, so I don't use it. I don't think the motor spinning up slower has anything to do with hybrid mode, but have you tested it on the other two (sensored/unsensored) modes?
```

---
## \#1397 Posted by: pshaw Posted at: 2017-08-13T19:06:04.046Z Reads: 220

```
I wonder if my 12s dual 6374 setup even comes close to pulling 1300w per motor anyhow. I'll uncheck the limit and see what happens as my top speed so far has been 34mph (GPS) and that could've been on a slight downhill IIRC. The calc says 35.4 seen here.... anyone know what the rider weight factored into this calc is?

<img src="/uploads/db1493/original/3X/7/5/75ebec10f50cf1450b22b26a8ed99d19e0a3347f.png" width="690" height="353">

As far as the motors not starting at the same time I wasn't saying it had anything to do with hybrid mode. All that means I guess is that sensored BLDC it does this. It probably would be a good idea to try FOC and see if it does it as well. Might be me calibrating in the wrong order or something. Also something to note... I did it with the belts off, as obviously belt tension can be an outside factor.
```

---
## \#1398 Posted by: Jinra Posted at: 2017-08-13T19:08:40.812Z Reads: 207

```
That's what efficiency is for. You only can guess what the top speed might be and the calc only displays top theoretical speed. Looks like you're pretty on target though. Pretty sure you won't be getting any difference in top speed. You will pull a lot of watts when hard accelerating or climbing hills, but at speed, you're pulling a lot less current, and thus, wattage.
```

---
## \#1399 Posted by: Quezacotl Posted at: 2017-08-14T10:31:00.054Z Reads: 208

```
Any help?
I tried uploading your firmware with your BLDC Tool, but when i have uploaded it, it acts like nothing has happened. It just says that too old firmware. And i have confirmed that it still has the old firmware in it, since it works just like before.
Same thing with Linux or Windows versions and Vedder's version.
```

---
## \#1400 Posted by: Ackmaniac Posted at: 2017-08-14T10:33:53.730Z Reads: 206

```
Seems that you have a Maytech VESC. So you would need a STMLink to install the bootloader
```

---
## \#1401 Posted by: Quezacotl Posted at: 2017-08-14T11:36:13.888Z Reads: 201

```
EDIT: Oh, i couldn't even imagine that a device can work without an bootloader. Strange that it isn't installed by default...
```

---
## \#1402 Posted by: trampa Posted at: 2017-08-14T11:51:38.647Z Reads: 214

```
No it's not the exact same! Manufacturers make people believe its the same, by calling it the same. Many VESC-based controllers use cheap components to save some $ in production. The design of the VESC by Benjamin Vedder doesn't like that. In addition some Manufacturers don't install the boot loader, so customers can't easily drop on different FW. 

Vesc-tool will be put soon and it has a bootloader upload funktion, so the ST-Link is not needed in future.

If it's a cheap piece of HW you bought, expect it to 

Frank
```

---
## \#1403 Posted by: pshaw Posted at: 2017-08-14T15:07:26.823Z Reads: 211

```
@Ackmaniac is there a way you could have an odometer built into the esc itself so that you could keep miles logged without having to pair to the bluetooth app?

Right now I'm using the metr app (i have iphone) and the only way I can keep total miles is if it is running while I'm riding.
```

---
## \#1404 Posted by: Ackmaniac Posted at: 2017-08-14T15:29:58.913Z Reads: 215

```
The issue is that the EEPROM storage of the VESC only has a limited amount of writes (roughly 100000). So it would be possible to track it there but if you save for example every 10 meters then the VESC's storage might fail after 1000 km because you reached 100000 write cycles. Next problem is that the EEPROm storage can fail or is very likely to fail when you save the data while the VESC get's disconnected from the battery. Then all the data could be lost. 
So in theory it is possible but it also has some risks.
```

---
## \#1405 Posted by: pshaw Posted at: 2017-08-14T16:22:36.860Z Reads: 210

```
Is there any other way to do this or is that pretty much what would have to happen to be phone free and still log miles?

You don't have an app that works with iphone do you? Right now I'm using the metr app with my bluetooth and the mileage tracking is all over the place. Some times it is accurate others it will say i rode 500 miles in one log.
```

---
## \#1406 Posted by: notger Posted at: 2017-08-14T16:49:41.913Z Reads: 207

```
if its just about logging miles and beeing phone-free:
you could use a SIGMA bike computer with odometer, the can log all kind of stuff and load it into a special training-log-data software via usb-dock.
(if you use a wireless SIGMA you can even mount it onto your remote and have a wireless tacho then, thats what i did)

another fancy possibility would be to install a data logger like the elogger (eagle-tree) or the the unilog (SM) than you could log V,A,Ah,SeaLevel,RPM,Speed,Temperature,............

greets
Notger
```

---
## \#1407 Posted by: pshaw Posted at: 2017-08-15T04:12:39.812Z Reads: 200

```
Info on the sigma setup?
```

---
## \#1408 Posted by: Titoxd10001 Posted at: 2017-08-15T04:42:12.902Z Reads: 206

```
If the wheels spin faster with no load in watt/current mode, wouldn't losing traction make the wheels spin at top speed losing even more traction. I'm pretty sure that's how I ate it going over a slippery surface at slow speeds. And at performance day there was a lot of boards losing traction and I wonder if this mode contributed to the problem.
```

---
## \#1409 Posted by: Jinra Posted at: 2017-08-15T04:51:37.127Z Reads: 209

```
it only goes full speed when of the ground, but once it touches down, load will increase and it'll rotate normally again. Doesn't cause a jolt for me
```

---
## \#1410 Posted by: Titoxd10001 Posted at: 2017-08-15T05:07:10.986Z Reads: 205

```
Once you lose traction wouldn't that pretty much be no load or am I tripping. So if you're in a dirt path just as a example and your wheels start spinning from traction loss wouldn't the wheels want to spin faster
```

---
## \#1411 Posted by: notger Posted at: 2017-08-15T05:28:27.097Z Reads: 210

```
Please read it yourself....
I use this one [http://sigmasport.com/en/produkte/fahrrad-computer/wireless/wireless/bc1416sts](http://sigmasport.com/en/produkte/fahrrad-computer/wireless/wireless/bc1416sts)

It's no Rocket-science, you add a magnet to the wheel, a odometer to the Truck and the Display to ?? yourself. Then you would need the usb docking station from Sigma to read the data from the Bike-Computer (or i think a smartphone would also work to read teh data via bluetooh)
```

---
## \#1412 Posted by: Jinra Posted at: 2017-08-15T05:33:38.958Z Reads: 203

```
yea but current at that point is low, once load returns current will still be low so it shouldn't cause an issues
```

---
## \#1413 Posted by: Titoxd10001 Posted at: 2017-08-15T06:04:05.442Z Reads: 207

```
Once traction is lost on dirt with urethane it's not easily regained. So if you're not expecting loss of traction and you're still on the throttle the wheels could potentially spin faster which means even less traction.
```

---
## \#1414 Posted by: L3chef Posted at: 2017-08-16T18:34:14.088Z Reads: 208

```
Broke the can receiver on one of my vesc. replaced the chip, and now when I try to do "can fwd" bldc shows "no firmware can be read/load ) something like that. Any thoughts?
```

---
## \#1415 Posted by: Ackmaniac Posted at: 2017-08-16T20:18:05.147Z Reads: 208

```
Did you also Set the correct controller id of the slave?
```

---
## \#1416 Posted by: L3chef Posted at: 2017-08-17T03:37:27.382Z Reads: 211

```
Yup. Master 0 slave 1
Tried swapping vesc as master/slave also
```

---
## \#1417 Posted by: Ackmaniac Posted at: 2017-08-17T07:46:55.107Z Reads: 211

```
I mean when you try to connect via CAN. So that you choose which controllerid you want connect to.
```

---
## \#1418 Posted by: L3chef Posted at: 2017-08-17T08:05:12.707Z Reads: 213

```
Ah, yess I did. It's stays connected to bldc tool until I activate the Can fwd. After that it takes a couple of seconds and the red "no firmware read response" shows up. 
It might disconnect the vesc from bldc tool after can fwd is checked. Not 100% sure if it did tho.
```

---
## \#1419 Posted by: Pimousse Posted at: 2017-08-18T11:07:27.040Z Reads: 212

```
Hi @Ackmaniac, hope you'rz fine !
I just come back from a road trip and first thing to do : ride an eBoard !! :smile:

Did you change something to the BT communication ? (sorry, but again, no logfile of your app so couldn't check by myself :yum: )
My phone still can detect my board in the BT menu but not your app anymore.

Also, I've been asked by french guys about having notification/vibration/alarm when the battery is running slow.
We talked about that and AFAIR, you were maybe considering to implement it. Is it still in your TODO list ? 

Finally, FYI, a french guy is currently writing an app just for iPhone for having monitoring info.
Maybe you could be in touch with him to provide more detail of your custom comm. protocol to implement also mode switch ;)
http://www.e-sk8.fr/forum/viewtopic.php?f=25&t=2050&start=10#p53242
```

---
## \#1420 Posted by: pshaw Posted at: 2017-08-21T01:22:11.743Z Reads: 210

```
 I am using hybrid sensored mode and when I set it up I calibrate FOC first no issues. Then go over to BLDC tab to calibrate and when I do it says hall section sensor failed. 

How does it see them and work in FOC calibration but not BLDC? 

Also can you run calibration through can forwarding or do you have to plug into each individual esc?
```

---
## \#1421 Posted by: Ackmaniac Posted at: 2017-08-21T07:32:56.341Z Reads: 208

```
The reaosn for that ismostly that the sensors for hall are not really well positioned. FOC is less sensitive than BLDC when it comes to hall detetction. Also had a bad motor once which had the same behavior. 
Just simply change to phase wires so that the motor runs in the opposite direction and do the BLDC detection again. Mostly it works then. 

And you can do the detection via CAN.
```

---
## \#1422 Posted by: pshaw Posted at: 2017-08-21T11:28:30.608Z Reads: 209

```
So if you detect in BLDC and it says failed for hall and you select hybrid... is it really not using the sensors in the first half because dectection failed?

So swap wires so it runs backwards then have it detect then just swap wires with no re calibration once it's spinning the right way?
```

---
## \#1423 Posted by: Ackmaniac Posted at: 2017-08-21T12:18:54.116Z Reads: 205

```
No. It doesn't help if the detection fails in the direction you want it to spin. Finally the hall sensors are not at the correct position.

And you need correct identified hall sensor positions to run in hybrid mode. Otherwise it doesn't work.
```

---
## \#1424 Posted by: ThierryGTLTS Posted at: 2017-08-22T17:10:07.869Z Reads: 206

```
Hi Ackmaniac,

Good job, well implemented :slight_smile:

Do you think it would be possible to implement "Watt Control Mode" for ADC input, because I wanna use wired throttle or wired rotation detection for an e-bike project ?!

I don't wanna use PPM because I prefer wire connexion.

Have a Nice Day.

Thierry
```

---
## \#1425 Posted by: pshaw Posted at: 2017-08-22T22:51:44.050Z Reads: 204

```
[quote="Ackmaniac, post:1423, topic:12286, full:true"]
No. It doesn't help if the detection fails in the direction you want it to spin. Finally the hall sensors are not at the correct position.

And you need correct identified hall sensor positions to run in hybrid mode. Otherwise it doesn't work.
[/quote]

So even if hall detection works in FOC, when trying to setup Hybrid if both escs dont say hall sensors detected under the BLDC tab when running BLDC calibration it'll just essentially run unsensored BLDC even if Hybrid is still checked?
```

---
## \#1426 Posted by: Ackmaniac Posted at: 2017-08-23T00:02:15.487Z Reads: 200

```
Each Vesc handles that for its own. For example you could run one Motor in BLDC in the other in FOC or  hybrid and sensorless.
```

---
## \#1427 Posted by: rich Posted at: 2017-08-23T15:45:27.569Z Reads: 203

```
@pshaw I had the same with one motor, after switching 2 phase wires the hall sensor worked. But why you want to setup FOC and BLDC? Many people fry it by switching modes. Best is to reupload FW and set up one mode not both. Anyway, when you use sensored motors you need FOC not BLDC!
```

---
## \#1428 Posted by: Ackmaniac Posted at: 2017-08-23T15:51:12.512Z Reads: 207

```
You should get completely naked if you want to change your shoes. Otherwise you will break your leg. Because many people broke their leg after they changed shoes and didn't get naked before.
And sensored works in BLDC and FOC.
```

---
## \#1429 Posted by: SeanHacker Posted at: 2017-08-23T16:08:55.643Z Reads: 209

```
I'm using sensored (Hybrid) with bldc just fine. Been using this firmware/app since release because of watt control. 

@Ackmaniac 
Great job on the app. It's turned out really nice!!!
```

---
## \#1430 Posted by: rich Posted at: 2017-08-23T16:26:27.389Z Reads: 217

```
[quote="Ackmaniac, post:1428, topic:12286"]
You should get completely naked if you want to change your shoes. Otherwise you will break your leg
[/quote]

True, i can confirm that :joy:
But joking aside, i was f***** around with hybrid BLDC for weeks and my sensored motors were cogging and jittering only at startup. Vedder suggested me to use FOC because of better hall sensor implementation what I did. It works like a charm now and for my motors FOC is the only solution. Let's get naked......
```

---
## \#1431 Posted by: Ackmaniac Posted at: 2017-08-23T21:28:21.109Z Reads: 215

```
As said before. I made that experience with badly placed hall sensors. If they are placed well then BLDC hybrid works. Best indicator for this is when sensor detection in BLDC only works in one direction.

And the firmware flashing is a myth. If you want to be sure nothing can get fucked a reboot after you wrote the settings is enough. But even that isn't needed.
```

---
## \#1432 Posted by: rich Posted at: 2017-08-23T21:52:14.340Z Reads: 219

```
That's interesting because I have trampa motors (€€€) and don't expect badly placed hall sensors on them. I've tried it with sensored maytech motor, too but with no difference (motors tested with all 6 possible phase wire combinations). Also I've read that several people have this cogging problem at startup with sensored motors in BLDC hybrid mode. All the builds with smooth startup I've seen running sensored FOC. But I'm glad to hear that there are people out there where it works!

Ok, let's burn the firmware flashing myth :boom: if you say so
```

---
## \#1433 Posted by: ThierryGTLTS Posted at: 2017-08-25T16:58:48.724Z Reads: 220

```
Hi Ackmaniack,

Do you think it would be easily possible to implement "Watt Control Mode" in the ADC Tab?

I've a lot of knowledge about hardware, but software is not my cup of tea :-)


Have a Nice Day.

Thierry
```

---
## \#1434 Posted by: RiGo Posted at: 2017-08-31T13:45:39.201Z Reads: 233

```
Hi @Ackmaniac. After discovering that I bought an incompatible HM-10 clone BT module, I'm now about to buy this one:

http://www.ebay.com.au/itm/KEYES-HM-10-6-Pin-BLE-Bluetooth-V4-0-Serial-Port-Module-Logic-Level-Translator-/132242503974?hash=item1eca447926:g:VMgAAOSwFJBZU57g

This is supposed to be the original HM-10 but I just want to make 100% sure that this will work with your firmware and android app. Could you please confirm?

Also, will I be able to connect to it using the BLDC tool on my Mac?

Thanks!
```

---
## \#1435 Posted by: Ackmaniac Posted at: 2017-08-31T14:35:30.887Z Reads: 225

```
I recommend the clones from my link i shard in the first post of this thread. They are cheap and work. I changed the timing a little in my firmware so that the module you posted also should work (which also seems to be a clone). 
So if you use my firmware mod then you should be able to connect. (At least if you have a decent smartphone that supports Bluetooth Low Energy properly)

But you can't use it to connect to your MAC. That simply isn't supported.
```

---
## \#1436 Posted by: Jaydan Posted at: 2017-09-02T19:41:36.339Z Reads: 218

```
can't believe i did this but i read all of the 1401 previous posts. this thread is pure awesomeness!! :heart_eyes:
i did not yet have the opportunity to ride my board with the updated firmware but ever since the update i've got a strange tingling sensation in my fingers..

@Ackmaniac is it possible to reboot the vesc using the app? as a fellow german i'm concerned about the police stopping me and in that case, a simple touch or swipe on my smartphone is a lot less suspicious as replugging a loop key.
```

---
## \#1437 Posted by: Ackmaniac Posted at: 2017-09-02T20:19:54.290Z Reads: 213

```
Simply create a mode that you want. For example 6 km/h max and activate it with 1 click
```

---
## \#1438 Posted by: Jaydan Posted at: 2017-09-02T20:32:44.663Z Reads: 211

```
maybe i should have taken the board for a spin before asking this question. just realised i haven't messed with switching modes yet. but if it's really as simple as you say it is: you are my hero!

edit: donation is on its way
```

---
## \#1439 Posted by: Vanarian Posted at: 2017-09-05T08:06:19.070Z Reads: 202

```
@Ackmaniac Yo~ can't wait to see your control mods done in new VESC Tool and new firmwares! When do you think you'll get it running? 

Cheers
```

---
## \#1440 Posted by: MontPierre Posted at: 2017-09-05T08:34:11.348Z Reads: 219

```
I second that! Can't wait !
```

---
## \#1441 Posted by: Ackmaniac Posted at: 2017-09-05T09:52:09.184Z Reads: 224

```
Just had a quick look and i am happy to see that Watt control is already implemented. So when you use the Current Control of the new VESC-Tool you are actually using Watt Control.
```

---
## \#1442 Posted by: i2oadsweepei2 Posted at: 2017-09-05T12:40:14.369Z Reads: 223

```
Does that mean you won't need to make a new extended vesc tool? Will it work now with 2.54?
```

---
## \#1443 Posted by: Ackmaniac Posted at: 2017-09-05T13:08:36.497Z Reads: 227

```
No no no no no no no. Watt control isn't the only thing i have changed. And it won't work with 2.54.
Need to make a lot of changes to implement all the stuff. Let's see when i find some time.
```

---
## \#1444 Posted by: i2oadsweepei2 Posted at: 2017-09-05T13:13:08.766Z Reads: 227

```
Thank you for the reply. I will watch this thread and send you some motivational $$love$$ for your hard work. Thank you
```

---
## \#1445 Posted by: guyguy Posted at: 2017-09-05T14:53:24.173Z Reads: 254

```
Looking forward to seeing your roadmap here with the release of vesc-tool. 

Are you going to be continuing to update the 2.xx firmware or will you be hopping to the 3.xx that was released with the VESC-Tool? Would you be building off the Vesc-Tool? The biggest selling point to me for staying on your FW is working with the phone app. 

Thank you for all you've done.
```

---
## \#1446 Posted by: emmaanuel Posted at: 2017-09-05T18:23:49.057Z Reads: 268

```
Hi everybody, 
I know that a lot of iPhone users were looking for this, so I've published a new iOS app for VESC with Vedder and Ackmaniac firmware.

<img src="/uploads/db1493/original/3X/d/a/da8d44a6cb924c5a0723c8cece58904a8f091206.PNG" width="281" height="499">

[Apple Store Link](http://www.electric-skateboard.builders/t/new-ios-app-eskate-vesc-for-standard-and-ackmaniac-fw/32340)

[http://www.electric-skateboard.builders/t/new-ios-app-eskate-vesc-for-standard-and-ackmaniac-fw/32340](http://www.electric-skateboard.builders/t/new-ios-app-eskate-vesc-for-standard-and-ackmaniac-fw/32340)
```

---
## \#1447 Posted by: Mickyboy Posted at: 2017-09-05T22:46:14.269Z Reads: 244

```
Great work. Just downloaded. Looking forward to trying it. Maybe you can make it compatible with Apple Watch?
```

---
## \#1448 Posted by: emmaanuel Posted at: 2017-09-06T06:44:05.390Z Reads: 239

```
Thank you.
Yes for the watch I'm thinking about it.
```

---
## \#1449 Posted by: Mickyboy Posted at: 2017-09-06T07:23:11.061Z Reads: 239

```
Just tried it out for the first time on the Raptor 2. Seems to connect okay, but speed is off, like 2x actual speed. I have the teeth settings at 1 for motor and 1 for pulley (hub motor), does that make a difference? Also what should my 'Poles Number' setting be? 14?
In the main screen, 'battery %' and 'remaining range' would be something good to include.
```

---
## \#1450 Posted by: MontPierre Posted at: 2017-09-06T11:59:14.802Z Reads: 246

```
@Mickyboy Are you taking about @Ackmaniac software or @emmaanuel??? 

This thread is about @Ackmaniac work, if you wish to comment on @emmaanuel stuff please comment on his thread! Simple!
```

---
## \#1451 Posted by: Quezacotl Posted at: 2017-09-06T13:42:46.564Z Reads: 236

```
Hello!

I got now two FOCBOXes with two hub motors. It works good with FOC.
I updated the firmware to yours, and appears to be working, so is the android app.

One thing that seems to not work, is different modes on the android app. Whatever i change, doesn't make any effect. Even limiting watts to like 10W or anything crazy doesn't make any difference.
I tap the mode, and choose a mode, and then it should be applied?
(Phone is rooted, but that should not affect?)
```

---
## \#1452 Posted by: Ackmaniac Posted at: 2017-09-06T13:46:07.561Z Reads: 231

```
Which phone do you have. Seems that bluetooth low energy isn't implemented well in the firmware of the phone. Do me a favour and try to change the mode with another phone.
```

---
## \#1453 Posted by: Quezacotl Posted at: 2017-09-06T13:49:22.544Z Reads: 235

```
Oneplus One with Lineage ROM and Boeffla kernel.
I will try with my tablet tomorrow.
```

---
## \#1454 Posted by: Mickyboy Posted at: 2017-09-06T21:05:13.510Z Reads: 231

```
I had the exact same issue a few weeks ago. Changed phone, problem solved.
```

---
## \#1455 Posted by: Quezacotl Posted at: 2017-09-07T12:26:04.094Z Reads: 245

```
Okay, i tried with Honor 6 phone and some Lenovo tablet also. Exactly same behavior.
<img src="/uploads/db1493/original/3X/f/1/f14e60ae45210c97f95e82bb2180bb0ad46d4c75.png" width="281" height="500">
Also i noticed, on mode box, it says "Disabled" all the time, while i think it should say about the throttle mode, like "Watt".
```

---
## \#1456 Posted by: Ackmaniac Posted at: 2017-09-07T12:29:31.461Z Reads: 221

```
You have to disable send can status at the master. Please let me know if that solved it?
```

---
## \#1457 Posted by: Quezacotl Posted at: 2017-09-07T15:36:10.642Z Reads: 228

```
It is already disabled. I verified also to make sure. And if those settings are wrong, the motors wouldn't sync correctly, which they do.
```

---
## \#1458 Posted by: Ackmaniac Posted at: 2017-09-07T15:39:03.073Z Reads: 232

```
If can status is enabled at the master it has no effect for the slave. So you would not notice that it is enabled or disabled. But the app needs it to identify the master. And if you attached the module to the slave you need to activate forward to can with the id of the master in the settings of the app.
```

---
## \#1459 Posted by: Quezacotl Posted at: 2017-09-07T17:25:55.054Z Reads: 241

```
Ohh.. that is it. I do have the BT module at the slave. I'll try that forward setting as soon as i get home to test it.
EDIT: Yep, now it works perfectly. The curves work and all settings i have tried so far.

Thank you! It is a very good firmware and applications.
```

---
## \#1460 Posted by: Sebike Posted at: 2017-09-07T17:44:42.447Z Reads: 246

```
I installed the extended BLDC-tool from @Ackmaniac and run FOC on my single drive 190 kv 6374, FOCBOX, 10s board. I took it for its first few drives today and experienced a lot of brake loss. 

This happened more at higher speeds where I didn't get any reponse from the motor when pulling the brake on the remote. Sometimes it brakes after after 1-2 seconds if I keep pulling, or if I let go and try again a few times, then it applies the braking. 

The remote is a FlySky GT2B with the Sparkle mod. Battery was at 40,5 after the first ride, but it happened after that as well. Didn't check battery voltage after last ride. 

Any ideas?
```

---
## \#1461 Posted by: RiGo Posted at: 2017-09-07T22:26:56.576Z Reads: 240

```
@Ackmaniac how will your development of this firmware be affected by the release of the new VESC tool?
```

---
## \#1462 Posted by: mmaner Posted at: 2017-09-07T22:29:55.508Z Reads: 244

```
I think the biggest development hurdle that @Ackmaniac is facing is all the capabilities he created have been co-opted and put into the VESC6 :slight_smile:.
```

---
## \#1463 Posted by: Deakbannok Posted at: 2017-09-11T14:46:37.398Z Reads: 240

```
Yes. the new VESC Tools have these function now.
But he* is the first implement of these ideas
Thanks to him and of all his time and efforts putting these together for us.

I will stick with 2.54 for awhile, and havent had problem with it.
 since the vesc version is still new. dont want to risk for an unknow glitches when I am cruise 40km+.
```

---
## \#1464 Posted by: pshaw Posted at: 2017-09-12T20:52:26.868Z Reads: 246

```
Is there any way I'm actually ever hitting the 1300w max I have capped. I was thinking about taking the cap off but figure it might do no good as I'm never actually hitting that.... 

12s4p / dual 6374 190kv / 97mm street wheels 

Thoughts?
```

---
## \#1465 Posted by: RiGo Posted at: 2017-09-13T06:59:50.125Z Reads: 247

```
[quote="RiGo, post:1461, topic:12286, full:true"]
@Ackmaniac how will your development of this firmware be affected by the release of the new VESC tool?
[/quote]

Hey @Ackmaniac. I love your app and would like to donate, but first I'd like to find out what's happening to development following the release of the new VESC tool?
```

---
## \#1466 Posted by: Ackmaniac Posted at: 2017-09-13T10:56:40.131Z Reads: 247

```
It's on my to do list when i find the time.
```

---
## \#1467 Posted by: GrecoMan Posted at: 2017-09-13T10:58:13.876Z Reads: 256

```
I switched to fw 3.24 yesterday and couldn’t stand it!  Thanks @Ackmaniac for spoiling me, I’ve switched back to your fw 😜
```

---
## \#1468 Posted by: BigBoyToys Posted at: 2017-09-14T02:58:51.048Z Reads: 255

```
The only thing I really need from FW 3.26 is the motor temp controls. I know its already on his todo list as well so Ill just be patient.
```

---
## \#1470 Posted by: Titoxd10001 Posted at: 2017-09-17T02:31:29.024Z Reads: 251

```
Now that vesc-tool came out are you going focus on that or will you make changes to bldc-tool. Kind of dislike vesc-tool just so many tabs to switch to. Not a huge deal but just wondering. 
Also if you have a chance can you take a look at duty cycle mode. From what understood vedder said it won't work on a vesc. But someone on the forum said it works for them (with neutral) presumably on vesc-6. Is there a reason it wouldn't work on a focbox?
```

---
## \#1471 Posted by: Eboosted Posted at: 2017-09-20T06:08:29.973Z Reads: 248

```
@ackmaniac can't wait for your FW with the new VESC tool, have you tried to contact Benjamin to partner with him?
```

---
## \#1472 Posted by: banjaxxed Posted at: 2017-09-22T06:42:58.346Z Reads: 246

```
Don't see that happening
```

---
## \#1473 Posted by: SeanHacker Posted at: 2017-09-24T00:07:44.187Z Reads: 244

```
He started submitting patches to Vedders git. https://github.com/vedderb/vesc_tool/commits/master
```

---
## \#1474 Posted by: Nexo Posted at: 2017-09-25T08:19:59.037Z Reads: 244

```
hi there :slight_smile:
is it possible to connect vesc and android phone with USB cable via USB OTG connection?
```

---
## \#1475 Posted by: Pimousse Posted at: 2017-09-25T08:50:18.265Z Reads: 246

```
Sure.
But there is no application for using this kind of connection.
```

---
## \#1476 Posted by: scepterr Posted at: 2017-09-25T12:15:53.958Z Reads: 255

```
Hey, is there a changelog for the Android app?
I'm trying to track down a change of behavior, not sure if it's the app or os...app doesn't stay active, impossible to log a full ride unless I keep phone awake and app open.
```

---
## \#1477 Posted by: ninja Posted at: 2017-09-25T20:52:06.859Z Reads: 265

```
Hi!
@Ackmaniac I found that my board eats more amps that I had written in bldc tool. How does it come? Here is an example from one short ride. There is 70A  mot max in mode, but on the ride mot max is 81.2A.
<img src="/uploads/db1493/original/3X/3/c/3c33a3612c7b891974d497e1782e3e68ad09af75.png" width="281" height="500">

Also it's just me or somebody have the same issue as me?: when I want to switch modes, sometimes it is very annoying to click many times on desired mode to get it. I've tried short click, long holding on click, double click. The best works long holding click, but even then sometimes I need to redo it at least 5 times to realy switch to my wanted mode from my default mode.
```

---
## \#1478 Posted by: Ackmaniac Posted at: 2017-09-25T20:55:36.736Z Reads: 244

```
I guess you have a dual drive. In that case if you selected 2 motors in the app then the values like motor amps, battery amps and watts get doubled. So that you see how many amps and watts the entire system uses.

And the problem of clicking many times can be causes by bad bluetooth module clones or a smartphone with a bad bluetooth low energy implementation.
```

---
## \#1479 Posted by: ninja Posted at: 2017-09-25T20:59:41.283Z Reads: 243

```
Ok thanx. 
Module is from link you suggested. 
Phone is Samsung Galaxy J3.
And I have single drive.
```

---
## \#1480 Posted by: landonkun Posted at: 2017-09-25T21:21:30.115Z Reads: 253

```
Hi @Ackmaniac !
For months now, I've been unable to use your firmware because I had a bootloader-less Maytech :frowning:
I did buy a ST-link, but didn't have the right cable and was too lazy to bother with it.

Now that the Vesc-tool comes with a bootloader, is it possible to use the vesc-tool to upload your custom firmware, then switch to your extended BLDC-tool?
```

---
## \#1481 Posted by: Ackmaniac Posted at: 2017-09-25T23:08:40.669Z Reads: 245

```
Think that should be possible.
```

---
## \#1482 Posted by: Ackmaniac Posted at: 2017-09-25T23:15:39.471Z Reads: 254

```
Then the VESC overshoots the aimed current. That is the reason that the absolute max limit is needed.
At the end the VESC controles the voltage of the motor. The higher the difference between the motors actual own voltage and the Voltage the VESC feeds the motor is the more amps it generates. 
So the VESC increases and decreases the voltge to try to stay in the correct limit to produce the correct amount of amps. But sometimes it overshoots a little. And the higher the amps the higher the risk of an overshoot. 
The VESC does this regulation a couple of thousand times a second. So if the values are detected in a bad moment then you can see higher amps.

But as long as you don't see overcurrent errors it is fine.
```

---
## \#1483 Posted by: landonkun Posted at: 2017-09-26T02:43:41.980Z Reads: 242

```
I successfully used the Vesc-tool to upload a bootloader to my Maytech vesc, then upload your custom firmware. I then switched over to your tool and got everything set up no problem!

And oh my gosh. The watt control mode is beautiful! Thank you so much for this firmware :slight_smile:
```

---
## \#1484 Posted by: Deckoz Posted at: 2017-09-26T04:09:10.066Z Reads: 241

```
Android system battery settings -> battery optimization, find vesc monitor, disable battery optimization for the app
```

---
## \#1485 Posted by: scepterr Posted at: 2017-09-26T04:12:18.636Z Reads: 242

```
I've tweaked every os setting, pinned it, etc...
I'm about to tweak the manifest to make it a system app lol
```

---
## \#1487 Posted by: ninja Posted at: 2017-09-27T21:30:40.605Z Reads: 266

```
Today I tested abit my board. So that problem with multiple clicking on modes to set them- you were absolutelly right. it's my smart phone. I tried with my girlfriend's phone and it worked like charm. I also read somewhere that samsung galaxy J3 has problems with bluetooth low energy. So I picked wrong phone, damn it :disappointed:

and other thing- now I had overcurrent error. see pictures:

<img src="/uploads/db1493/original/3X/3/6/367f0cc9ff14675dc8a33a8657d0fee1dbdabdb3.jpg" width="300" height="500">

<img src="/uploads/db1493/original/3X/5/c/5c575dca0a2913d6d7bbea90d508e3c06b685831.jpg" width="300" height="500">

could it be from hard braking? I had one hard braking where brakes was lost in the end for maybe second, but it also could be my receiver, it is a bit damaged i ordered new one. 

Aso is it o.k. that motor current stays at some 0,22A when board stay still, while batt current stays at 0A?
```

---
## \#1488 Posted by: notger Posted at: 2017-09-29T17:04:49.433Z Reads: 253

```

[quote="Ackmaniac, post:5, topic:12286"]
am working also on other stuff at the moment which allows you to change the mode at any time via APP or the remote.
[/quote]

so the app is done but is there actually any option to quickly change power modes via ppm (rc-remote)  ? 
like the cruise control on dual vesc-setup using a second channel for power mode change ?

greets notger

ah, and actualy i love this firmware, i did allready update to the new vesx-tool firmware, but switched back to your firmware cause of the "brake, double-trigger reverse" function, otherwise reverse  with ppm is useless in my opinion
```

---
## \#1489 Posted by: Pimousse Posted at: 2017-09-29T17:24:23.097Z Reads: 259

```
@Ackmaniac, Itried the new version with battery profiles. Selecting Lipo, there is no value for 70%.<img src="/uploads/db1493/original/3X/2/9/29c8914c340883c90bac831fc0b4f069b80e04a8.jpg" width="281" height="500"> 

Also a typo "Costum" instead of "Custom".
```

---
## \#1490 Posted by: Ackmaniac Posted at: 2017-09-29T17:29:25.642Z Reads: 244

```
Did you Update to the latest Version? I think I fixed that issue already
```

---
## \#1491 Posted by: Ackmaniac Posted at: 2017-09-29T17:30:59.654Z Reads: 250

```
I thought about that before but it would be hard to store and manage multiple different modes on the VESC itself.
```

---
## \#1492 Posted by: Pimousse Posted at: 2017-09-29T17:31:20.725Z Reads: 253

```
I think so (1.57). At least, Play Store don't offer any update
```

---
## \#1493 Posted by: notger Posted at: 2017-09-29T23:10:59.071Z Reads: 253

```
and what about just changing one Value (via ppm signal) like MaxWatts ?
```

---
## \#1494 Posted by: Bloop Posted at: 2017-09-30T05:45:52.534Z Reads: 259

```
Hey if i run dual setup i should halve all the values from Current Limits? I saw in @Ackmaniac tool that only for batt max and bat min is the tooltip with "If you have 2 vesc you should halve that value"

But yeah im not sure about motor max. if i have a motor that supports 80A i should get it to 70 or keep it at 40 or .. ? 

Also if i set the watt mode and set max watt to 3000W the current settings like mot max still apply ?

Thank you
```

---
## \#1495 Posted by: i2oadsweepei2 Posted at: 2017-09-30T13:05:31.493Z Reads: 260

```
The watt values should add up with the max battery current on each vesc. If li-ions are used and your battery/bms can handle 80 amps then 3.6v x 10s x 40 amp = 1440 watts per vesc. If your max battery is set to 30a or 20a on each vesc then use the same formula. If you were using a single setup then you could set the battery max higher to match the battery's max continuous output keeping in mind the limit of the bms if one is used. You don't have to set max values for watts. That is a lot of power. Best to be conservative at first.

Be safe.
```

---
## \#1496 Posted by: notger Posted at: 2017-09-30T19:05:20.348Z Reads: 275

```
[quote="Ackmaniac, post:1491, topic:12286, full:true"]
I thought about that before but it would be hard to store and manage multiple different modes on the VESC itself.
[/quote]

Hmm, ould be really nice to couple up with @Wajdi and his [http://www.electric-skateboard.builders/t/universal-advanced-vesc-remote-control-custom-design/24654/153](http://www.electric-skateboard.builders/t/universal-advanced-vesc-remote-control-custom-design/24654/153) 

teh receiver communicates via UART, and has quite some "brain" left, so it might be possible to send similar data (power change modes or even more) like the smartphone does with your Android VESC app.

!!!
```

---
## \#1497 Posted by: Ackmaniac Posted at: 2017-10-11T17:17:15.810Z Reads: 262

```
Just had a close look and the 70% Battery % parameter  issue is fixed in version 1.59 which i released a minute ago. Thanks for the info.
```

---
## \#1498 Posted by: Snow4us Posted at: 2017-10-12T17:43:01.579Z Reads: 265

```
I'm attempting to flash a Maytech 50a that currently has 2.18 with your (awesome) 2.54.  Im on WIndows 10 using the BLDC tool for 2.54.  When i plug in the VESC, I get the wrong firmware error and then go to the firmware tab, select the "VESC_Ackmaniac_Mod_2_54.bin" file and select upload.  The upload completes and I get "FW Upload Done" message and the VESC disconnects.  When I try and re-connect, no VESC is detected.  If i power cycle the VESC and then pplug it back in, it reverts to 2.18.  Any idea what is happening and how I can get 2.54 on the VESC? (it's vesion 4.12)

Thanks!
```

---
## \#1499 Posted by: Blasto Posted at: 2017-10-12T17:54:17.711Z Reads: 259

```
[quote="Ackmaniac, post:1007, topic:12286, full:true"]
I think the maytech VESCs have no bootloader installed. So you need a programmer. there is more info on vedders website www.vedder.se
I don't really understand why so many buy the maytech VESCs in the last days.
[/quote]

@Snow4us  no bootloader in maytech vesc
```

---
## \#1500 Posted by: Snow4us Posted at: 2017-10-12T18:07:13.389Z Reads: 262

```
Damn, so I couldn't even flash my other Maytech down to 2.18?  That's a huge bummer.
```

---
## \#1501 Posted by: Snow4us Posted at: 2017-10-12T18:10:53.042Z Reads: 267

```
I have a [UART Cable](https://www.amazon.com/Converter-Terminated-Galileo-BeagleBone-Minnowboard/dp/B06ZYPLFNB/ref=sr_1_11?ie=UTF8&qid=1507831754&sr=8-11&keywords=uart), could this be used to connect to the Maytech?
```

---
## \#1502 Posted by: Snow4us Posted at: 2017-10-12T19:54:27.272Z Reads: 269

```
I think i'm confused is a "bootloader" software?  If so, is there any way to flash a bootloader onto a Maytech VESC?
```

---
## \#1503 Posted by: Silverline Posted at: 2017-10-12T20:05:46.270Z Reads: 269

```
By using the new vesc-tool , you can flash the missing bootloader to your maytech vesc... And then you can fw updated, to what ever fw you like. .
```

---
## \#1504 Posted by: Achmed20 Posted at: 2017-10-12T20:24:55.403Z Reads: 287

```
[quote="Snow4us, post:1502, topic:12286, full:true"]
I think i'm confused is a "bootloader" software?  If so, is there any way to flash a bootloader onto a Maytech VESC?
[/quote]

[quote="Silverline, post:1503, topic:12286, full:true"]
By using the new vesc-tool , you can flash the missing bootloader to your maytech vesc... And then you can fw updated, to what ever fw you like.
[/quote]

well if this works, then you should be fine. however, if it doesnt work, you need this thing here and flash it manualy
https://www.amazon.de/gp/product/B01F37YMJ4/ref=oh_aui_detailpage_o02_s00?ie=UTF8&psc=1
```

---
## \#1505 Posted by: Snow4us Posted at: 2017-10-12T20:27:23.580Z Reads: 265

```
I am only able to find guides using the tool you have linked.   Not able to find i fo on flashing the bootloader from the BLDC tool....
```

---
## \#1506 Posted by: Pimousse Posted at: 2017-10-12T20:34:55.248Z Reads: 270

```
Download VESC Tool instead and upload bootloader from it.
```

---
## \#1507 Posted by: zepton Posted at: 2017-10-31T19:45:07.075Z Reads: 262

```
That is amazing! Well done
```

---
## \#1508 Posted by: scepterr Posted at: 2017-11-09T23:01:55.162Z Reads: 262

```
@Ackmaniac can you post the apk please
```

---
## \#1509 Posted by: zepton Posted at: 2017-11-10T00:48:30.536Z Reads: 271

```
A couple questions/concerns:

1. I just started using the watt mode and feels exactly the same as the current control mode.

2. Sometimes when I ride at full throttle for a while my throttle cuts out, this could be due to voltage sag, however I never had this issue before I started using watt mode and my voltage limits are the same.

3. Is it necessary to buy a separate bluetooth module to use the Android app?
```

---
## \#1510 Posted by: Ackmaniac Posted at: 2017-11-10T11:10:15.046Z Reads: 283

```
1. If you have battery max and motor max at more or less the same values then it will feel very similar. When motor max is higher than batter may then you feel the difference. So if you would show a screenshot of your settings it would be helpful.

2. Don't think that voltage sag causes that, because it would ramp the power down instead f instant loss. I guess your remote looses connection which will lead to instant power loss.

3. Yes you need a HM-10 bluetooth module.
```

---
## \#1511 Posted by: Eboosted Posted at: 2017-11-10T18:21:46.838Z Reads: 290

```
@ackmaniac are you going to support the latest VESC Tool software? I really miss the possibility to change current limits via HM10 bluetooth device for HW4.12
```

---
## \#1512 Posted by: Ackmaniac Posted at: 2017-11-10T18:25:49.353Z Reads: 301

```
I just released already the mod for vesc-tool
```

---
## \#1513 Posted by: Eboosted Posted at: 2017-11-24T04:20:13.592Z Reads: 338

```
[quote="Ackmaniac, post:1512, topic:12286, full:true"]
I just released already the mod for vesc-tool
[/quote]

I uploaded your v2.54 version via the v0.86 bldc tool but it requests to upload a new firmware in order to continue.

Is there a different FW version for VESC Tool v0.86?
```

---
## \#1514 Posted by: Deckoz Posted at: 2017-11-24T05:19:07.039Z Reads: 333

```
@Eboosted 2.54 is BLDC tool

Vesc tool firmwares will be 3.xx

See here
 https://www.electric-skateboard.builders/t/extended-ackmaniac-esc-tool-based-on-vesc-tool/35116
```

---
## \#1515 Posted by: Eboosted Posted at: 2017-11-24T06:34:59.721Z Reads: 333

```
Thanks pal!

I don't know how I missed that!
```

---
## \#1516 Posted by: chrisongtj Posted at: 2017-11-26T10:34:06.075Z Reads: 329

```
I just downloaded the new vesc tool via ackmaniacs Dropbox link and updated my firmware. Is there any way to swap between FOC and BLDC via app? Can't find it
```

---
## \#1517 Posted by: Ackmaniac Posted at: 2017-11-26T14:09:25.460Z Reads: 330

```
When you do a long click on the box where you switch modes it will ask you if you want to store the actual settings as default and the middle button in that screen asks you if you want to change the mode between FOC and BLDC.
```

---
## \#1518 Posted by: neobrain Posted at: 2017-12-03T17:45:15.112Z Reads: 316

```
Hi Ackmaina, first of all, i want to thank u for the work u did.. i like the extended version.. but i do have a topic: iam using a BMS in my Board and the BMS cuts the power to the vescs, when iam brakeing at higher voltage.. so i was looking in ur bldc for the maximum brake voltage. so that the board brake as much as the cells like it and dont hurt them.. my question is do u have a maxmimum voltage for braking ??

Thanks for answering, greets from stuttgart
```

---
## \#1519 Posted by: hackware Posted at: 2017-12-22T00:00:38.348Z Reads: 304

```
Ackmaniac, has anybody tested your code with 4WD...?

Was wondering about 3 slaves on can bus...

I am a lurker on this board because I'm building a robot with 4 10" hoverboard motor-wheels, using VESC as drives...

william...
```

---
## \#1521 Posted by: Fabian287 Posted at: 2018-01-30T22:19:29.654Z Reads: 288

```
@Ackmaniac    is your bldc Tool v. 3.xx with the ArduboardControler and  with the vescuartcontrol compatible by @RollingGecko?
 
 with  v. 2.54  it worked. 

Thanks 

Fabian Langer
```

---
## \#1522 Posted by: Ackmaniac Posted at: 2018-01-31T00:01:51.062Z Reads: 285

```
I did not test it. But the interface changed in the new firmware and rollinggecko has a vesc6 branch which might work.
```

---
## \#1523 Posted by: E-lite Posted at: 2018-02-08T14:15:04.626Z Reads: 269

```
hi guys, I-m making some tests with my sk8 but is it htere a way to have a data logging app that can provide an overlay video of the recorded data over a camera recorded video? I-m looking for it and I can't find it simple to use on windows. thanks

Gabriele
```

---
## \#1524 Posted by: Ackmaniac Posted at: 2018-02-08T15:46:57.527Z Reads: 267

```
You can use my app to make videos with the camera that have integrated overlays.
http://www.electric-skateboard.builders/t/vesc-monitor-android-app/20888?u=ackmaniac
```

---
## \#1525 Posted by: nikoli280 Posted at: 2018-02-19T12:17:08.993Z Reads: 254

```
Isn't it bad to use Watt mode for the VESC? i mean if you have a VESC with max 50A output, using 50A at 36V is   1800W but at 42V its 2100W. So if i set the Watt max to 2000W, then at 34V it would overdo the max VESC with a total of 58A that could destroy the VESC`?
```

---
## \#1526 Posted by: Ackmaniac Posted at: 2018-02-19T14:04:13.448Z Reads: 259

```
All the safety regulations are still active. Max amps has a higher priority than max watts.
```

---
## \#1527 Posted by: nikoli280 Posted at: 2018-02-19T15:00:48.638Z Reads: 257

```
Okay so if i have a VESC with max 50A and a 10S battery i should enter 36V * 50 = 1800W ? and then set the motor max and battery max to 50A?
```

---
## \#1528 Posted by: nikoli280 Posted at: 2018-02-19T16:16:36.989Z Reads: 270

```
Also is the battery  Wh calculated by saying (Cells * nominal voltage * pack capacity) or (Cells * maximum voltage * pack capacity)

its it like this

10 * 3.6V * 12.5Ah = 450Wh 

or like this

10 * 4.2V * 12.5Ah = 525Wh


And can you set the motor max to 80A if that is what the motor is rated at if the VESC can max output 50A?
```

---
## \#1529 Posted by: Ackmaniac Posted at: 2018-02-19T18:03:38.362Z Reads: 288

```
If you are a beginner you can set the motor max to 40 or 60A and the battery max to 50A. Then I would start with 750Watts for each vesc. Later you can go to 80A motor max and raise the watts. 3600 watts total is already plenty for a mid weight driver.

And to calculate what you use 3.6V for Li-Ion and 3.7V for Lipo.
```

---
## \#1530 Posted by: rey8801 Posted at: 2018-02-24T10:44:02.993Z Reads: 284

```
Hi, I am really looking forward to try out this firmware and the app too. I have a nano x remote. I read something in the thread but I didn't find a clear answer. Is it possible to set a cruise control on it? The nano X has two additional bottoms one for the mirror throttle and one called channel two switch (for instance turn on the lights). ![ffaedb921edd8108ffb429bfb65fe90023cb64fe_1_690x491|690x491](upload://rigoCOMHbrOXST9UIjyXuSaU9cK.jpg)
```

---
## \#1531 Posted by: Ackmaniac Posted at: 2018-02-24T21:46:58.345Z Reads: 284

```
No it can't. The switch for the light doesn't give a PPM signal.
```

---
## \#1532 Posted by: rey8801 Posted at: 2018-02-24T22:07:14.444Z Reads: 287

```
That's a pity. And the one for the mirror throttle?
```

---
## \#1533 Posted by: Ackmaniac Posted at: 2018-02-24T22:12:11.870Z Reads: 299

```
That doesn't output a signal. It only makes a change internally to switch the signal. So it can't be used for cruise.
```

---
## \#1534 Posted by: rey8801 Posted at: 2018-02-24T22:31:45.259Z Reads: 298

```
Ok thank you very much. I will than use it without. So the right configuration sequence would be. Connect master VESC and receiver. Program it as multiple ESC over Can. Then set the motor, battery max and min and the configure the remote (nano x) as PPM signal. Once done with the master VESC repeat the same with the slave VESC except that the receiver  is not connected to the slave one and the VESC send data to master over CAN. Do I need to set motor, battery min max too, or it will be done automatically my the master? Thx
```

---
## \#1535 Posted by: Ackmaniac Posted at: 2018-02-25T08:57:16.763Z Reads: 292

```
You need to configure it for the slave as well.
```

---
## \#1536 Posted by: MartyMcFly88 Posted at: 2018-03-07T10:10:28.902Z Reads: 296

```
Hey, first of all, thank you @Ackmaniac for your amazing App and for your modified BLDC-tool, I have been using both for about 3 months now and I can't get enough :heart_eyes: I love the fact that you can switch modes in the app! (might be helpful when being stopped by the police ;) )
A slight problem has arisen for me since upgrading my phone to oreo though, since upgrading, I cannot seem to connect to the Bluetooth device anymore... I don't know if you are aware of this yet, but it seems to be that others are facing this as well:  [link](http://www.electric-skateboard.builders/t/bluetooth-hm-10-not-discoverable-on-android-8-0-8-1-oreo/36713) 
I have dug around a bit an apparently oreo has a general problem with ble connections, therefore I don't know if it is something you can fix or not .. Maybe this helps? [link](https://www.beaconzone.co.uk/blog/bluetooth-scanning-on-android-oreo/) 
when switching back to Android 7 everything I working fine, but looking forward maybe there is something that you can do :) :slight_smile:
```

---
## \#1537 Posted by: DeathCookies Posted at: 2018-03-07T19:50:31.267Z Reads: 296

```
1.Board Turned on
2. Reciever turned on
3. Board does Not move (0mph)
4. Connect over Bluetooth

Does that not work?
```

---
## \#1538 Posted by: MartyMcFly88 Posted at: 2018-03-08T14:54:09.368Z Reads: 293

```
Nope, as I said it worked perfectly for a couple of months.. I did exactly the same as before.. oreo does seem to have bluetooth issues..i just wandered if there was something on @Ackmaniac s end, which he could fix
```

---
## \#1539 Posted by: Ackmaniac Posted at: 2018-03-08T17:09:54.787Z Reads: 298

```
If the smartphone firmware has issues there is nothing i can do about it.
```

---
## \#1540 Posted by: Sender Posted at: 2018-03-08T18:07:49.126Z Reads: 294

```
Come on Bro, have him mail you the phone! 😂🤣😂 (I gots the jokea today)
```

---
## \#1541 Posted by: MartyMcFly88 Posted at: 2018-03-08T23:02:31.066Z Reads: 297

```
I think it is an issue with android oreo to be honest .. I found a lot of peoples online having trouble with BLE modules once switching to oreo.
```

---
## \#1542 Posted by: KhanCity Posted at: 2018-03-30T08:34:25.797Z Reads: 281

```
hi, which battery were you using LT2X with 96Wh or LT3X with 144Wh?
```

---
## \#1543 Posted by: philvanzu Posted at: 2018-03-30T09:37:24.118Z Reads: 280

```
LT3x / 7S6P
```

---
## \#1544 Posted by: KhanCity Posted at: 2018-03-31T08:17:37.126Z Reads: 283

```
How is your 2 Vesc setup?
2 controllers via can bus connector Master/Slave where each controller connected to separate side of the Leiftech battery? or you ran y cables to connect battery in parallel (y connector coming from controllers running to joined Y connection coming from both sides of the battery)
```

---
## \#1545 Posted by: philvanzu Posted at: 2018-03-31T08:35:41.552Z Reads: 282

```
Via can bus, this was months ago though and the problem never reappeared. I just had to enable cruise control, ride a few hours then disable it again IIRC. One thing that may be atypical is the can cable is pretty long , around 50 cm, because the 2 vescs are at opposite ends of the board.
```

---
## \#1546 Posted by: KhanCity Posted at: 2018-03-31T08:55:02.226Z Reads: 281

```
so, do you have LT3x battery connected each side separately to each controller, or you ran 2 combined female battery connectors to one and ran to a combined y cable from both controllers to run your power?
```

---
## \#1547 Posted by: sandrewvdv Posted at: 2018-04-02T18:25:55.734Z Reads: 278

```
@e.board_solutions this has all the info you need ;-) (and more :-P)
```

---
## \#1548 Posted by: e.board_solutions Posted at: 2018-04-02T19:28:13.026Z Reads: 280

```
Thanks ;)
10char
```

---
## \#1549 Posted by: KhanCity Posted at: 2018-04-04T06:59:38.269Z Reads: 288

```
I can't find a C rating of Leiftech battery to find out **batt max** You have 15A, how did you figure that out? you know the C rating?
```

---
## \#1550 Posted by: Tuomalar Posted at: 2018-04-04T17:01:44.754Z Reads: 289

```
@Ackmaniac Just just updated my vescs to newer firmware and noticed that in my slave vesc both red and blue led stays permanently on. Is that a problem or why does it do that? 

And do I need "soft ermp limit"? I'm using watt mode without reverse and did set PID max erpm to 60000
```

---
## \#1551 Posted by: Tuomalar Posted at: 2018-04-06T09:13:29.662Z Reads: 288

```
Can anyone help me with that, can’t find any specific info what those leds mean in this case ^
```

---
## \#1552 Posted by: celica39 Posted at: 2018-06-10T20:40:20.441Z Reads: 231

```
hi, everyone i try to save the file 3.102 to my computer and the .exe file is not recognized by winzip

ok i found how to download it sorry
```

---
## \#1553 Posted by: mmaner Posted at: 2018-07-15T16:58:11.928Z Reads: 196

```
Where's the "Limit ERPM with negative torque" option in @Ackmaniac  3.102?
```

---
## \#1554 Posted by: Sender Posted at: 2018-07-15T17:27:40.090Z Reads: 203

```
I couldn't find it. I wonder if it is something different in 3.1x.  I did notice going downhill that when I accelerated it would apply negative torque like braking if I was past the "max speed".  Curious.
```

---
## \#1555 Posted by: rey8801 Posted at: 2018-08-15T05:08:21.374Z Reads: 198

```
Hi! I see you are the only one that got asked the same question. Did you figured it out? I can't find the limit ERPM with negative torque in Ackmaniac vesc tool. Did it remove it? Thanks man and congratulation for the Leader Upgrade! :wink:
```

---
## \#1556 Posted by: Andy87 Posted at: 2018-08-15T08:48:44.744Z Reads: 200

```
I read somewhere why it’s not included anymore....unfortunately I can’t find it now 😬
It was something like the watt control mode lowers the torque the higher the speed is but don’t apply a negative torque when reaching max erpm.
```

---
## \#1557 Posted by: Andy87 Posted at: 2018-08-15T09:00:53.001Z Reads: 200

```
@mmaner and  @rey8801 I found it.
Here the official explanation from ack why it’s not included in the new version 
https://www.electric-skateboard.builders/t/extended-ackmaniac-esc-tool-based-on-vesc-tool/35116/124?u=andy87
```

---
## \#1558 Posted by: rey8801 Posted at: 2018-08-15T10:24:24.495Z Reads: 198

```
Thanks Bru! Better like that.
```

---
## \#1559 Posted by: deucesdown Posted at: 2018-08-16T02:06:54.564Z Reads: 199

```
Does anyone have the 2.53 zip for windows? Trying to get the settings from an old board before flashing 2.54. My google-fu wasn't strong enough...
```

---
## \#1560 Posted by: Pimousse Posted at: 2018-08-18T11:03:32.503Z Reads: 196

```
I should have it on my Google Drive :
https://drive.google.com/folderview?id=1Tkd1QHlOFbEAlC2QA7JUT4-JOcN3nOSM
```

---
## \#1561 Posted by: deucesdown Posted at: 2018-08-18T14:09:21.712Z Reads: 191

```
thank you thank you thank you, but looking for windows not ubuntu. trying virtualbox...
```

---
## \#1562 Posted by: Ackmaniac Posted at: 2018-08-18T16:38:10.086Z Reads: 195

```
Yes the app is from me as well. Do you use my firmware? And I am not familiar with that Bluetooth device. Is it a HM-10?
```

---
## \#1563 Posted by: deucesdown Posted at: 2018-08-18T19:48:21.355Z Reads: 198

```
Holy shit after a ton of dicking around with virtualbox and vagrant, I got your ubuntu zip to work, and have pulled the settings as xml. Thank you thank you! :slight_smile:
```

---
## \#1564 Posted by: Pimousse Posted at: 2018-08-18T20:23:12.406Z Reads: 199

```
Glad you got it working ! :slight_smile:
Sorry, I should hav checked the OS version.
```

---
## \#1565 Posted by: krloz Posted at: 2018-09-03T09:05:07.609Z Reads: 193

```
Hi everyone.  I'm not sure this has come up before but i have tried to be up to date in most of these posts.
Would somebody mind checking out this weird behaviour I get sometimes on watt reverse where only the master wheel turns backwards with a weird nose.  Other times it just works normally. 
https://youtu.be/wsxHNKiYDis
Thanks
```

---
## \#1566 Posted by: RobsonM Posted at: 2018-09-04T22:55:22.039Z Reads: 196

```
Hi! Big fan of your firmware @Ackmaniac! I was using it for past few months on 6S setup but just yesterday swapped it for 8S. I have changed all the according voltage ranges, redone the BLDC detection and went for a ride. The issues is when I want to accelerate hard I get a FAULT_CODE_DRV, but no additional details, and ESC cuts out. Please see attached screenshot of the log. Any suggestions? I run sensorless BLDC setup.

Thank for everything you do! ;)

![Screenshot_20180904-221139|281x500](upload://rKKcQoxFBcHhhsp1kCOCmw4UhO5.jpg)
```

---
## \#1567 Posted by: Ackmaniac Posted at: 2018-09-05T06:06:56.179Z Reads: 200

```
Looks like your DRV has issues. Check for loose phase in wires connections. But in most cases your DRV doesn't work 100% anymore and will break down soon.
You can also try to do the motor detection again.
```

---
## \#1568 Posted by: RobsonM Posted at: 2018-09-05T12:05:06.261Z Reads: 204

```
Thanks for the answer. Lowering max motor current from 50A down to 30A seems to help. Can it be that DRV is faulty in this case? Or is it maybe more related to some interference that's stronger with higher voltage? Like I said, over 300km with 6S and it happens exactly when I swap for 8S. If DRV is faulty shouldn't it also fail with 6S?
```

---
## \#1569 Posted by: Marksmoura Posted at: 2019-04-16T13:12:40.941Z Reads: 124

```
Hello, I can't get the direction switch to work properly. I saw some solution but they aren't working. 

 I set the erpm limit option on and using 3000 it but still the motors start going backwards without having to release the brakes. What can it be? I'm running without hall sensors. Can it be the reason?
```

---
## \#1570 Posted by: Marksmoura Posted at: 2019-04-16T13:40:47.697Z Reads: 124

```
I found the problem.
This function doesn't work in current mode only in Watt mode. 

I using the moded 2.54
```

---
## \#1571 Posted by: Ackmaniac Posted at: 2019-04-19T09:59:25.301Z Reads: 121

```
That's correct
```

---
## \#1572 Posted by: Bataleon Posted at: 2019-06-19T14:19:39.414Z Reads: 84

```
@Ackmaniac what firmware would you recommend I use for BLDC mode on HW4.12? I'm currently running stock FW2.18 which has been flawless but for the `cc_ramp_step_max * 10` bug when saving settings.

From what I understand Vedder stopped giving BLDC mode implementation much attention after FW2.18. Thanks
```

---
## \#1573 Posted by: mmaner Posted at: 2019-06-19T17:47:26.015Z Reads: 85

```
I would suggest you use Ack's 2.54 int he beginning, it's an easy setup.  If you want to later, upgrade to Ack's 3.103.
```

---
## \#1574 Posted by: Bataleon Posted at: 2019-06-19T21:53:58.334Z Reads: 79

```
Thanks @mmaner, I'll give it a try this weekend.
```

---
## \#1575 Posted by: banjaxxed Posted at: 2019-10-22T12:42:59.257Z Reads: 40

```
Don’t suppose anyone know where the Ack 3.103 firmware bin is? I can’t use the tool, plan is to program it with a st-link
```

---
## \#1576 Posted by: banjaxxed Posted at: 2019-10-22T13:04:47.033Z Reads: 39

```
Found it

https://github.com/Ackmaniac/bldc/blob/master/build_all/410_o_411_o_412/VESC_default.bin

version 3.103 which fixes a bug with for NRF remotes and adds support…

… for ADC remotes in combination with the Android App.
```

---
