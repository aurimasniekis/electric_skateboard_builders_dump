# VESC Monitor Android App

### Replies: 1166 Views: 48293

## \#1 Posted by: Ackmaniac Posted at: 2017-04-12T22:27:41.322Z Reads: 1970

```
I want to present you my android app. 

If you want to use all the features like mode changes and fault analysis then you need to flash the VESC with my firmware mod/extended which has the actual Version 2.54. If you use the standard firmware (2.18) then you will only see the realtime data.
You can get more information about the firmware mod/extention here.
https://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286

First of all you need a Bluetooth module. You can buy them very cheap here.
https://www.aliexpress.com/item/HM-10-BLE-Bluetooth-4-0-CC2540-CC2541-Serial-Wireless-Module/32516357718.html?isOrigTitle=true11

You need to connect the Bluetooth module this wayvia the 
**5V** Vesc to **VCC** Module
**GND** Vesc to **GND** Module
**RX** Vesc to **TX** Module
**TX** Vesc to **RX** Module
So you see that RX and TX needs to be crossed.

Then in the BLDC-Tool you have to activate UART and set the BAud Rate to 9600. if you have the Bluetooth module connected to the slave VESC in case of a dual setup which is connected via CAN then you need to activate there only UART. If it is connected to the master and you use a PPM controller then you need to activate PPM+UART.

the app itself can be downloaded in the Google Play store
[Vesc Monitor](https://play.google.com/store/apps/details?id=ackmaniac.vescmonitor)

When you start the app the first time you have to confirm that the app is allowed to use a couple of services like Bluetooth (for the connection)
GPS (to get the actual position for logging and speed)
Access to your storage (to store the log and video files) 
Camera (to shoot videos with realtime overlay)

After that you will see the actual available low Energy Bluetooth devices. So the board needs to be swicthed on to see it. Here in this picture you see my "Dual" Board. So once the app was connected to a Bluetooth module and received data it will ask you to give that Board a name so that it will be easy for you to detect the correct device again.
<img src="/uploads/db1493/original/3X/b/3/b3b0af1753cec746b78e5268ff11347ed5710801.png" width="281" height="500">

After you selected the correct Board (Module) you come to the realtime screen.
It trys to connect to the baord immediately. if that fails you can try it again by pressing connect on the upper right corner again. You can also disconnect via the same butten which will turn into Discon. (Disconnect) ones aou are connected.
<img src="/uploads/db1493/original/3X/d/f/df9723be46b92d38e52709b2cc550469c93fc12d.png" width="281" height="500">

The first time you see this screen it is a bit overloaded with information. But ones you understood what all the values mean you will love it. But more about that later.

First you should adjust the right settings for your board. So press the pencil Button on the top to go into the settings.
## **SETTINGS**
<img src="/uploads/db1493/original/3X/d/6/d6862b3fdfc300fd4b87d8175e2ae13fb0e880e5.png" width="281" height="500">
* **Board Name** Here you can change the Name of the Board.
* **No of Motors** Set the number of VESC in your power system. When this is set to 2 then the values like Watts,Motor Current and Battery Current are multiplied by that number. So you see how much Watts and Current are drawn from the entire system.
* **Mode Setup**
* **Battery Setup**
* **Drive Gear Setup**
* **Video Setup**
* **Save GPS Position** If you want the the GPS position get's stored in the Log files and that you see the GPS speed in the realtime Screen you need to enable this.
* **Connect by CAN to ID** If you want to connect to another VESC to see their realtime values or the Bluetooth module is connected to a slave VESC then you need to enable this parameter and select in the dropdown box the Controller Id if the VESC you want to connect to. In most cases the Master is 0 and the Slave is 1. You can see that in the BLDC-Tool App Configuration/General tab.

## **Battery Setup**
<img src="/uploads/db1493/original/3X/2/d/2dc149a97eccea2c0837c50f7d1cd8708a72928a.png" width="281" height="500">
* Here you adjust the WH of you Battery. this is important for the calculation of the range of the board. You can calculate this value by the number of cells in series multiplied by 3.6V for Li-ion cells or 3.7V for Li-Po cells. And the multiply the the AH of your Battery. So for example a 10S4P Battery with Samsung 25R cells have 10S * 3,6V * (2,5A a cell * 4P) = 360Wh. And i recommend to set the values a bit conservative here. So just reduce it by 10% or 15%. Because it also depends on the settings you have for the battery cutoff in the VESC. Because 2.5A a cell can only be reached if you discharge the cells till 2.5V. But mostly the cutoff end is at 2.8V a cell to don't stress the cells too much. So for a 10S4P Battery a value of 320 Wh is more realistic.
* No of cells in Series of the Battery
* As next you need to adjust at which single cell voltage at no load (now power drawn) the battery has which level of capacity in percent.

## **Drive Gear Setup**
<img src="/uploads/db1493/original/3X/7/5/7547c967af639f51220ef912f0aad80adbb92f5f.png" width="281" height="500">

* **Motor Magnets** the total amount of magnets in your motor. A normal SK3 or 6374 or 6355 motor has 14 magnets. A Hub motor mostly have 28 poles.
* **Wheel Size in mm** Size of the wheels diameter in mm. if you only know the size in inch then you need to multiply it by 2.54 to get the mm.
* **Wheel Pulley teeth** Teeth for the timing Belt or sprocket for chain drive in the Pulley. If you have a Hub motor then you should set this value to 1.
* **Motor pulley teeth** Teeth for the timing Belt or sprocket for chain drive in the Pulley. If you have a Hub motor then you should set this value to 1.
* **Motor pulley teeth** Kilometers or Miles

## **_So here are the individual Boxes in detail:_**

## **Mode Box:**

Here you see the actual active mode and the most important settings for that mode. 
<img src="/uploads/db1493/original/3X/b/2/b27bab58f0aade245602e1b245d147f20a56c7ac.JPG" width="407" height="215">
You can define new Modes in the menu and activate them by clicking on this mode box which opens a popup window that let's you select one of your modes. 
First you see which Remote Control mode is activated. Like Watt or Current control.

* **Max W** If a maximum Watt limit is set then you will see the watt limit here. If it isn't set then you will see if BLDC or FOC is activated. 
* **Max M** Motor Max like in BLDC-Tool.
* **Min M**  Motor Min like in BLDC-Tool.
* **Max km/h / Max mi/h** Maximum speed that is allowed for the mode.
* **Max B**  Battery Max like in BLDC-Tool.
* **Min B**  Battery Min like in BLDC-Tool.
These settings show the settings for each individual VESC
<img src="/uploads/db1493/original/3X/a/0/a09b0a00b484f6357c24b4b0173573c53941d18e.png" width="281" height="500">
Default is the mode that is adjusted by the BLDC-Tool. It is the mode the Board starts with when you turn it on. When you change a mode it doesn't get stored on the VESC. So ones you switch the board off and on again it is back to default.
if you want to store the values you need to press longer on the Mode Box. Then a popup window will appear which asks you if you want to store the actual selected mode as the new default mode, so that it will overwrite the actual default values.
<img src="/uploads/db1493/original/3X/4/a/4ab7e5d6bad345d6ea983124dcfd10678b5854a0.png" width="281" height="500">
Here you can also switch the motor mode BLDC to FOC or back. This only works when you made the motor detection before for both modes. So you have to make sure you set both modes up correctly. this way you can drive in silent mode or with motor sound if you like. Also BLDC is a little faster.

## **VOLT BOX**
The Main Value of this box shows the actual battery Volts. You will see that the Volts will decrease the more amps are drawn from the battery. this is called voltage sag which sounds worse than it is. That is how a Battery works. 
When the label turns yellow then the power is reduced because it reached the "Battery cutoff start" of the VESC. When it turns red then it reached the "Battery cutoff end".
<img src="/uploads/db1493/original/3X/5/c/5c04a503ecf75cea9e1cf7f737cbe9e87d591c48.JPG" width="400" height="143">
The % value in the Label shows you the actual Battery % which can be adjusted in the Battery settings. This value is only updated when no power is drawn from or charged to the battery.

* **Min** The lowest value that was seen during the ride.
* **Cell** The actual voltage of a single cell. Makes it easier when you have no 10S Battery to know at which voltage each cell is. this value is calculated by the actual battery voltage divided by the number of cells in series.

## **TEMPERATURE BOX**
The Main Value of this box shows you the actual Temperature of the VESC. When the label turns yellow then the power is reduced because it reached the "Temperature cutoff start" of the VESC. When it turns red then it reached the "Temperature cutoff end".
<img src="/uploads/db1493/original/3X/c/8/c8fdc3663d6fc03c2af063c13029edac9257ac75.JPG" width="404" height="140">

## **DISTANCE BOX**
The Main Value of this box shows the actual distance that has been done during the ride.
<img src="/uploads/db1493/original/3X/6/0/602c6f4fb53db097b05bf5bb5925a141d863be76.JPG" width="436" height="151">

## **RANGE BOX**
The Main Value of this box shows the theoretical Range that can be reached if the ride is continued with the average actual Wh consumption. This value is calculated by the Wh of your battery which you can define in the Battery settings.
<img src="/uploads/db1493/original/3X/e/8/e8fa9e9b2537ae910c70c6301387452ffee85b7d.JPG" width="434" height="152">

## **WH / AH BOX**
<img src="/uploads/db1493/original/3X/e/a/eaa34f4f7efd22dc1681f16382c61a801d553ab4.JPG" width="436" height="240">

* **Drawn** The complete drawn Wh during the ride and the complete drawn Ah during the ride.
* **Charged** The complete charged Wh during the ride and the complete charged Ah during the ride.
* **Ø per km** The average Wh per kilometer / mile during the entire ride and the average Ah per kilometer / mile during the ride.
* **per km** The Actual Wh and Ah per kilometer / mile if the ride would be continued like the board was ridden in the last half second. So you will see very high values when you accelerate from a standstill or uphill. And also minus values will be shown during braking.

## **Speed Box:**
The Main Value of this box shows the actual speed which is calculated by the Motor RPM.
<img src="/uploads/db1493/original/3X/f/5/f566ae2781345d4d77e98ca49f4f8288df1c3c3c.JPG" width="405" height="214">

* **Max W** If a maximum Watt limit is set then you will see the watt limit here. If it isn't set then you will see if BLDC or FOC is activated. 
* **GPS** Shows the actual speed meassured by the GPS. Only works when GPS is activated in the settings. This will always update with a little delay because the other speeds which are shown are taken from the Motor RPM which are very precise.
* **MAX**  the maximum speed which have been reached during the ride.
* **Ø T**  The average speed during your total ride. It will also xount it when you stand still. the counting starts ones the board strated to move the first time.
* **Ø R**  The average speed which is counted only when you are riding. So it won't be counted when you stand still.

## **POWER BOX**
The Main Value of this box shows the watts that are drawn or charged. If you set the number of VESC to 2 for a dual drive then the realtime data values will be multiplied by 2. So don't be surprised if you set a maximum of 1000 watts and you see 2000 here. The Label of this Box has Progress Bars which show you in each direction how far away you are form the maxium. When they reach the end then this is your limiting factor.
<img src="/uploads/db1493/original/3X/c/5/c5ed2ed6965c6e951aac8e125bf3609385b5fd6d.JPG" width="403" height="142">
* **Min** Minimum Watts (Braking) that are reached during the ride.
* **Max** Maximum Watts that are reached during the ride.

## **MOTOR CURRENT BOX**
The Main Value of this box shows the actual Motor Current (Amps). If you set the number of VESC to 2 for a dual drive then the realtime data values will be multiplied by 2. So don't be surprised if you set a maximum of 50 A and you see 100 A here. The Label of this Box has Progress Bars which show you in each direction how far away you are form the maximum. When they reach the end then this is your limiting factor.
<img src="/uploads/db1493/original/3X/c/2/c293107d3fb959968f840365c12114066dc17702.JPG" width="406" height="142">
* **Min** Minimum Current (Braking) that are reached during the ride.
* **Max** Maximum Current that are reached during the ride.

## **BATTERY CURRENT BOX**
The Main Value of this box shows the actual Battery Current (Amps). If you set the number of VESC to 2 for a dual drive then the realtime data values will be multiplied by 2. So don't be surprised if you set a maximum of 30 A and you see 60 A here. The Label of this Box has Progress Bars which show you in each direction how far away you are form the maximum. When they reach the end then this is your limiting factor.
<img src="/uploads/db1493/original/3X/a/c/ac9486d298b10972d26b764acc5652897060ea53.JPG" width="434" height="156">
* **Min** Minimum Current (Braking) that are reached during the ride.
* **Max** Maximum Current that are reached during the ride.

## **DUTY BOX**
The Main Value of this box shows the actual Duty Cycle (ratio of Motor Amps to Battery Amps). 95% is the maximum that can be reached in each direction.
<img src="/uploads/db1493/original/3X/5/c/5c65da30093a784005d63ec92794843aeb9978b6.JPG" width="436" height="153">

## **Ø Active / Riding**
<img src="/uploads/db1493/original/3X/6/b/6ba7d543389cf1662bd576d1996a1db6bd0a5238.JPG" width="440" height="246">

* **Mot** 
1: Average Motor Current only when drawn 
2: Average Motor Current only when charged
3: Average Motor Current drawn when driving. Calculated also when no power is drawn. Here you can see how much amps are really used for the motor on average during the entire ride.
4: Average Motor Current charged when driving. Calculated also when no power is charged. Here you can see how much amps are really charged back from the motor on average during the entire ride. 
* **Bat**
1: Average Battery Current only when drawn 
2: Average Battery Current only when charged
3: Average Battery Current drawn when driving. Calculated also when no power is drawn. Here you can see how much amps are really drawn from the battery during the entire ride.
4: Average Battery Current charged when driving. Calculated also when no power is charged. Here you can see how much amps are really charged back to the battery on average during the entire ride.   
* **Watt**
1: Average Watts which are calculated only by the time power is drawn or charged. So when you only roll it won't be counted.
2: Average Watts which are calculated over the entire riding time. So when you roll it will also be counted.

* **Time**
1: Shows the time that has passed since you started to roll the first time.
2: Shows the time that since you started to roll the first time. but it doesn't count the time when you stand still. So you see how long you were really on the moving.

## **MODES SETUP**
<img src="/uploads/db1493/original/3X/b/0/b0828048f62faec58fcfe8561eaa6082eb3b454a.png" width="281" height="500">
In this screen you can create and modify different modes for your board.To create a new Mode you need to press the "+" sign on the upper right of the screen. And to modify a already existing mode you simply need to press on it.

You can make basic setups for modes and also more advanced one. But first of all you should give the mode a name.
then you should select the Controller mode like Watt or Current control with or without reverse.
<img src="/uploads/db1493/original/3X/c/f/cf2f15fd3220026113bd1b2bf7e1d59e94919b3d.png" width="281" height="500">
Then you can adjust the Basic settings like in BLDC-Tool for Motor max, Battery max, Motor min and Battery min. You also have the possibility to set a watt limit for watt control modes.
if you want to limit the maximum speed you can do it here as well. (It will set the PPM or Nunchuk ERPM limit end to this speed and sets the ERPM limit start to 10 less than this value)

**Use different settings for front axle**
If you have motors at the back axle and at the front axle then you have the possibility to use different acceleration and brake power at the front and back axle. This only really works in watt control modes because in Current control it only shares the Current.
So you have to activate "Use different settings for front axle" and choose the Controller Id's of the front axle so that the app knows which VESCs will use the front setup.
<img src="/uploads/db1493/original/3X/8/a/8a962871f2b71da6697432dcc0d5a7dad4700bfe.png" width="281" height="500">
immediately you will see that different settings can be adjusted for the front. So if you want for example 66% of acceleration power at the back and 33% at the front 66% brake power at the front and 33% at the back then you could use the settings in the picture.

**Use special throttle curve**
When you activate this checkbox you will see actual throttle curve settings which are defined for that mode.
<img src="/uploads/db1493/original/3X/2/4/2490c0e86dea5137242254d36c4652c1a30f2395.png" width="281" height="500">
to change the throttle curve just click on the button with the numbers.
You see that a new screen appears that shows you the throttle curve in detail and let's you adjust it. it works exactly like the one in BLDC-Tool of my firmware mod. i recommend to start with the values like in the picture which work very well for me.
<img src="/uploads/db1493/original/3X/6/b/6b9d92e43272e978d6fe9815894e3f98abe8c2b2.png" width="281" height="500">

**Use Special Braking at Cruise Control**
When you click on this checkbox then a dropdown box appears which let's you select of it should be allowed for cruise control that it brakes when you are too fast or not. If you use special settings in PPM which overwrite the function for left or right then this will make no change.
<img src="/uploads/db1493/original/3X/0/8/08ab01b145e0a836bb28ee9b1994024fc16dad37.png" width="281" height="500">

**Use Special Cruise Control PID**
Here you can adjust the PID controller fro the cruise control. i recommend the settings like in the picture. If you want that it regulates the speed smoother you should lower the P and I. If you want it quicker you should raise the values. For carving at Cruise Control it is better to have it very smooth. If you change your motor max value then you normally also need to adjust the PID controller again because it regulates the power via the motor max. So if you lower the motor max you normally need to raise the values for the PID controller and if you raise the motor max you need to lower the PID values.
<img src="/uploads/db1493/original/3X/3/0/30f60c7726049f4eb79c9f5f5ab5e15b2ae528f6.png" width="281" height="500">


**And if somebody wants to honor all the work. (many hundred hours)**
:point_down::point_down::point_down::point_down::point_down::point_down::point_down::point_down::point_down::point_down::point_down::point_down::point_down::point_down::point_down::point_down:
:point_right: **[Donations](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=GJ59FXYPUQHUY)** :money_mouth: **[Donations](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=GJ59FXYPUQHUY)** :money_mouth: **[Donations](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=GJ59FXYPUQHUY)**:point_left:
:point_up_2::point_up_2::point_up_2::point_up_2::point_up_2::point_up_2::point_up_2::point_up_2::point_up_2::point_up_2::point_up_2::point_up_2::point_up_2::point_up_2::point_up_2::point_up_2:

This text is not complete yet and will be extended soon.
PLEASE don't use this thread to tell me that you want a IOS app. Any of such posts will be removed by me. Please concentrate only on the app,
```

---
## \#2 Posted by: Mobutusan Posted at: 2017-04-13T00:06:48.442Z Reads: 1124

```
Saweeet!! Your timing couldn't be more perfect. I just got my VESC-Xs this week, and installed your software on my computer last night. This will be my first foray into the wild world of VESCs, so I'm crossing my fingers that I don't screw anything up. Once I figure all this out, you're definitely getting a donation. I can't imagine how much time and knowledge it took for you to create this. :metal:

Also, is they're a good, current tutorial on how to initially set up VESCs and check settings, especially with this software? Or should I just scour and absorb info from your massive BLDC tool thread? I really don't want to screw anything up.
```

---
## \#4 Posted by: JLabs Posted at: 2017-04-13T01:36:47.054Z Reads: 1082

```
He dosnt have one yet, that is why he stated this:
[quote="Ackmaniac, post:1, topic:20888"]
PLEASE don't use this thread to tell me that you want a IOS app.
[/quote]
```

---
## \#5 Posted by: Ackmaniac Posted at: 2017-04-13T10:38:01.586Z Reads: 1016

```
Updates the text in the first post to explain the mode setup
```

---
## \#6 Posted by: t0m_r1dd1e Posted at: 2017-04-13T15:43:55.013Z Reads: 984

```
Awesome! I've been meaning to add BT to my board. Do you have a suggestion for a connector to plug into the VESC? I think it's a 7 pin connector right?
```

---
## \#7 Posted by: Ackmaniac Posted at: 2017-04-13T15:54:42.417Z Reads: 964

```
You can buy them at Aliexpress or on ebay. It is a JST 2.0 PH 7 Pin

https://www.aliexpress.com/item/20-SETS-Mini-Micro-JST-2-0-PH-7-Pin-Connector-plug-with-Wires-Cables-200MM/32805216474.html?spm=2114.01020208.3.262.UgDIPs&ws_ab_test=searchweb0_0,searchweb201602_5_10152_10065_10151_10068_10136_10137_10060_10138_10062_10156_10153_10141_10056_10055_128_10054_10059_10099_5070013_10103_10102_10101_10096_10148_10147_10052_10053_10142_10107_10050_10143_10051_10084_10083_10080_10082_10081_10110_10111_10112_10113_10114_10037_10032_10078_10079_10077_10073_10070_10123_10124,searchweb201603_6,afswitch_1,ppcSwitch_5_ppcChannel&btsid=b0a4dcc6-4591-40d9-a17c-0c09dda2d202&algo_expid=9f3202e5-a6b1-4e1c-b770-bcdb3a287399-11&algo_pvid=9f3202e5-a6b1-4e1c-b770-bcdb3a287399
```

---
## \#8 Posted by: Maxid Posted at: 2017-04-15T10:32:55.661Z Reads: 885

```
Just tried to connect to my board and the app crashes before it can make a connection. I can see my board in the BT detection but once I click on the connect button the app crashes without showing me any data from the board.
I am on a 7.1.1 custom rom (pure nexus) on a Nexus 5 (also still using your 2.54 beta firmware - do i need to upgrade to the release version first?)
```

---
## \#9 Posted by: Ackmaniac Posted at: 2017-04-15T10:36:01.521Z Reads: 852

```
Yes you have to update to the released 2.54. I optimized some stuff In the communication.
```

---
## \#10 Posted by: Guacamoleface Posted at: 2017-04-15T10:40:17.766Z Reads: 831

```
Mine crashed first time before it was allowed to activate Bluetooth, aftet that it worked.
```

---
## \#11 Posted by: yaca Posted at: 2017-04-17T19:19:56.376Z Reads: 822

```
I found a problem at least in connection with android 5.1.1. When I make a video with "Video Layout Left" it works but when a make a video with "Video layout Left and Right or Minimal" I get a strange video with mainly green and violet colours. What's wrong?
```

---
## \#12 Posted by: guyguy Posted at: 2017-04-19T16:58:33.165Z Reads: 796

```
switching between FOC/BLDC is pretty slick. nice job!
```

---
## \#13 Posted by: yaca Posted at: 2017-04-20T09:58:39.064Z Reads: 774

```
I can not see this function. Or is it just visible if FOC Mode is on in BLDC Tool?
```

---
## \#14 Posted by: Ackmaniac Posted at: 2017-04-20T10:14:54.399Z Reads: 765

```
Instead of clocking on the mode box to change a mode you have to press long on the mode box. Then you can store the actual settings as default or it also allows you to switch the motor control mode. But you have to make sure that FOC and BLDC is configured right. It is the same like if you would simply select the other mode in BLDC-Tool.
```

---
## \#15 Posted by: yaca Posted at: 2017-04-20T10:28:41.796Z Reads: 736

```
Ok thanks. Do you have an idea about the video problem which I posted 3 days ago?
```

---
## \#16 Posted by: Ackmaniac Posted at: 2017-04-20T10:34:16.043Z Reads: 719

```
No solution for that at the moment. Never had that problem.
```

---
## \#17 Posted by: yaca Posted at: 2017-04-20T17:09:22.472Z Reads: 710

```
It was always not recommended switching between FOC and BLDC without resetting the firmware. Isn't it suddenly no problem at all?
```

---
## \#18 Posted by: Ackmaniac Posted at: 2017-04-20T18:32:13.628Z Reads: 707

```
That's my favorite myth. It's like you have to get completely naked each time you change your socks.
```

---
## \#19 Posted by: yaca Posted at: 2017-04-20T20:56:42.626Z Reads: 714

```
I hope it is a myth but I'm not sure. Today I tried the first time FOC Mode. Everything was alright and I switched with the app to BLDC and back to FOC. But now I had a strange stuttering, I didn't try more, just reflashed the firmware and for the moment I think I stay with BLDC. No faults detected.
```

---
## \#20 Posted by: Ackmaniac Posted at: 2017-04-20T21:17:17.513Z Reads: 717

```
Reflashing makes makes no sense. But it also doesn't hurt. When your motor stutters at higher speeds then try to increase the switching frequency from 20000 to 30000. That solved the problem with my 6355 motors.
```

---
## \#21 Posted by: yaca Posted at: 2017-04-20T21:51:37.481Z Reads: 716

```
Stuttering was at lower speed and on the bench the wheels almost didn't want to start running when I gave throttle on the remote.
```

---
## \#22 Posted by: yaca Posted at: 2017-04-20T22:22:30.068Z Reads: 660

```
If I change from BLDC to FOC via VESC Monitor, it will change to FOC on both VESCs, right? HM-10 is connected to the Master VESC and Number of motors is set to "2". "Connect  by CAN to" is disenabled.
```

---
## \#23 Posted by: Ackmaniac Posted at: 2017-04-20T22:24:46.563Z Reads: 654

```
Yes it changes it on both when you send the command to the master. Important is that at the master "Send status over CAN"  is disabled.
```

---
## \#24 Posted by: Titoxd10001 Posted at: 2017-04-21T05:57:48.720Z Reads: 662

```
I'm having trouble changing settings with the app not sure if I'm doing it right. I go to mode setup and make a new mode, then I go to main screen and under default I select the new mode. The settings in the mode box change, but the it doesn't change on vesc?
```

---
## \#25 Posted by: will_manners Posted at: 2017-04-21T06:38:20.756Z Reads: 644

```
Dude this is next level! I cannot begin to imagine how many 100's (more like 1000's) of hours that went into the creation of your VESC app and BLDC-tool. I guess I'll have to go through the grueling process of installing a bootloader on my maytech vesc's :sob: Thanks so much for your work Ackmaniac! Just donated! ;)
```

---
## \#26 Posted by: Ackmaniac Posted at: 2017-04-21T13:11:04.723Z Reads: 629

```
I provided a new Version which should fix some resulution issues where the text was splitted into 2 lines. It's available at the Dropbox link and in a couple of hours also via the Google play store.
```

---
## \#27 Posted by: guyguy Posted at: 2017-04-21T13:35:45.209Z Reads: 595

```
Bench isn't a good way to test. FOC will stutter like crazy if you run it on bench.
```

---
## \#28 Posted by: The_Dude Posted at: 2017-04-21T13:40:51.783Z Reads: 596

```
Not with hall sensors😏
```

---
## \#29 Posted by: yaca Posted at: 2017-04-23T08:37:32.114Z Reads: 585

```
Still not on Google Play Store. 😢
```

---
## \#30 Posted by: sandrewvdv Posted at: 2017-04-27T19:18:29.515Z Reads: 612

```
OK wow, this app is amazing :astonished:. I orderded a bluethooth module a week ago and it arrived today.
So first thing I did was installing your upgraded firmware. 

Since I had to manually reset every parameter I thought, why not do a detection for FOC mode also. I have never done this in the past because I read somewhere it causes your VESC to break (in some cases). But man am I happy I did this :) my board runs sooo quiet now.  

Also to be able to see your amp draw, speed, range and all that other good stuff is amazing! Changing settings on the fly is really handy! Havent tried the video overlay, will be trying that (hopefully) this weekend. 

While using this app, I also found a bit of an issue with my VESC. After about 1 km of going 35 km/h, my VESC reached the temperature limit of 80 -90 °C and gave me less torque/speed. Is this a well know issue? 
( I saw a thread the other day where someone was having also an issue with this, but his temp sensor was broken. Mine isnt, because when I stop the temps begin to drop immediately)  

Now that I have the upgraded firmware, is there anything worth checking out in it? I know he added the 'Watt modus', but my board runs fine withouth any modification, I think :confused:

To end this I would really want to thank @Ackmaniac for making this incredible app. I will check your donation link out ;)
```

---
## \#31 Posted by: Ackmaniac Posted at: 2017-04-27T21:20:19.200Z Reads: 584

```
I would double check you settings to find the temperature issue there. Because my firmware mod doesn't really change anything which can cause a temperature rise. So maybe you VESC has a Issue with FOC or if you run BLDC again then please check that you did a motor detection in BLDC.
Another explanation could be that it is the first time that you see that you have a temperature issue. So i guess you have a single drive. Because dual normally don't get that issue.
```

---
## \#32 Posted by: sandrewvdv Posted at: 2017-04-28T03:38:57.755Z Reads: 556

```
No no it is definitely not your app. It is just something  I didnt know about before I had your app 😉
And you are correct, I'm using a single drive. Was just wondering if someone else had this problem too.
Edit: spelling
```

---
## \#33 Posted by: Rollbrett Posted at: 2017-04-28T08:01:30.129Z Reads: 530

```
Any plans on adding support for the pebble watch (you can pick one up for next to nothing nowadays)  or other smartwatches? That'd be a killer feature!
```

---
## \#34 Posted by: yaca Posted at: 2017-04-28T09:05:30.586Z Reads: 536

```
[quote="Ackmaniac, post:26, topic:20888, full:true"]
I provided a new Version which should fix some resulution issues where the text was splitted into 2 lines. It's available at the Dropbox link and in a couple of hours also via the Google play store.
[/quote]

On Google Play Store is still version 1.20 from 12th of April. Should not be a newer version available?
```

---
## \#35 Posted by: Ackmaniac Posted at: 2017-04-28T09:17:16.848Z Reads: 525

```
You are right, google changed the way to publish apps. So i missed a step. Should be available now or in a couple of hours. Correct new version is 1.21
```

---
## \#36 Posted by: capfirepants Posted at: 2017-04-28T15:20:42.464Z Reads: 531

```
So i've tried installing this app as well and sadly I can't connect to the BTLE Model at all. I'm using a HM-10 Module with firmware version 5.4. The connection works without problems with the VESC_CONNECT app from Jacob but I cant connect using yours. Running vesc FW 4.18. 
I was using v 1.2 this morning and I got "cannot connect, please try again" as an error message. Updated to 1.21 this afternoon and now I dont get the error message any more, the connect button changes to "Disconnect" but the graphs still don't show any data.
```

---
## \#37 Posted by: Ackmaniac Posted at: 2017-04-28T15:41:27.348Z Reads: 530

```
Did you connect it this way?
VESC 5v - VCC Module
VESC GND - GND Module
VESC RX - TX Module
VESC TX - RX Module

And you need to set a baudrate of 9600 for UART in BLDC-Tool.
```

---
## \#38 Posted by: capfirepants Posted at: 2017-04-28T15:42:16.878Z Reads: 532

```
Yes, the connection is correct - it works with Jacob Bloy's app "Vesc connect". Also the baudrate is set correctly.
```

---
## \#39 Posted by: Ackmaniac Posted at: 2017-04-28T15:48:30.283Z Reads: 555

```
Can you also read the data in the Vesc Connect app?
Seems that you have the wrong Bluetooth module. They mostly work with my firmware mod because i changed the timing there. You can find more information here.

https://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286
```

---
## \#40 Posted by: capfirepants Posted at: 2017-04-28T15:51:01.477Z Reads: 536

```
Yes, its possible to read and write data in the vesc connect app. The firmware of the bluetooth chip is the official HM-10 one which I flashed this morning. There a quite a few cheap copies of the HM-10 around which behave slightly differently so it may be that you are using a clone and havn't realized yet: http://blog.yavilevich.com/2017/03/mlt-bt05-ble-module-a-clone-of-a-clone/
```

---
## \#41 Posted by: Ackmaniac Posted at: 2017-04-28T15:57:30.884Z Reads: 534

```
Please show me which Bluetooth module you used exactly. 
And you can also give my VESC firmware mod a try if you want. Maybe it fixes the problem, maybe not. 
You can also try to restart your smartphone. Had a issue once.
```

---
## \#42 Posted by: capfirepants Posted at: 2017-04-28T16:00:24.509Z Reads: 490

```
I recieved a MLT-BT05 branded chip - they are discussed in the article I linked above. I then used this method: https://forum.arduino.cc/index.php?topic=393655.0 to flash the official HM-10 Firmware onto the chip. 
I have a different phone which I can use to test and will do that now.
```

---
## \#43 Posted by: Ackmaniac Posted at: 2017-04-28T16:02:56.637Z Reads: 474

```
So you have a clone and flashed it with the original firmware. Hard to tell what could be the issue then.
```

---
## \#44 Posted by: capfirepants Posted at: 2017-04-28T16:17:28.576Z Reads: 481

```
So the problem seems to be the phone. My huawei mate 9 doesn't seem to like connecting to the module. My old samsung galaxy s4 does it without a problem. 

Also, sorry if my last comments came across a bit dickish, that wasn't my intention.
```

---
## \#45 Posted by: Ackmaniac Posted at: 2017-04-29T02:19:25.875Z Reads: 488

```
I published a new version 1.25 which should be a bit more stable when it switches from the normal to the video view.

Edit: Changed the layout of the app a little bit so that it should be easier for the eye to concentrate on the important data.
Also added a auto focus for the camera and and automatic stabilization of the video if the smartphone supports this feature.
Also changed the handling of the different modes which let's you change the their order. And you can now copy already existing modes which should make it easier to create a new one.
```

---
## \#46 Posted by: Ackmaniac Posted at: 2017-05-01T00:33:10.518Z Reads: 480

```
Here is a little Video which is made with the new layout.

https://www.youtube.com/watch?v=vNNcW0CIh5Y
```

---
## \#47 Posted by: Marty Posted at: 2017-05-01T13:55:01.533Z Reads: 460

```
unfortunately my App crashes constantly when switching to the Video Capture page
```

---
## \#48 Posted by: Ackmaniac Posted at: 2017-05-01T20:39:18.371Z Reads: 456

```
I provided a new version which hopefully foxes a couple of crashes on some devices. If the app crashes then please send the bug report. 
@Marty would be great if you can also give it a try.
```

---
## \#49 Posted by: Marty Posted at: 2017-05-02T13:08:25.116Z Reads: 446

```
hi - yeah I sent a bug report feedback
```

---
## \#50 Posted by: Ackmaniac Posted at: 2017-05-02T13:30:22.486Z Reads: 451

```
Please update the app to the newest Version 1.26 and try it again. I think this error is fixed in the new one. You definitely used the old version.
If the problem still exists then please report the issue again.
```

---
## \#51 Posted by: Marty Posted at: 2017-05-02T14:20:59.947Z Reads: 441

```
updated to 1.26 - same UI crash when selcting video capture
```

---
## \#52 Posted by: t0m_r1dd1e Posted at: 2017-05-12T19:29:34.360Z Reads: 431

```
Finally got around to setting this up. The app is so cool! 

On the other hand, my board keeps disconnecting from my phone while riding. Got any suggestions for BT module placement? My deck is wood and fiberglass and my enclosure is plastic.
```

---
## \#53 Posted by: Ackmaniac Posted at: 2017-05-12T19:31:43.783Z Reads: 420

```
Best is to keep the module away from the battery and phase wire cables. With my board i still have a good connection when i am 10 meters away.
```

---
## \#54 Posted by: t0m_r1dd1e Posted at: 2017-05-12T19:34:36.497Z Reads: 408

```
Good to know. I'll try that. Thanks!
```

---
## \#55 Posted by: oxi Posted at: 2017-05-12T22:17:51.406Z Reads: 436

```
@Ackmaniac Hello :) In your extended firmware bdlc tools thread, i have ask you a question about the sharing of your android app source code. I think it can be very usefull for me to see how (with android) you communicate with the vesc by bluetooth.

I plan to create an application for raspberry connected to a gsm module. I fact i wan't to relay vesc information over internet.   
With that i wan't to trace my e-mtb in an google map style application.

So if you can share,(i don't need your full code, or if you wan't the source of your first version) just said me :slight_smile:

thanks you

oxi
```

---
## \#56 Posted by: Jebe Posted at: 2017-05-21T02:55:01.109Z Reads: 399

```
This is amazing work ! Thank you :)
```

---
## \#57 Posted by: Guacamoleface Posted at: 2017-05-26T23:45:07.838Z Reads: 406

```
Hey @Ackmaniac. Got your firmware along with the application. Its awesome and was very smooth to setup. 
The only issue I have as mentioned before in this thread was crashes while swapping either into (clicking camera icon) and out of it. It crashed quite some times while doing that. Also had some troubles sending / transfering files from phone to computer or phone to my google drive / youtube etc. 

Im on a LG G5 with Nougat 7.0!
 
Great job, the bldc version and app is awesome!
```

---
## \#58 Posted by: Ackmaniac Posted at: 2017-05-27T08:09:58.694Z Reads: 397

```
Just released a new Version of the app which fixes a little bug in the realtime data when you only brake. 
@Guacamoleface seems that Nougat 7.0 is causing issues. Need to buy a new smartphone soon to test that. But in the meanwhile please always send the error report when the app crashes. That really helps me to improve the app. And if you like the app donations are also very welcome and keep up the motivation :joy:
```

---
## \#59 Posted by: Guacamoleface Posted at: 2017-05-27T18:36:57.027Z Reads: 384

```
@Ackmaniac and everyone else in this thread - what is the best quality settings for video for you guys? I tried 1080p at 2k bitrate and it was pretty choppy for me. 
I changed it to maxed out, Phone resolution + highest bitrate but not yet tried it out except for indoors.
```

---
## \#60 Posted by: Ackmaniac Posted at: 2017-05-27T20:38:06.275Z Reads: 390

```
Just the highest settings and the quality should be fine. But even HD with the highest Bitrate works fine.
```

---
## \#61 Posted by: Daan_vZon Posted at: 2017-06-08T16:19:58.145Z Reads: 399

```
Hi @Ackmaniac, great work you did with the app! Read your explanation a few weeks ago and immediately ordered the Bluetooth module you advised to give it a try. I set it all up yesterday and can successfully connect with the module within the app. The problem, however, is that once it is connected it doesn't show the data coming from the VESC. Everything (speed, power, battery, temperature etc.) keeps standing at 0. Do you have any idea how I can fix this? The baud rate is set to 9600 and it is on PPM + UART mode, but I don't use your special firmware since you said it doesn't work on Windows and I'm afraid to do something wrong in setting it up. Could that be the issue? I have the exact same problem with the VESC_CONNECT_PRO app.
```

---
## \#62 Posted by: Ackmaniac Posted at: 2017-06-08T17:05:53.574Z Reads: 366

```
My firmware mod also works on windows so you can give it a try.
And did you connect the bluetooth module to the 5V line and connected RX at the VESC to TX at the module and TX at the VESC to RX at the module?
```

---
## \#63 Posted by: Daan_vZon Posted at: 2017-06-08T17:20:22.588Z Reads: 359

```
Yeahh, I connected it exactly that way. Then I will might give it a try, thought you said you needed Ubuntu for it or something.
```

---
## \#64 Posted by: Achmed20 Posted at: 2017-06-10T13:33:10.789Z Reads: 368

```
soooo,
my programmer finaly arrived which means i could finaly flash your firmware (was missing a bootloader) and use your app completly with modes

nice work, donations incoming ^^
```

---
## \#65 Posted by: Maxid Posted at: 2017-06-11T17:25:46.427Z Reads: 388

```
For anyone interested I recently had the problem that my AntiSpark switch was turned on the entire week during which I did not ride the board. The battery was luckily only drained to 31V from 41V.
This got me thinking however, on how to keep this from happening again.
I don't want to have to actively check every day if the board is still on or not and I also don't want a status LED because of stealthiness. So I had to come up with a different way.

Since we already have a BT module in our boards why not simply have [Tasker](http://tasker.dinglisch.net/) check if the BT device is in range and if it is give a warning? To keep it from constantly checking and giving random warnings I added the phone being charged as a second requirement before the warning is allowed to show.

Works like a charm. Whenever the board is still on when I plug the phone in for charging at night I'll get a warning message telling me to turn off the board.

You just have to set a profile with the conditions "charging" and "BT near" and associate a warning message to it.
The BT near can be set up with the following settings: Name and address of the BT device you can see in @Ackmaniac's app and then activate the checkboxes for "Low energy devices" and "unpaired devices".

So if anybody wants to reduce the risk of accidentally leaving the board on for an extended period of time I can only recommend giving this a shot as well.

Edit: You obviously need to have the board in BT range of your phone at night  - if you have a 300m^2 house and the board on the opposite side to your phone this will not work :)
```

---
## \#66 Posted by: TarzanHBK Posted at: 2017-06-12T08:04:45.528Z Reads: 346

```
That´s an awesome idea! I´ll check that later, because i´m not trusting my eswitch on my bms :D
```

---
## \#67 Posted by: Pimousse Posted at: 2017-06-12T15:06:29.557Z Reads: 340

```
I already kiiled 5 lipos by forgetting to switch off mine as well.
Thank you very much for the tip !
```

---
## \#68 Posted by: Ackmaniac Posted at: 2017-06-12T18:34:23.318Z Reads: 335

```
Just rolled out a new version which fixes the issue that you don't see the data anymore when the phones screen is switched off with the app running in the background and you turned of the board. 
Now it shows the last captured data even if the board is already turned off while the app is running in the background. 
Of course you need to start the app first and connect to the board.
```

---
## \#69 Posted by: DeathCookies Posted at: 2017-06-12T18:36:06.490Z Reads: 324

```
And you need to turn in the tx...
```

---
## \#70 Posted by: Titoxd10001 Posted at: 2017-06-12T23:50:19.924Z Reads: 328

```
A issue I had was at a event there was a lot people with Bluetooth devices so I was not able to see or select my board. Also is it risky that someone can hijack my board via Bluetooth?
```

---
## \#71 Posted by: Ackmaniac Posted at: 2017-06-12T23:54:18.594Z Reads: 330

```
Once you connected to the board with the app and gave the board a name then you will see the device with the name in red. And in theory it is possible to high jack the board. But once you are connected nobody else can connect to it anymore.
```

---
## \#72 Posted by: Titoxd10001 Posted at: 2017-06-13T00:11:10.880Z Reads: 329

```
I have connected to my board before and given it a name. I think there where to many devices around me and the red name from my board like there usually is didn't pop up.
```

---
## \#73 Posted by: TarzanHBK Posted at: 2017-06-13T06:18:24.250Z Reads: 320

```
so it would be nice to get an already connected and named board on top of the results.
```

---
## \#74 Posted by: Ackmaniac Posted at: 2017-06-13T06:59:54.055Z Reads: 328

```
That's a great idea. Will do so
```

---
## \#75 Posted by: ninja Posted at: 2017-06-13T12:52:19.638Z Reads: 312

```
Wich android version do I need to get your app working? At the moment I have old phone with 4.1.2. android version.
```

---
## \#76 Posted by: Ackmaniac Posted at: 2017-06-13T12:56:48.669Z Reads: 316

```
At least 5.0 if you want to use the feature to record videos and 4.4 i think if you only want to see the real-time data.
```

---
## \#77 Posted by: ninja Posted at: 2017-06-13T13:04:48.741Z Reads: 321

```
O.k thanx.
Than I will ask Santa Claus for a new phone :)
Or indeed inadvertently I could smash my phone, then nothing will stop from buying new one :wink:
```

---
## \#78 Posted by: Pimousse Posted at: 2017-06-13T13:26:25.651Z Reads: 319

```
Ohh nice !!
I often had this problem : turned the board off then looked at the phone for avg consumption : pwned. :smile: 

Thanks a lot.
```

---
## \#79 Posted by: TarzanHBK Posted at: 2017-06-13T13:29:35.910Z Reads: 331

```
Is it normal that the app is not saving the average speed, Wh and other things?
I tried it now only for a few km without video to check that everything is working and it did.
Tried it a few days later again and saw that all average specs are gone.
Is this normal? Would be nice to save these things to see the average data of all your runs.
```

---
## \#80 Posted by: Ackmaniac Posted at: 2017-06-13T14:15:56.977Z Reads: 331

```
You need to let the app run in the background. If you close it and start it after the run again it is like a new start for the app. So just leave the app by pressing the home button or the power button to switch off the display so that it is still opened in the background, this way it will capture the data while you are riding.
```

---
## \#81 Posted by: TarzanHBK Posted at: 2017-06-13T14:22:07.517Z Reads: 329

```
I rode like a kilometer with it open and like i said it worked great, but a few days later all the average data from the last run were gone. I would want to see the average data from all my runs while the app is active. So that i can tell how many wh for example i drew over the last month or so. Shouldn´t it work this way with the average data?
```

---
## \#82 Posted by: Maxid Posted at: 2017-06-13T14:24:02.322Z Reads: 305

```
I think right now average only means the average in a single run
A global average might be a good idea though - maybe one for every board
```

---
## \#83 Posted by: TarzanHBK Posted at: 2017-06-13T14:33:06.468Z Reads: 299

```
thats exactly what i´m looking for!
```

---
## \#84 Posted by: Ackmaniac Posted at: 2017-06-13T14:47:26.844Z Reads: 305

```
Now i understand. Thought about it already. But need to find the time to program something like that.
```

---
## \#85 Posted by: Surfer Posted at: 2017-06-13T15:10:02.880Z Reads: 325

```
Hi you can also flash a custom ROM up to android 7, have a look:
https://lineageos.org
If you want help on that just let me know
```

---
## \#86 Posted by: ninja Posted at: 2017-06-13T19:25:49.027Z Reads: 320

```
Can you explain me what it is and how to do it, in simple words, because with IT things I'm dumb ?

 I have old phone, but that bustard still works like charm. Anyway it is samsung SII, model number GT-I9100 with android version 4.1.2.

So you are saying that I can still use that app with my phone, just need to change something in my phone?
```

---
## \#87 Posted by: Surfer Posted at: 2017-06-13T22:26:11.570Z Reads: 344

```
in simple words is like reinstall windows in your laptop, but this time in your phone, this is a unofficial version of android, **custom** operative system by lineageos.
 is not difficult to flash a new rom, but you have to think what you are doing and follow properly the steps if you do it wrong you can have a nice brick instead a phone.
 And of course all data will be deleted, just like fresh start. back up!
here the link for the ROM
https://download.lineageos.org/i9100
here just a random video tutorial from the tube:
https://www.youtube.com/watch?v=1u6EB-zD42Y
custom Recovery:
https://forum.xda-developers.com/galaxy-s2/development-derivatives/recovery-twrp-3-0-0-0-t3330457
and the last Odin, the flashing software:
https://forum.xda-developers.com/galaxy-s2/general/odin-v3-04-t1703998
Good luck!! And if you need help, you know
```

---
## \#88 Posted by: SeanHacker Posted at: 2017-06-13T23:01:02.768Z Reads: 323

```
Or... :grin:

http://aokp.co

<img src="/uploads/db1493/original/3X/c/0/c0bd659fdfb86a1271053a05b8245024cfdde5d4.jpg" width="281" height="500">
```

---
## \#89 Posted by: Ackmaniac Posted at: 2017-06-13T23:19:50.518Z Reads: 308

```
But if your old Android phone doesn't have the Hardware for Bluetooth low energy it won't help at all.
```

---
## \#90 Posted by: ninja Posted at: 2017-06-14T00:03:20.080Z Reads: 307

```
Thanx guys @Surfer and @SeanHacker, I'll do it if my phone have the Hardware for Bluetooth low energy.

@Ackmaniac I'll check if my phone have that low energy hardware, but i'm not sure where I should lookin, but will see :wink:
```

---
## \#91 Posted by: Ken Posted at: 2017-06-15T17:43:07.646Z Reads: 302

```
Looking to install this in the next day or two. If I connect the HM-10 to the slave VESC-X, can I save new modes this way, or do I need to connect it to the master VESC-X?
Ken
```

---
## \#92 Posted by: Ackmaniac Posted at: 2017-06-15T19:26:06.725Z Reads: 297

```
You can connect it to the vesc but then you have to activate "Connect by can to ID" and enter the controller ID of the master.
```

---
## \#93 Posted by: Ken Posted at: 2017-06-15T20:25:56.848Z Reads: 310

```
EDIT: found the app and downloaded to my new Samsung Galaxy Express 3 phone. Only $50 at Best Buy, and the had android phones starting at $20 that were version 5.1. I spent the extra so I can add up to 128gb memory card for videos

Thanks!
I can't find the APP on google play. I'm signed in, added a payment method, and I'm ready to go. I even downloaded the App permission that you wrote, as well as the vedder monitor app (by mistake). Clicking on your above link won't find it either...it keeps asking me to retry.
```

---
## \#94 Posted by: JLabs Posted at: 2017-06-15T22:35:34.387Z Reads: 302

```
Just search VESC on Google Play and a bunch of apps come up, incliding the one you want.
```

---
## \#95 Posted by: Ackmaniac Posted at: 2017-06-16T01:36:37.017Z Reads: 339

```
Just released a new Version of the app.
i added a Tripmeter/Tachometer which records the driven km, used Wh and Ah and some additional information of all your rides. There are 3 Trips and a total available which can be selected by the button on the top right. To reset a trip you need to press long on the screen. then you will be asked if you really want to reset the trip.
By this you can record the total driven kilometers of your board, km since the last charge or km during the entire day. Just reset the trip whenever you want to start recording from scratch again. If the Total Trip get's deleted then all other trips will be deleted as well. So this only should  be done if use the module in a new board.

<img src="/uploads/db1493/original/3X/1/7/17335cfe474cebb43ab969183015aca644af5e6e.png" width="281" height="500">

You can select the "Board Info" Screen via the settings Menu.
<img src="/uploads/db1493/original/3X/d/f/dfdefdf26591028adc755d1ce99ec22de63073da.png" width="281" height="500">
```

---
## \#96 Posted by: JLabs Posted at: 2017-06-16T03:00:36.738Z Reads: 303

```
Looks good Nico!
```

---
## \#97 Posted by: TarzanHBK Posted at: 2017-06-16T07:32:26.824Z Reads: 299

```
That´s awesome! Thanks for that. I get my new board running, test this next week and of course drop some moneys at your paypal :slight_smile:
```

---
## \#98 Posted by: Pimousse Posted at: 2017-06-16T07:48:41.301Z Reads: 298

```
Great !!
We talked about that months ago and thought it wasn't planned.
So nice you coded it, thank you very much ! :slight_smile:
```

---
## \#99 Posted by: ninja Posted at: 2017-06-17T09:09:17.301Z Reads: 298

```
Hi! 
Here is specifictions of my phone, des it have that bluetooth low energy harware? http://www.gsmarena.com/samsung_i9100_galaxy_s_ii-3621.php
```

---
## \#100 Posted by: Ackmaniac Posted at: 2017-06-17T12:38:01.483Z Reads: 294

```
It has Bluetooth 3.0. So it doesn't have Low Energy features, sorry.
```

---
## \#101 Posted by: Ken Posted at: 2017-06-17T21:06:24.589Z Reads: 314

```
How did you determine the values for battery setup? I have a Samsung 25R 16850 (2599Ah) 10S6P battery pack. Best I can determine is it's Wh is 540. Nominal charge is 3.6V and full charge is 4.2. 
Do I start with Battery 100% at 4.2 or 3.6V? What should 0% battery be?

<img src="/uploads/db1493/original/3X/c/a/cadede26fe7c50571c5d7782387cdb2ec8bd48b2.png" width="277" height="500">
```

---
## \#102 Posted by: Ackmaniac Posted at: 2017-06-17T21:47:47.346Z Reads: 285

```
Just leave it as it is. That's a good starting point. It measures the actual battery % only when you don't draw any power from the Batterys. So if the battery is at 3.46V in idle then it is at 0%. Sadly every battery differs. So it is a starting point and you can adjust it by your experience or personal preference.
```

---
## \#103 Posted by: Ackmaniac Posted at: 2017-06-17T21:50:59.005Z Reads: 291

```
Just released a new version of the app which changes the parameter names in the Trip Screen to hopefully more intuitive and understandable names for the values.
And in Devices Screen the already known Bluetooth modules will be shown first. This way it should be easy to find the Boards Module in a bluetooth crowded environment.
```

---
## \#104 Posted by: Ken Posted at: 2017-06-17T22:15:49.695Z Reads: 290

```
The above graph is from your sample in the first post. Currently, it's with 2 percentage point of my LCD Volt  display that Bara included with his battery. I'll monitor how close they are as drain the battery to 0%.

I did have a few issues connecting this afternoon...my phone screen turned black a few times. Not sure if it's a phone issue or an app issue, but I thought I'd mention it. I just updated the app, so I'll check that later. Thanks again!
```

---
## \#105 Posted by: Ackmaniac Posted at: 2017-06-18T20:35:30.740Z Reads: 314

```
Just released a new Version of the app.
Notifications are now added when a module is currently connected. You will see a icon in the statusbar that reminds you that the the board is still switched on and records data.
When you pull down the status bar the actual Battery %, Volt and Range of the Board will be shown as quick info. And when you click on the notification the app will with all the data will be opened again.
This way the app can run in the background while you do other things with the Smartphone and you can always have a quick look about the status of your battery.

BTW: "Titanium" is my boards name.
<img src="/uploads/db1493/original/3X/d/7/d775bb504282c2b7161981f6ab4670e757e2a7cd.png" width="281" height="500">
```

---
## \#106 Posted by: austin54 Posted at: 2017-06-19T09:26:00.246Z Reads: 294

```
Amazing App! I just tried it. I was able to connect to my VESC und the default values, which I set with the BLCD Tool are shown in the App + the real time data. The only thing which is not working is switching between different drive modes. Every time I select a mode, I end up with the default mode. What could be wrong here?
```

---
## \#107 Posted by: Pimousse Posted at: 2017-06-19T10:06:02.209Z Reads: 298

```
@Ackmaniac, since the 1.34 update, I experience crashes when after doing other stuff with other apps (e.g. sending a text or web browsing), I come back to your app.
Then, I get the "The application doesn't respond" error pop-up.
It doesn't happen each time, but mostly if I do lot's of stuff, lock, unlock screen and so on.

I reported it. Hope it can help.
Running Android 6.0.1 on Nexus 5X.
```

---
## \#108 Posted by: Ackmaniac Posted at: 2017-06-19T10:09:20.691Z Reads: 281

```
To change the mode you need my modded firmware.
```

---
## \#109 Posted by: austin54 Posted at: 2017-06-19T15:04:45.050Z Reads: 292

```
I'm using your firmeware 2.54. see attached picture. I tried with 2 different boards. Both VESC have HW Version 4.1.
<img src="/uploads/db1493/original/3X/5/2/52819ffd1669286ad62fe4a2cef5e8fe96156671.png" width="455" height="396">
```

---
## \#110 Posted by: Ackmaniac Posted at: 2017-06-19T17:29:22.059Z Reads: 272

```
Which modules are you using?
```

---
## \#111 Posted by: Guacamoleface Posted at: 2017-06-19T18:13:36.444Z Reads: 276

```
Noticed a thing with the new version, was just out running my board and decided to record. Unfortunently my fat finger came across the lock phone button. Now with it still monitor while phone is asleep/locked when app is running is doing the same with recording video. it will record the lock screen. 
Not really a problem but worth knowing :slight_smile:
```

---
## \#112 Posted by: austin54 Posted at: 2017-06-19T20:15:28.707Z Reads: 274

```
I'm using: HM-10 BLE Bluetooth 4,0 CC2540 CC2541 from Alibaba. I think that are the ones you recomend.
```

---
## \#113 Posted by: Ackmaniac Posted at: 2017-06-19T21:05:03.383Z Reads: 273

```
That's very strange. Maybe try to restart your phone and if that doesn't work then reinstall the app. Which kind of phone are you using and is it a modded OS?
```

---
## \#114 Posted by: Ken Posted at: 2017-06-19T21:46:58.737Z Reads: 268

```
Using the "Send" feature, I was trying to send a video to youtube and google drive, but to no avail. Does the Send feature work, or am I doing something wrong?
```

---
## \#115 Posted by: Guacamoleface Posted at: 2017-06-19T21:58:38.833Z Reads: 268

```
@Ken 
Does not work for me either, and on plugin I just see empty folders. I can send Video to my photo section of my drive. But nothing else.
```

---
## \#116 Posted by: guyguy Posted at: 2017-06-20T15:42:31.286Z Reads: 266

```
The updates are awesome thanks ackmaniac
```

---
## \#117 Posted by: thisguyhere Posted at: 2017-06-20T16:20:38.924Z Reads: 280

```
if i'm running dual by splitting the remote servo wire, instead of master+slave via CAN, would i need two bluetooth modules to connect to both VESCs, or just one and set setting to 2 VESC in software?

i'm thinking the latter, just want to make sure.
```

---
## \#118 Posted by: Jinra Posted at: 2017-06-20T16:23:12.787Z Reads: 287

```
I'm not 100% sure but I think you can connect the CAN for communications for the module, but not for PPM control. I'm guessing you'd still have to select "send status via CAN" from the slave VESC, but not use "multiple ESCs over can" on the master.
```

---
## \#119 Posted by: mmaner Posted at: 2017-06-20T16:25:41.877Z Reads: 294

```
@Jinra is pretty much correct.  With CAN Bus you will only need 1 Bluetooth module, with a split servo you would need 2 bluetooth modules.  CAN bus does support PPM to both modules, in a weird way, not sure I really understand it but it works.
```

---
## \#120 Posted by: austin54 Posted at: 2017-06-20T17:10:13.534Z Reads: 291

```
I'm using a Doogee Y300 with Android 6.0. I deinstalled the App and reinstalled, but same behavior.
```

---
## \#121 Posted by: Ackmaniac Posted at: 2017-06-20T20:17:25.614Z Reads: 297

```
Actually i never did that but sounds like it should work with a splitter cable.
```

---
## \#122 Posted by: austin54 Posted at: 2017-06-21T19:36:13.546Z Reads: 282

```
To be sure I flashed the 2.54 firmware into the VESC again. But problem still exists. Is there a chance to get the log of the communication between the app and the VESC to find out which error code was given back?
```

---
## \#123 Posted by: Ackmaniac Posted at: 2017-06-21T20:02:05.407Z Reads: 275

```
Could be that your smartphones bluetooth doesn't work properly. Maybe you can try with a friends phone if the connection works. Problem is that i need to split the message in multiple packs. And i think your smartphone has a problem with that.
```

---
## \#124 Posted by: austin54 Posted at: 2017-06-21T20:39:03.623Z Reads: 275

```
Yes, that was also my next idea. The Doogee Phone is a cheap china Android phone. So may be the BT implementation  is not properly done. Which is a pity behause I only baught the phone for the VESC monitor app. ☹️ So I'll check with a different Android phone.
```

---
## \#125 Posted by: Ackmaniac Posted at: 2017-06-22T17:26:38.977Z Reads: 276

```
Just released a new version 1_36 which hopefully fixes a bigger communication issue which caused a crash of the app in some situations.
The new version should now also support to read the realtime values of the VESC 6. It isn't possible to change the mode for VESC 6 yet. Sadly i don't have one myself so it would be great if somebody is brave and gives it a try. (don't forget to update the app first)
I also changed the look and feel a bit and hopefully the red and green bars are shown now correct for power, motor, battery and duty.
```

---
## \#126 Posted by: Ackmaniac Posted at: 2017-06-25T20:56:00.974Z Reads: 263

```
Just released new Version 1_38 which hopefully makes the communication a bit more robust. Especially the switch from the normal app to the video capturing should be more stable.
```

---
## \#127 Posted by: Pimousse Posted at: 2017-06-26T12:42:10.433Z Reads: 263

```
How does the app knows it's connected either to a VESC 4 or a VESC 6 ? By choosing it in configuration panel ?
As I told you by PM, old commands bricks the new bootloader (e.g VESC 6) so no place to mistake ! :neutral_face:

BTW, glad to help you making your app compatible with VESC 6 ! :wink:
```

---
## \#128 Posted by: Ackmaniac Posted at: 2017-06-26T12:45:29.587Z Reads: 254

```
I identify it by the firmware version. If the VESC 6 firmware is identified it uses the COMM_PACKET of the VESC 6. But not sure if it works without issues.
```

---
## \#129 Posted by: Pimousse Posted at: 2017-06-26T12:53:47.676Z Reads: 265

```
In theory, that should work.
Maybe using VESC6 commands with VESC4 is less "dangerous" than the opposite. TBC.
Thus, the default COMM_PACKET to use should be the new one. Do you agree with it ?
```

---
## \#130 Posted by: Ackmaniac Posted at: 2017-06-26T12:57:30.692Z Reads: 268

```
i am not sending any commands. So it is not possible to change the settings. Guess when i ask for the actual motor and app configuration that it get's translated in some bullshit. But it might work. Also the realtime data might be wrong. Sadly i can't test it myself so if somebody want's to give it a try feel free.
```

---
## \#131 Posted by: Pimousse Posted at: 2017-06-26T13:10:58.722Z Reads: 263

```
How do you send the configuration of a custom mode from the app to the VESC ?
Don't you use COMM_SET_MCCONF ?
```

---
## \#132 Posted by: Ackmaniac Posted at: 2017-06-26T13:55:33.189Z Reads: 256

```
No, i added a special command. Which of course doesn't exist in the VESC 6 code.
```

---
## \#133 Posted by: suwuj12 Posted at: 2017-06-27T07:45:34.862Z Reads: 261

```
https://www.instagram.com/p/BVwO16XgjWl/?taken-by=suwuj12
thanks @Ackmaniac I appreciate your dedication and hard work to make this possible
```

---
## \#134 Posted by: suwuj12 Posted at: 2017-06-27T07:47:48.163Z Reads: 256

```
https://www.instagram.com/p/BVqwNNNgiAn/?taken-by=suwuj12
```

---
## \#135 Posted by: Ackmaniac Posted at: 2017-06-27T23:09:09.857Z Reads: 251

```
Thanks for the video. Sadly i saw in the video that there is a little bug. Because every time you give some throttle the green power bar is always fully drawn. But it should show how much of the maximum power is drawn.

Just released a new version which should fix that glitch.
```

---
## \#136 Posted by: austin54 Posted at: 2017-06-29T12:52:37.174Z Reads: 250

```
I checked with a friends phone and it worked. So I flashed a new ROM into my phone and now I works. Thanks for your help.
```

---
## \#137 Posted by: solidgeek Posted at: 2017-06-29T13:42:40.961Z Reads: 256

```
Very nice app @Ackmaniac do you know if anyone has tried your app with a VESC 6? I am currently finishing my build using a VESC 6, and I would love to use your app. However I would hate to brick my VESC 6 at the moment :sweat_smile:
```

---
## \#138 Posted by: Ken Posted at: 2017-07-02T06:10:32.192Z Reads: 272

```
A video from a week ago using the app. Wisconsin has miles of sweet bike trails that follow Lake Michigan. This is in Milwaukee at South Shore Park

https://www.youtube.com/watch?v=ekMIp_5BqNg&feature=youtu.be
```

---
## \#139 Posted by: Pimousse Posted at: 2017-07-02T16:30:21.847Z Reads: 275

```
@Ackmaniac, I tested your app with the VESC 6 : it doesn't work.
As I'm working on an Arduino project for communicating with the VESC, I could catch a bunch of data and figured out that the serialization has changed...

But good news !
After few hours of reverse-engineering, I got the new one. :slight_smile:
```

---
## \#140 Posted by: Ackmaniac Posted at: 2017-07-04T09:50:16.246Z Reads: 265

```
Just released a new version which should be able to show the realtime data for VESC 6.
```

---
## \#141 Posted by: Pimousse Posted at: 2017-07-04T11:44:55.824Z Reads: 272

```
Great. I'll test it asap.
Are the non-compatible features disabled in this version ?
I mean, if VESC6 firmware is detected, only the COMM_GET_VALUES command is sent, right ?
```

---
## \#142 Posted by: Ackmaniac Posted at: 2017-07-04T13:11:40.611Z Reads: 252

```
No it doesn't. But i released a new version 5 kin ago again which should fix a little bug with VESC 6. So please use the newest version. Sadly the progress bars will not work correctly and the app might crash with VESC 6 but hopefully the realtime data is visible.
```

---
## \#143 Posted by: Pimousse Posted at: 2017-07-05T19:04:34.969Z Reads: 264

```
Ok, it works. :slight_smile:

<img src="/uploads/db1493/original/3X/1/a/1ae55b528bcaeea5a8db9ab81847802fa6273063.png" width="281" height="500">

But the power value stays at 0W.
Also, could you add the motor temperature ?
As now with VESC 6, the main limiting factor will be the motor temperature (due to huge performances of the new VESC), it will be necessary to keep an eye on it. ;)
```

---
## \#144 Posted by: Ackmaniac Posted at: 2017-07-05T21:09:54.923Z Reads: 236

```
@Pimousse thx for all the usefull info and for testing. 
I released a new version which shows should fix the power value issue.
```

---
## \#145 Posted by: Pimousse Posted at: 2017-07-06T05:16:43.574Z Reads: 258

```
You're welcome ! 
I'm a daily user of your app since the first version, it's normal to send you the lift back.
BTW, I'll continue to test your app. It crashed a lot (reported).
I also got error 22 multiple times (had to kill the app to have it running back).

<img src="/uploads/db1493/original/3X/0/1/019ffddca915590904271d9162504275b3211a1c.png" width="281" height="500">
```

---
## \#146 Posted by: Ackmaniac Posted at: 2017-07-08T23:49:05.449Z Reads: 248

```
Just released a new Version 1_43 of the app.
Now you can see the already known boards which let's you adjust the settings and see the Trip info (total km, wh, ah etc.) even when the board is not connected via Bluetooth. In this case the boards name is shown in gray. When the boards Bluetooth is available it will turn red.
```

---
## \#147 Posted by: Pimousse Posted at: 2017-07-21T14:05:06.407Z Reads: 249

```
@Ackmaniac : I had my first ride with my dual VESC 6.
It worked well, but values seems to be very low when I look at the chart with VDLA (7 Wh/km with dual 3550W on a eMTB, only 46A max drawn).
I set 2 in VESC numbers.

Is it possible that the app didn't double values regarding my dual configuration ?
```

---
## \#148 Posted by: Ackmaniac Posted at: 2017-07-21T15:44:43.478Z Reads: 240

```
Thank you for the info. Your were absolutely right. Just released a new version which fixes this issue. That was a very stupid mistake. Sadly i can't test it myself.
```

---
## \#149 Posted by: thisguyhere Posted at: 2017-07-21T15:54:36.895Z Reads: 244

```
i'm putting the finishing touches on a new build and including vesc monitoring, just waiting for the jst 7pin connector to arrive.  in some ways i'm looking forward to the vesc monitoring the most out of this new build.

i think this question kind of answers itself but wanted to make sure.

i'm controlling dual vesc by [splitting the remote receiver's 3pin servo cable](http://www.electric-skateboard.builders/t/y-piece-or-canbus/26461/2?u=thisguyhere).

since i'm not using the CAN, do i just enable "send status over CAN" tickbox so the 'slave' vesc reports back to the master, where the bluetooth module is connected?

if i HAVE to control dual drive with CAN, i will probably monitor one vesc and just double the values in my head.
```

---
## \#150 Posted by: rich Posted at: 2017-07-22T16:58:23.900Z Reads: 231

```
Hey @Ackmaniac, the app worked well but since i've updated my HW 4.12 to FW 3.26 there is no more realtime data visible. I've updated the app today so it's the newest version.
Any Idea? Thanks
```

---
## \#151 Posted by: Surfer Posted at: 2017-07-22T17:19:25.450Z Reads: 232

```
Hi Rich, did you see some improvement in 4.12 with the new firmware?
```

---
## \#152 Posted by: rich Posted at: 2017-07-22T17:59:48.853Z Reads: 240

```
Yes there are new features like motor temperature max. settings (if you have motors with temp sensors like trampa) and motor temp realtime data. Also the FW update without bootloader on PCB 4.12 is no problem. There are nice motor and app wizards in Vesc-Tool and adjustable throttle curve, max. watt,....
Also FOC should run better (but i don't use it). Everything looks good.
Tomorrow i'll test it outside the first time :grinning:
```

---
## \#153 Posted by: guyguy Posted at: 2017-07-24T18:44:34.208Z Reads: 234

```
The app seems to crash if the board gets disconnected or turned off when the app is running in the background. It's also really hard to kill the app when it's frozen.
```

---
## \#154 Posted by: L3chef Posted at: 2017-07-28T19:26:05.865Z Reads: 233

```
I have an wemos 8266 d1 mini laying around. Have someone made it to work with it?
@Ackmaniac thank you so much for the app. With mode control I can set the board to go 15kmh and therfor leagally ride it from the pub :smile:  
Will buy you a couple of beers when it's up and running!
```

---
## \#155 Posted by: Ackmaniac Posted at: 2017-07-28T19:33:52.843Z Reads: 230

```
Made it already working with the ESP via WiFi UART. Nice but tue WiFi uses too much ma. And you can Limit the speed in any mode. Just simply Set the Max speed for the mode. A couple of beers are very welcome.
```

---
## \#156 Posted by: L3chef Posted at: 2017-07-29T16:16:22.160Z Reads: 231

```
Just noticed it´s saturday. good time for a beer then :)
```

---
## \#157 Posted by: capfirepants Posted at: 2017-07-30T12:58:36.750Z Reads: 229

```
Just wanted to ask if anybody has been using the app with a phone running android 7 (nougat)? I can connect to the module but no data is displayed. The module works with my old phone running android 5.1.
```

---
## \#158 Posted by: Guacamoleface Posted at: 2017-07-30T13:11:33.617Z Reads: 227

```
@capfirepants 
Im using it with ny android (LG G5) along with nougat, Used to have problems with crashes but now it works flawless as far as I noticed.
```

---
## \#159 Posted by: Maxid Posted at: 2017-07-30T16:01:56.507Z Reads: 235

```
I am running a Nexus 5 with 7.1.1 and it works just fine.
The only (minor) thing I experience occasionally is that the app won't connect straight away when choosing my board, so I have to press connect again in the top right corner.
other than that I am super happy with the app - just tested the mode changing feature yesterday and it is awesome to not need a PC everytime you want to try a new setting.
```

---
## \#160 Posted by: krloz Posted at: 2017-07-31T06:54:52.971Z Reads: 235

```
Hy. Firstly.  Thanks a lot @Ackmaniac for these beast of custom firmware and app. I'm more than anxious to try it out as soon as i catch a brake from work. 
I have a very  tiny concern in my head however. I am sure I am not going to have my phone always connected when I have my board running and I don't like the idea of someone connecting to my board when I'm riding and screwing something up. Would it be possible to add a switch to the bluetooth module?  Maybe simply to the 5v line?  Would that be safe for the module and the vesc?  And would it be safe to hot switch on and off the module?
```

---
## \#161 Posted by: Ackmaniac Posted at: 2017-07-31T07:00:02.142Z Reads: 229

```
Sure you can add a switch to the 5V line. For UART that shouldn't be a problem.
```

---
## \#162 Posted by: krloz Posted at: 2017-07-31T07:06:10.803Z Reads: 223

```
Thanks. Am I the first to try this?  I'll comment then when I get to do this.
Thanks dude:wink:
```

---
## \#163 Posted by: Ackmaniac Posted at: 2017-08-06T13:36:51.479Z Reads: 226

```
Just released a new version of the app which hopefully fixes some bugs which can cause app crashes. Should run a bit more stable now. It's version 1.45
```

---
## \#164 Posted by: deucesdown Posted at: 2017-08-10T21:56:56.675Z Reads: 231

```
Awesome. Just wow.

It's like unbelievable as is, but I have some feature requests:

* for dual, capture csv for both vesc
* for csv file, I love the graphs. Would love it more if somehow it could show min/max/avg especially for amps/watts
* trips, if there was a trip called "most recent" that shows totals/avg/min/max for current or most recent trip.
* I'm only familiar with PPM, but some kind of live PPM display

I think my biggest use for this is to understand if I'm bumping into limits so I can adjust things like braking strength, so having min/max/avg/totals for recorded trips would be awesome. Of course I can copy off and crunch the csv, but it's nice to have it in the app.
```

---
## \#165 Posted by: philvanzu Posted at: 2017-08-14T18:41:48.028Z Reads: 219

```
Great App & firmware. Just donated.

I'd love to get audio feedback, mostly battery level, for when your phone is in the pocket.
IE when battery voltage passes some threshold the phone vibrates, rings or outputs some audio file.
I'd be down to contribute the code myself if you were willing to get help or go open source. I'm mostly a win desktop programmer with no xp at all in android development but outputting audio can't be that hard to implement I imagine.
```

---
## \#166 Posted by: deucesdown Posted at: 2017-08-15T13:55:32.615Z Reads: 223

```
If you haven't already figured this out,

* splitting receiver wire will only let you monitor one VESC. I tried doing this with 2 bluetooth modules, but connection was flakey. Perhaps they interfere.

* selecting number of motors in the app automatically multplies the relevant numbers (amsp, watts, etc) by number of motors. You don't have to do math in your head.

* using can bus master/slave, you can tell the app to talk to the "local" vesc (the vesc the bluetooth module is attached to), or another vesc on the can bus by its ID. Side note, I don't think you can talk to the "local" vesc via canbus ID

* be careful of canbus settings, especially with traction control turned on! Turned low speed cogging into an adventure for me.
```

---
## \#167 Posted by: Pimousse Posted at: 2017-08-21T17:41:35.177Z Reads: 216

```
@Ackmaniac : analyzing another ride with my dual VESC 6, I figured out that duty cycle is only integer in the csv file (either 0 or 1).
Could you have a look to this ?
Thanks ! :wink:
```

---
## \#168 Posted by: Ackmaniac Posted at: 2017-08-21T17:56:53.146Z Reads: 212

```
So Vesc 6 works again with the app? I will have a look.
```

---
## \#169 Posted by: Pimousse Posted at: 2017-08-21T19:17:59.393Z Reads: 216

```
It has always worked with the VESC 6, but no more with my regular VESC 4.12. ;)
```

---
## \#170 Posted by: Ackmaniac Posted at: 2017-08-21T22:11:30.969Z Reads: 221

```
Does the duty cycle look ok in the realtime data that is visible?

Edit. think i fixed the problem. also fixed a bug in the Graph Visualization of the app. That's in Version 1.46
```

---
## \#171 Posted by: Pimousse Posted at: 2017-08-22T04:25:53.834Z Reads: 225

```
Thanks for being responsive !
About the connection issue with my other board, do you change something on the BT side  in the last updates ?
Or must I investigate on the HW side ?

And any plan on the warning voltage/range/capacity feature ?
(Sorry for being insistent, I'm being asked very often with this one by french guys :wink: )

Cheers !
```

---
## \#172 Posted by: markyoe Posted at: 2017-08-23T22:06:35.027Z Reads: 220

```
What's the pinout for the VESC so I know where to connect the bluetooth module to?
```

---
## \#173 Posted by: Ackmaniac Posted at: 2017-08-23T22:51:43.565Z Reads: 252

```
I just released a new Version a couple of minutes ago which has a nice new Feature. You can measure the acceleration of your board.

Once you click on the Speed Box the app tells you that it will start to measure when the board comes to a complete stop.
When it is ready to start then you see "Ready to go".
Now you can start to accelerate.

You will see a result like this:
<img src="/uploads/db1493/original/3X/a/2/a271ab3de880bb7383b9702ac7b73ed1bdaa62e8.png" width="294" height="500">
1: shows the seconds needed to accelerate from 0 - 10 km/h
2: shows the seconds needed to accelerate from 10 - 20 km/h
3: shows the seconds needed to accelerate from 0 - 20 km/h
a.s.o
The last lines shows the seconds needed to accelerate till the maximum reached speed.

To start another testrun you should click the speed box to stop the measurement and click it again to start from new.

Have fun
```

---
## \#174 Posted by: Ackmaniac Posted at: 2017-08-24T10:40:10.669Z Reads: 240

```
Realized that when mi/h is used then steps of 10 mi/h are a bit too much. So i changed it to steps of 5 mi/h for the acceleration data.
```

---
## \#175 Posted by: Pimousse Posted at: 2017-08-24T12:16:02.952Z Reads: 245

```
http://www.electric-skateboard.builders/t/vesc-hm-10-bluetooth-wiring/12838/19?u=pimousse
```

---
## \#176 Posted by: philvanzu Posted at: 2017-08-24T18:48:23.645Z Reads: 241

```
Will this work with a kickstart? my 400 kv motors have no torque at all when stopped.
```

---
## \#177 Posted by: Ackmaniac Posted at: 2017-08-24T19:38:53.887Z Reads: 238

```
Sure. Just give it a try.
```

---
## \#178 Posted by: philvanzu Posted at: 2017-08-25T20:35:59.093Z Reads: 243

```
Sure will.

So I found a roundabout way to get audio alerts with vesc monitor. Activating a developer option to log all BT traffic in a file. I then just have to read that file to get all telemetry data. Getting audio alerts after that is child's play.

proof of concept : 
[https://youtu.be/ZPyg_2yS2VQ](https://youtu.be/ZPyg_2yS2VQ)

I'll polish that for a bit then make a github and maybe a dedicated thread.
```

---
## \#179 Posted by: Mickyboy Posted at: 2017-08-25T22:48:49.127Z Reads: 237

```
Brilliant!!
```

---
## \#180 Posted by: The_Dude Posted at: 2017-08-26T14:35:46.674Z Reads: 236

```
Trip specific recording - I have the same data in the total and the trip 1-3 views. Where do I have to select which trip is recorded? Thanks!
```

---
## \#181 Posted by: Ackmaniac Posted at: 2017-08-26T14:41:26.441Z Reads: 241

```
You can reset Trip 1, 2 or 3 by selecting it and then press long in the screen. The app will ask you then to reset the Trip. It Worms like the little Button in Most cars at the odometer. It just Starts to count from there.

Actually reminds me that there was s little bug. Because when you reset tue data the screen doesn't refresh so that you still see the old data. But it works.
```

---
## \#182 Posted by: The_Dude Posted at: 2017-08-26T15:04:59.273Z Reads: 239

```
Yep, think I forgot to reset after changing from total to trip1 before riding. So each ride is recorded to all trips, and the distinction is made just by resetting at the start?! Thanks!
```

---
## \#183 Posted by: Ackmaniac Posted at: 2017-08-27T00:03:54.586Z Reads: 253

```
I just applied a new version of the app which fixes the refresh issue of the trip modes when they are reset and also a nice little feature many wanted me to implement.

Now you can get warning sounds when the Battery is below 50%, 40%, 30%, 20%, 10% and 0%.
You can enable it in the battery setup screen. 
The sound that is played is **"Warning! Battery at 50%"**
But please be aware that the sound will only be as loud as your actual ringtone volume.
<img src="/uploads/db1493/original/3X/8/f/8f9b831c578586d3fbeff42d322f5812979c0c4c.png" width="282" height="500">
```

---
## \#184 Posted by: The_Dude Posted at: 2017-08-27T07:52:57.182Z Reads: 224

```
Hi Nico,
just curious: I suppose, you use the current voltage of the pack for the alarm. The battery Wh is used for the estimation of the remaining range - is this done linear or you use some kind of battery model? Can you explain a little on that, because I mostly have quite high km-ranges left and in the end they "drop down" quite fast. 

Thanks
Dude
```

---
## \#185 Posted by: Ackmaniac Posted at: 2017-08-27T08:07:26.598Z Reads: 223

```
Because of that you define yourself in 10% steps at which voltage the battery has how many % capacity left. Can be seen in tue picture above.
```

---
## \#186 Posted by: The_Dude Posted at: 2017-08-27T08:20:05.407Z Reads: 227

```
Yes ... but then, how do you calculate the Range? I wonder for what purpose resp. how you use the "Battery Wh" in the Battery Setup.
Just curious to know, because I run the same board with different battery setups and want to keep the changes when swapping the batteries (different s, different capacity) to a minimum.
```

---
## \#187 Posted by: Ackmaniac Posted at: 2017-08-27T13:24:06.504Z Reads: 228

```
First i calculate the capacity in percent. Then Wh multiplied with that percentage which gives me the left over Wh. And the the actula Wh consumption devided by the left over Wh.

E.g.
Wh 400
100% 4.2
90% 4.1
80% 4.0
70% 3.9
60% 3.8
50% 3.7
40% 3.6
30% 3.5
20% 3.4
10% 3.3
0% 3.3

Voltage is at 43.2V for a 12S Battery it is which is 40% capacity because the single cell voltage is 3.6V.
40% * 400Wh = 160Wh

If the actual Wh consumpion is 12.5 Wh/km you have 12,8 km left. (160 / 12.5)

So if you want to use different batterys it would b good that they are of the same type. Because then the capacity would match for the single cell voltage. So you only need to change the Wh and the amount of cells.
```

---
## \#188 Posted by: Pimousse Posted at: 2017-08-27T13:29:07.417Z Reads: 217

```
Congrats ! That's amazing !
Hack of Ack' :smile:

@Ackmaniac : Is VESC Monitor compatible with latest Android 7.0 Nougat ?
```

---
## \#189 Posted by: Ackmaniac Posted at: 2017-08-27T13:47:43.716Z Reads: 211

```
Think so. No chance to try but should work.
```

---
## \#190 Posted by: Maxid Posted at: 2017-08-27T13:48:24.495Z Reads: 216

```
I am using it on a Nexus 5 with 7.1.1 and works perfectly fine
```

---
## \#191 Posted by: Pimousse Posted at: 2017-08-27T13:50:58.027Z Reads: 218

```
Perfect. That was the only blocking point for upgrading my Nexus 5X.
For you, is it worth it ?
```

---
## \#192 Posted by: Maxid Posted at: 2017-08-27T14:08:49.900Z Reads: 217

```
I am always trying to stay up to date - even if it is just for the security updates.
```

---
## \#193 Posted by: The_Dude Posted at: 2017-08-27T15:37:14.594Z Reads: 209

```
Hi,
one more question regarding the "Trip Feature". The recorded distance in t trips seem to be approximately twice the distance I actually rode (and which is shown in the "normal" screen). I'm running a dual motor setup, could this be the reason?
```

---
## \#194 Posted by: Ackmaniac Posted at: 2017-08-27T16:45:30.835Z Reads: 201

```
Heard about that bug before. But i can't reproduce it. For me it is working reliable.

Edit: Found the bug. It happens when you switch from the realtime data screen to the video recording screen.
```

---
## \#195 Posted by: Ackmaniac Posted at: 2017-08-27T17:44:42.616Z Reads: 205

```
Just released a new version 1.51 which fixes that issue. Thx for the info.
```

---
## \#196 Posted by: The_Dude Posted at: 2017-08-27T18:53:26.365Z Reads: 203

```
BAM - that's what I call responsiveness :+1:
Thanks!
```

---
## \#197 Posted by: L3chef Posted at: 2017-08-27T19:04:33.245Z Reads: 209

```
You need tp update to 7.1.2 asap then :smile: jk
```

---
## \#198 Posted by: L3chef Posted at: 2017-08-30T06:11:11.670Z Reads: 212

```
My canbus is not working on my dual setup. Can I use 2 bluetooth modules and still change the modes with the app?
```

---
## \#199 Posted by: TarzanHBK Posted at: 2017-08-30T06:21:09.340Z Reads: 213

```
what´s wrong with you canbus?
```

---
## \#200 Posted by: L3chef Posted at: 2017-08-30T08:13:45.180Z Reads: 222

```
I have no Idea. They refuse to communicate. I think the can bus chip is broken on one of the vesc's. Not sure since it power on and everything else works.
I have a thread about the issue. If you have some idea what might be wrong, please feel fee to suggest options :slight_smile:
```

---
## \#201 Posted by: Trdolan03 Posted at: 2017-09-01T00:24:59.918Z Reads: 226

```
How close is a IOS app?
```

---
## \#202 Posted by: thisguyhere Posted at: 2017-09-02T08:11:13.545Z Reads: 225

```
hey @Ackmaniac, what does orange color on the block header indicate?

 <img src="/uploads/db1493/original/3X/a/0/a065f94bd58fdd65b60869246b8279630b7a5e15.jpg" width="690" height="388">
```

---
## \#203 Posted by: Ackmaniac Posted at: 2017-09-02T08:34:34.588Z Reads: 224

```
That you reached the battery cutoff start. When you reach the cutoff end it will turn red. By this you see that you touched a limit. The temperature box also does the same.
It means that the power get's reduced to stay in the limits so that the battery doesn't get over stressed and that the VESC itself doesn't overheat..
```

---
## \#204 Posted by: thisguyhere Posted at: 2017-09-02T16:52:05.500Z Reads: 216

```
Yea now that you say it, it's obvious.
```

---
## \#205 Posted by: SageTX Posted at: 2017-09-02T22:55:35.034Z Reads: 217

```
Is there a way to backup setup info /modes /trip info to migrate to a new phone?
```

---
## \#206 Posted by: BigBoyToys Posted at: 2017-09-13T03:00:51.969Z Reads: 215

```
[quote="rich, post:150, topic:20888"]
Hey @Ackmaniac, the app worked well but since i've updated my HW 4.12 to FW 3.26 there is no more realtime data visible. I've updated the app today so it's the newest version.
[/quote]

Same problem here, any update on this?
```

---
## \#207 Posted by: BigBoyToys Posted at: 2017-09-13T05:00:52.107Z Reads: 219

```
[quote="guyguy, post:153, topic:20888, full:true"]
The app seems to crash if the board gets disconnected or turned off when the app is running in the background. It's also really hard to kill the app when it's frozen.
[/quote]

I also have noticed this. Im using the galaxy S8 plus and 3.26 fw.
```

---
## \#208 Posted by: krloz Posted at: 2017-09-14T12:26:54.734Z Reads: 219

```
Quick question
Anyone have the app properly running on android 7.0
My phone wants to update but I'm not going to allow it if i risk the app
Thanks
```

---
## \#209 Posted by: Pimousse Posted at: 2017-09-14T12:33:32.158Z Reads: 223

```
No worries, it's compatible.
```

---
## \#210 Posted by: SeanHacker Posted at: 2017-09-14T12:35:51.717Z Reads: 227

```
Works fine. 

<img src="/uploads/db1493/original/3X/3/3/336585c757d1517d579326f1cec1a9d6c9e467db.jpg" width="690" height="124">
```

---
## \#211 Posted by: krloz Posted at: 2017-09-14T12:52:49.139Z Reads: 221

```
Thanks. I will update then
```

---
## \#212 Posted by: Ackmaniac Posted at: 2017-09-21T02:37:51.363Z Reads: 223

```
Just released a new update which should gives a better VESC-Tool Firmware support. For the VESC-Tool Users i recommend to use Version 3.28 because there a UART bug has been fixed.

I also added a better battery support so that different battery types can be choosen. (Li-Ion, Li-Po and ANR26650 (A123) and Costum). Li-Ion are adjusted for Samsung 30Q Batterys. Just spent a lit of time to get a good preset for each type. But still each one of them can be adjusted individually.

Also fixed a bug for the warning notifications when the battery runs low.
```

---
## \#213 Posted by: krloz Posted at: 2017-09-22T11:36:33.186Z Reads: 211

```
 I have been having an issue with the app. Both when I had android 6 and now with 7. Occaisionally (I haven't been able to find a common reason) the app freezes. It will show the frozen values on all boxes and no information in the notification bar. And if I close it and open it again it will show an empty screen work no Bluetooth devices to connect to. I have to open app administration and force close the app. Any clue why this could be happening?
```

---
## \#214 Posted by: Pimousse Posted at: 2017-09-22T12:29:11.698Z Reads: 208

```
It crashed a lot for me as well (Android 6 and 7).
Just updated to Android 8, I'll give a try this evening and report.
```

---
## \#215 Posted by: Paulf Posted at: 2017-09-23T15:45:30.475Z Reads: 213

```
<img src="/uploads/db1493/original/3X/d/4/d44bf80f15b6e3bf509928405e05fd11d974e9dd.png" width="281" height="500">
<img src="/uploads/db1493/original/3X/d/3/d360082e47fbdc94523f43d76912af356166a048.jpg" width="269" height="500">
Does anyone know why my range would stay at 0?
```

---
## \#216 Posted by: Paulf Posted at: 2017-09-23T15:56:48.177Z Reads: 194

```
Also the app crashes when I try to delete a board, just after I type "Delete"
```

---
## \#217 Posted by: Ackmaniac Posted at: 2017-09-23T21:42:56.828Z Reads: 202

```
Just released a new Version where the Range and the Delete Bug is fixed. Thx for the info.
```

---
## \#219 Posted by: Ackmaniac Posted at: 2017-09-26T11:38:28.727Z Reads: 205

```
Just released a new version of the app which asks you to disable the battery optimization for phones with Android M or higher. That hopefully fixes some issues that people have with more modern smartphones.
```

---
## \#220 Posted by: SageTX Posted at: 2017-09-26T17:59:42.935Z Reads: 209

```
~~Any idea why I can't scroll through the settings in the mode setup?~~

Sorry misreading the labels!

Brake setting is Motor Min :blush:
```

---
## \#221 Posted by: Ackmaniac Posted at: 2017-09-26T18:21:47.675Z Reads: 200

```
No sorry. No idea and first time I hear that. Do you have a modded firmware?
```

---
## \#222 Posted by: SageTX Posted at: 2017-09-26T18:27:34.371Z Reads: 201

```
Edited my post... Sorry

I was looking for "brake max" and  should  have been looking for "Motor min"  Doh!
```

---
## \#223 Posted by: Maxid Posted at: 2017-09-26T20:06:20.237Z Reads: 207

```
Is there a way to change the y axis limits in the plotted graph? Two finger pinching only changes the x axis on my phone and to have a look at for example the battery voltage the y axis limits are way too big.
```

---
## \#224 Posted by: spares Posted at: 2017-09-27T07:21:07.959Z Reads: 208

```
@ackmaniac loveing the app, dislike the frozen / disconnects. But that is andriod.

I wanted to know how others have set up for the raptor2, max/min for this and that.

Also is there any way to log controller inputs as I have been getting some gliches. When crusing the poser drops offs with no change in throttle position. I have to go to idle then apply power which is slow in coming then blasts off. Scares the hell out of me. Any help thanks
```

---
## \#225 Posted by: Maxid Posted at: 2017-09-27T16:34:25.410Z Reads: 208

```
I have yet another feature idea:
When changing the modes there should also be the option to change batteries.
I have a 10S Liion, a 6S Liion, a 6S Lipo and a 7S Lifepo battery at home and it would be great if I could switch them out during a run without the need to have a computer with me to readjust the low voltage cut-offs.
```

---
## \#227 Posted by: krloz Posted at: 2017-09-28T10:01:59.170Z Reads: 198

```
I second that idea.  This would be awesome for the build I am currently doing where I have interchangeable packs of same s count but with different capacities
```

---
## \#228 Posted by: Maxid Posted at: 2017-09-28T10:36:01.392Z Reads: 201

```
Why would you need the feature if all you change is the capacity?
Voltage cut offs only need to be changed when switching chemistry or S count.
```

---
## \#229 Posted by: krloz Posted at: 2017-09-28T12:45:35.858Z Reads: 210

```
Yeah i know. But why would we want to have the feature of changing driving modes when you can change the amp limits
Just saying it would be nice to switch batteries by clicking on it instead of having to remember and type the amp. Maybe the statistics could be stored for each battery to compare them also
```

---
## \#230 Posted by: Pimousse Posted at: 2017-09-28T13:13:16.081Z Reads: 205

```
[quote="krloz, post:229, topic:20888"]
But why would we want to have the feature of changing driving modes when you can change the amp limits
[/quote]

Simply because a mode is not only a matter of amps limits but also ERPM limit, control mode, custom throttle curve... ;)
```

---
## \#231 Posted by: krloz Posted at: 2017-09-29T07:17:58.396Z Reads: 200

```
Battery chemistry. Correspondence between volts and percentage.  Capacity. I would even suggest a max amp limit to adapt to different capacities and discharge rates. 
What's your point?
```

---
## \#232 Posted by: notger Posted at: 2017-10-06T09:36:22.694Z Reads: 200

```
I have a damaged CAN port on my Dual-Focboxes.
So out of need i use servo-split cable now.
my question now:
the only option to really monitor both VESC would be two bluetoot modules, right.
but how does the app differ betweend the VESCS then ?

greets
Notger
```

---
## \#233 Posted by: Ackmaniac Posted at: 2017-10-06T09:44:31.187Z Reads: 199

```
The app will detect this as another Board. So if you want to change a mode sou have to connect to both vesc individually. It's just a bit annoying but this way it is still possible to change modes
```

---
## \#234 Posted by: E-Boarding Posted at: 2017-10-06T10:47:54.427Z Reads: 199

```
Is there some sort of security or can everybody with this app connect to my board and change my settings?

I'm going to test this with a Raptor 2 and try to shutdown the brakes or something while the other person is riding it, this is potentially very dangerous, at least a password protection would be good.
```

---
## \#235 Posted by: krloz Posted at: 2017-10-06T12:18:53.503Z Reads: 201

```
I think this was talked about before.  Nobody will be able to connect to your board as long as you are connected before.  That's why I'm adding a switch to the 5v line of the Bluetooth to turn it off when I dont intend to connect my phone
```

---
## \#236 Posted by: Trdolan03 Posted at: 2017-10-10T14:46:23.523Z Reads: 197

```
Any chance you are working on an IOS version?
```

---
## \#237 Posted by: caustin Posted at: 2017-10-15T19:27:45.601Z Reads: 208

```
@Ackmaniac   Quick one, have my Raptor 2 up and running, had to reprogram a new replacement rear assembly so used the Enertion version of BLDC for settings now written to VESC as default mode.

Now using the Ackmaniac app works fine for viewing live data, video logging etc, but not able to write any of the other modes (example advanced, pro, etc or custom I built).  I am pressing the mode box (showing default settings) and get the choose the drive mode screens and pick one by pressing but only returns to same main screen with same default settings.

What am I missing, does the Raptor 2 not come with the modified firmware allowing changes to be made from app (not just BLDC tool)?   I am able to switch between FOC/BLDC (and already did motor detection calibration for both) from the app by long pressing the Mode box to get overwrite default settings screen, so it seems to be able to write to VESC for that.  ??
```

---
## \#238 Posted by: Martinsp Posted at: 2017-10-15T19:42:20.521Z Reads: 197

```
I have the same problem where I am not able to actually change the mode. I click on it, the box disappears but it still is set to "default"  I am using 2.54FW 4.12HW and V1.59 of the app.
```

---
## \#239 Posted by: Martinsp Posted at: 2017-10-15T19:46:26.853Z Reads: 200

```
Where do you have a graph in the app :O
```

---
## \#240 Posted by: ninja Posted at: 2017-10-15T20:20:02.021Z Reads: 203

```
Seems like it is your phone. I had same issue, sometimes I needed to long press even up to 10 times to get it to pick my desired mode. So I tried with my girlfriends phone and issue is gone. So my phone have some issues with blue tooth low energy. Try with different phone and also make sure it is different model of phone. Don't try with Samsung J3, it has issues.
```

---
## \#241 Posted by: caustin Posted at: 2017-10-15T20:23:15.944Z Reads: 200

```
GRaphs are in modes setup if you pick a mode to edit and then tick box use special throttle curve etc
```

---
## \#242 Posted by: caustin Posted at: 2017-10-15T20:23:59.877Z Reads: 195

```
Arghhh let me try and see if phone is issue though using two phone android already and no luck lol
```

---
## \#243 Posted by: Ackmaniac Posted at: 2017-10-15T20:32:00.786Z Reads: 199

```
I just tested it again and it is working as it should. Could it be that you made a firmware update of your phone? And which phone do you use?
```

---
## \#244 Posted by: Martinsp Posted at: 2017-10-15T20:35:11.822Z Reads: 188

```
I just tried it with Samsung galaxy s5 mini and it works so it is definitely a phone issue :/
```

---
## \#246 Posted by: Ackmaniac Posted at: 2017-10-15T20:51:19.179Z Reads: 185

```
Thx for the quick test.
```

---
## \#247 Posted by: caustin Posted at: 2017-10-15T21:33:34.086Z Reads: 189

```
TI am using a R1 HD BLU. Android 6 security latch level June 1 2016

And a Jelly Pro Android 7.0 security patch level sept 5 2017
Kernel 3.18.35

Same problem with both. Does not recognize mode change. Is there any other way to select change modes by app as I am out of android phones for now lol
```

---
## \#248 Posted by: caustin Posted at: 2017-10-15T21:36:46.740Z Reads: 188

```
Using v1.59 of app
```

---
## \#249 Posted by: Ackmaniac Posted at: 2017-10-15T21:51:57.899Z Reads: 184

```
Try to reinstall the app. If i  remember right one guy fixed it by that. The problem is that the Bluetooth low energy integration in the firmware of the smatphones is sometimes bad. 
If you have the chance please try it on another board (not the raptor) with my new firmware mod. If it woks with the new firmware then i know how to improve it. 
Sadly i can't test it myself because all my smartphones work with the app.
```

---
## \#250 Posted by: danielz Posted at: 2017-10-16T01:03:39.062Z Reads: 188

```
I want to say a big thanks for the app, i love data! Its been very helpful. I appreciate the amount of work that goes into making an app. You have saved me many days of work trying to write one myself!

Using z5 compact, latest updates, genuine hm-10 with crystal.
```

---
## \#251 Posted by: karma Posted at: 2017-10-16T20:26:01.630Z Reads: 192

```
Damn this app is amazing @Ackmaniac! It works great but I think I have a bug in the Default panel. It says my Max km/h speed is 227km/h. I set up 10S with 40T WHeel pulley and 15T Motor pulley with 90mm wheels. Tried to search in this topic but couldn't find anyone with the same problem. Any ideas why?
```

---
## \#252 Posted by: Ackmaniac Posted at: 2017-10-16T23:32:22.188Z Reads: 198

```
Because if no max ppm is set in the PPM settings then the VESC takes 200000 ERPM as default. Now worries, it's all good. If you don't want that the VESC does limit the speed then simply set the speed to like 100 km/h (a speed you can never reach)
But most people will recognize that it feels a bit like hitting a wall when you reach max speed. So i recommend to set the max speed to 2 km/h more then you can reach. Because modes which are defined by the app will start to reduce the pwoer 10% before you reach max speed. By this the power get's slowly reduced before you reach max speed which feels much smoother.
```

---
## \#253 Posted by: Ackmaniac Posted at: 2017-10-17T11:54:04.878Z Reads: 222

```
Just released a new version where the motor temperature is visible if temp sensors are installed in the motor. It only works with the firmware since version 3.xx
<img src="/uploads/db1493/original/3X/a/7/a7798e1d8cbabc970fc79412c9a402f72af62230.png" width="357" height="375">

If no temp sensor are installed you will see the average temperature as before.

Would be great if someone who has temperature sensor in the motor could make a video. Sadly i don't have one myself.
```

---
## \#254 Posted by: Ackmaniac Posted at: 2017-10-18T12:02:38.478Z Reads: 215

```
Just renamed the app to AKMANIAC-ESC Monitor according to the Trademark Policys
```

---
## \#255 Posted by: BigBoyToys Posted at: 2017-10-22T09:08:15.339Z Reads: 218

```
  I updated my app, have 3.100 FW on an FOC box and  temp sensored motors (Carvon V3's), but the motor temp does not display on the App or on the video during recording.  It just has a Theta undernrath the mosfet temp. Ideas?
```

---
## \#256 Posted by: bsancken Posted at: 2017-10-23T23:52:47.965Z Reads: 207

```
I have updated to 3.1 on my FOCBox  (hw  4.12) and I can no longer connect to the vesc. It says connected, but instead it doesn't show any values or anything. I have un installed and reinstalled the app.  This was working perfectly on fw 2.54, but I mistakenly thought I did need to upgrade to 3.xx but now the app won't show anything. 

Nothing except the Fw version has changed, but that shouldn't affect it since you had just said it was updated to work with the new fw version... 

Thanks
```

---
## \#257 Posted by: Ackmaniac Posted at: 2017-10-23T23:54:16.406Z Reads: 198

```
Check that you use PPM and UART as control mode or UART if it is the lave VESC and also set a baudrate of 9600.
```

---
## \#258 Posted by: bsancken Posted at: 2017-10-23T23:58:46.842Z Reads: 185

```
That would be it! (ppm -> ppm + UART) I swear I checked it, but I'm still not used to using the esc-tool and where all the settings are. (I really do enjoy the modified bldc tool, but there doesn't seem to support 3.1) 

Thank you!
```

---
## \#259 Posted by: BigBoyToys Posted at: 2017-10-24T00:13:13.428Z Reads: 171

```
Can anyone tell me how to change modes using the app? There doesnt seem to be an apply mode button.
```

---
## \#260 Posted by: bsancken Posted at: 2017-10-24T00:24:41.119Z Reads: 176

```
Click the top left box (the one with the Max W and such, to the left of speed) That'll make the popup for selecting the modes that you set u using the pencil/edit button
```

---
## \#261 Posted by: Ackmaniac Posted at: 2017-10-24T00:26:45.125Z Reads: 196

```
Click here. And if you press long on that box you will be asked if you want to use the actual settings as the new default.
<img src="/uploads/db1493/original/3X/8/0/800e86441c300b6d65bb368ec094e7fe6e1af151.png" width="383" height="500">
```

---
## \#262 Posted by: BigBoyToys Posted at: 2017-10-24T00:39:46.351Z Reads: 188

```
Thanks,

But how will the app know which of the modes I want to use?
```

---
## \#263 Posted by: Ackmaniac Posted at: 2017-10-24T00:49:33.196Z Reads: 183

```
It lets you choose one of your modes.
```

---
## \#264 Posted by: caustin Posted at: 2017-10-24T01:38:46.738Z Reads: 189

```
Yeah it took awhile for me to get modes working on my phone.  Don’t worry about defaults and long press, you need to confirm that a single quick press of mode box brings up a menu of modes to choose from and that if you click on it then that it then populates the modes box with right values. If that works then you can set default etc but need to get mode change working first. That was a problem on a few android phons I tried.
```

---
## \#265 Posted by: BigBoyToys Posted at: 2017-10-24T01:49:54.666Z Reads: 185

```
It works! Thanks guys
```

---
## \#266 Posted by: caustin Posted at: 2017-10-24T02:30:41.488Z Reads: 179

```
Great, really useful to change modes and current/watt control BLDC/FOC etc on the fly. Should be interesting if you are using to monitor all 3 slave vesc by canbus as well. Not sure if Ackmaniac has any custom settings in mind for AWD like he has for dual diagonal offset config. Anyway would be interested in swing your trip logs of 4wd posted. Would like to compare to 2wd at some point and see the differences lol.
```

---
## \#267 Posted by: BigBoyToys Posted at: 2017-10-24T02:43:51.370Z Reads: 174

```
I dont connect via can bus as Ive had too many issues with It. I have a separate BT module for each VESC for tuning and comparision purposes but just use one of the modules for efficiency testing and then multiply by 4.
```

---
## \#268 Posted by: caustin Posted at: 2017-10-24T02:52:18.746Z Reads: 176

```
Nice. Yes canbus canbe scary sometimes lol
```

---
## \#269 Posted by: Ackmaniac Posted at: 2017-10-24T08:11:11.362Z Reads: 181

```
Via the app you can also adjust a 4WD. You can define 2 controller id's for the front axle.
@BigBoyToys you can set number of motors in the app to 4. By this the values get multiplied automatically.
Did you try already different settings for the front and rear axle? Like 30% acceleration power at the front and 70%  on the back and at braking the other way round.
```

---
## \#270 Posted by: BigBoyToys Posted at: 2017-10-24T08:52:35.180Z Reads: 183

```
I have run different settings front and rear on my other 4wd boards but with the big grippy 107's on the Carvon V3's it doesnt seem to be needed.  It doesnt have enough torque with the big wheels to break traction during hard acceleration or braking.

Im gonna be testing is some more tomorrow with the 83mm flywheels and will use the front rear power split you described if it starts breaking traction. I will be using it for sure on the 8085mm 4wd board Ill be finishing up in the next couple of weeks but again I dont use 4wd can bus anymore since its been problematic for me. I just run four separate bluetooth modules.

This is a truely amazing app. I couldnt get your donation link to work but I sent a token of appreciation to your email address via PayPal.

Thanks again
<img src="/uploads/db1493/original/3X/2/3/232f981b11c808af08418bdf9825f55b8980d8ae.jpg" width="690" height="419">
```

---
## \#271 Posted by: BigBoyToys Posted at: 2017-10-24T09:39:36.971Z Reads: 171

```
[quote="caustin, post:268, topic:20888"]
Yes canbus canbe scary sometimes
[/quote]

Fear turned into about 7 blown CAN transceivers. Zero since I abandoned CAN.
```

---
## \#272 Posted by: BigBoyToys Posted at: 2017-10-24T09:43:34.120Z Reads: 174

```
[quote="Ackmaniac, post:269, topic:20888"]
set number of motors in the app to 4. By this the values get multiplied automatically.
[/quote]

Do all the values displayed get multiplied? I felt like some weren't so if figured Id leave it set to one and multiply myself just to be sure until I asked.

I seem to have lots of freezing issues but its intermittent and unpredictable. When the app freezes its almost impossible to close and restart without waiting. Is there anything I can do to minimize this? I use a GALAXY S8 plus btw.
```

---
## \#273 Posted by: Ackmaniac Posted at: 2017-10-24T09:47:07.377Z Reads: 179

```
I think it doesn't only help when you loose traction. It also could help for stability. For example when you only power the front wheels then it is hard to make a corner. SO it should be helpful to have less power at the front to improve carving during acceleration. And at braking it also should be more stable when the front brakes more than the back.

And i am working on the crashes. But did not find the root cause yet.
```

---
## \#274 Posted by: BigBoyToys Posted at: 2017-10-24T10:07:50.003Z Reads: 177

```
Ill give the power split a try tomorrow and see if I can feels a difference in the way it handles.
```

---
## \#275 Posted by: guyguy Posted at: 2017-10-24T13:04:18.433Z Reads: 178

```
I personally don't like traction control. With it off at least I know what it's doing, that is, it's still responding to the throttle in a predictable way to me. When TC is on and I hit a slick spot while accelerating resulting in a motor to spin up suddenly it feels like it pumps the brakes on the wheel with traction at worst and at least it stops behaving how I'm expecting it to given the trigger position.
```

---
## \#276 Posted by: notger Posted at: 2017-10-24T15:08:42.194Z Reads: 181

```
[quote="BigBoyToys, post:271, topic:20888"]
Fear turned into about 7 blown CAN transceivers. Zero since I abandoned CAN.
[/quote]


Hi,
so, what do you mean with "blown CAN reansceivers", do you know more about it, or know anyone able to repair it ? how does a blown CAN Transceiver look like or can you/i acutally see it ?

I actually made a similar experience with my brand new Focboxes ? not many people seem to know about CAN troubles, or at least the only advice given to me is "use a servo split cable its safer than CAN" on the other hand Trampa is strictly recommendin not to use servo split-cables with their new VESC6
I go with servo split right now, and its working great, still id like to know ,...is this a random bug, or a production fault,...or...

if anyone knows more about it here i openen a topic with questions to it

[http://www.electric-skateboard.builders/t/dual-vesc-can-problems/34035](http://www.electric-skateboard.builders/t/dual-vesc-can-problems/34035)
```

---
## \#277 Posted by: Ackmaniac Posted at: 2017-10-24T17:22:06.765Z Reads: 163

```
Just released a new version of the app (1.62) which hopefully improves the stability of the app. Please let me know if it males a difference on your phone? Will take a couple of minutes for google to publish it so please be patient.
```

---
## \#278 Posted by: BigBoyToys Posted at: 2017-10-24T17:51:23.926Z Reads: 172

```
Installed, will test this evening and report back.
```

---
## \#279 Posted by: guyguy Posted at: 2017-10-24T17:57:07.257Z Reads: 175

```
Thanks for your work

Every 300 miles I run on your app I'm going to drop you a donation
```

---
## \#280 Posted by: BigBoyToys Posted at: 2017-10-24T18:33:45.347Z Reads: 176

```
Whatever you did drastically improved the stability on my phone. Im running a cloned version and the Original version on the phone at the same time and it hasnt frozen once even when both are connected and switching back and forth between the apps and when connecting and disconnecting. The app did stop once when switching from video back to the main screen but it restarted fine which wasn't the case before. It would hang up for over a minute and sometimes not eork again until I turned off the board. Quick work, nice improvement.
```

---
## \#281 Posted by: caustin Posted at: 2017-10-24T20:06:39.833Z Reads: 181

```
This thing is awesome, really liking now that I have an android phone that works for mode change.  Taking a closer look, on the two android phones that still do not work (even with recent update v1.62), it is just the mode selection dropdown page that is the issue on some phones.  Everything else works (including changing default and BLDC/FOC) but for some reason some phones are not able to pickup the selection of a new drive mode from that drop down screen and pass it along to the main app mode box.  So it acts as if nothing was chosen so nothing changes.  I know its not a priority, but would be great if that mode change drop down menu worked like the FOC/BLDC change menu, as the mode change feature is top of list for many people.  I expect the different UI for mode change dropdown vs FOC/BLDC is driven by the fact that the menu options are dynamic and pulled from the modes setup section of the app (vs FOC/BLDC and default write to VESC are hardwired options).  Even a command level prompt box where we type in a drive mode would help, not pretty but at least works. Just throwing that out there lol.
```

---
## \#282 Posted by: notger Posted at: 2017-10-24T20:08:14.468Z Reads: 175

```
[quote="BigBoyToys, post:280, topic:20888"]
Im running a cloned version......................
[/quote]

Interesting, so you are able to read data of both motors on two "cloned" Ack-Apps ?.
Are both apps able to connect to both bluetooth modules at the same time, and read and write data of both motors ?
And sorry, im still a oldschool mobile user, but i got a android 4.4 Smarthpone gifted, so how do you clone apps ?
```

---
## \#283 Posted by: Ackmaniac Posted at: 2017-10-24T20:27:04.195Z Reads: 170

```
Do you have another Board where sou can try my or benjamins new firmware? If it works with this  then I Know the reason.
```

---
## \#284 Posted by: Surfer Posted at: 2017-10-24T20:47:55.501Z Reads: 178

```
Hi Nico, just i would like to know if is there a option to keep the track of the kilometers i do skating with your f+C++g awesome app, since i change very often the mobile phone i can't keep it, is a there a way to edit the km? thanks buddy, i'm in love with your brain. :+1::nerd:
```

---
## \#285 Posted by: BigBoyToys Posted at: 2017-10-24T20:52:22.079Z Reads: 172

```
Yes they can both apps can connect to the separate bluetokth modules and read data and change modes :). Just search "clone app" on the play store.
```

---
## \#286 Posted by: caustin Posted at: 2017-10-24T21:03:12.032Z Reads: 175

```
Ah yes, I remember you had pointed me in that direction before.  I do have a couple of beta vesc 6 as well as few Ollin VESC that I would need to install your FW to.  Probably this weekend, so just to clarify I can try this with the beta vesc6 w/vedder FW already installed (I have not updated it in quite awhile) or I need to install your FW on my Ollin VESC HW v4.12?  Also to double confirm which version of your firmware should I use with the Ollin VESC?
```

---
## \#287 Posted by: Ackmaniac Posted at: 2017-10-24T21:19:18.931Z Reads: 170

```
You can use Version 3.100 on both.
```

---
## \#288 Posted by: caustin Posted at: 2017-10-24T22:31:33.912Z Reads: 171

```
Ok great. As I already have dual beta vesc 6 up and running on a build and just need to add BLE, will the test work with existing new Vedder HW for some reason or need your FW 3.1?  Rather not change variables if possible lol.
```

---
## \#289 Posted by: Ackmaniac Posted at: 2017-10-25T01:15:51.186Z Reads: 173

```
You need Firmware 3.100 to try the mode change
```

---
## \#290 Posted by: BigBoyToys Posted at: 2017-10-25T01:50:12.331Z Reads: 175

```
Im still trying to figure out why motor temp isnt displayed on my App. Any tips?
```

---
## \#291 Posted by: Ackmaniac Posted at: 2017-10-25T02:12:56.110Z Reads: 181

```
Which temperature does it show in the realtime window on you pc?
```

---
## \#292 Posted by: bsancken Posted at: 2017-10-25T03:15:20.116Z Reads: 200

```
As far as I can tell, the app really dislikes it if it is connected to the board, and you power cycle the board without hitting disconnect. It doesn't happen all the time, but when it does, it hangs, goes white, then the android "App has crashed" pops up for like .5 seconds. I have to force stop it and re-launch it to get it to be able to re-connect it.

Verizon S8
FocBox hw 4.12 fw 3.1 (? sounds right?) 
with a HM-10 bt le
Switching on/off with Vedder anti-spark.


Edit 
----------
Did it again, no errors on vesc. The app froze and in trying to get out of the app, the crash dialogue popped up and disappeared before I could hit the submit report.



----------


**Edit #2**

----------
Timeline- Ride the board with it connected, turn off board, go to class. 

After class, turn on board, look at app and it is in this state. 

(Picture Below)

Attempt to hit disconnect and/or Back (leave that "Board's app in screen)  causes the app to freeze and eventually crash if not force stopped.

 After force stopped, open it and it works as normal. 

<img src="/uploads/db1493/original/3X/9/c/9cc37d63db244c61d3833cc069729f445805b25c.png" width="243" height="500">
```

---
## \#293 Posted by: BigBoyToys Posted at: 2017-10-25T03:16:15.825Z Reads: 194

```
Both were visible as different colored lines in the VESC tool 3.26. I belive in yours 3.100 as well, but Id have to disassemble the board to check now.
```

---
## \#294 Posted by: Maxid Posted at: 2017-11-01T12:04:16.316Z Reads: 190

```
How does the App deal with uneven dual drives? I have two different motors with two different gear ratios and have even set different amp settings for each of the VESCs.
This means I can't just multiply values by two right? Is there another way to know what both VESCs are using in terms of Wh etc.?
```

---
## \#295 Posted by: Ackmaniac Posted at: 2017-11-01T17:01:53.053Z Reads: 189

```
You have to connect by can to the slave then and read the values individually and calculate them yourself. But at least my modded Firmware gives you the chance to define different amp settings for each Motor so that they run on different Power.
```

---
## \#296 Posted by: Fabian287 Posted at: 2017-11-02T07:42:32.490Z Reads: 186

```
Can you connect the Bluetooth module to the slave vesc and use all the Features like to connect it to the master? @Ackmaniac
```

---
## \#297 Posted by: Maxid Posted at: 2017-11-04T16:01:09.672Z Reads: 187

```
Went for rides today and have to report that the app does not work for me anymore. The app does not connect to the module even though I can see it in the overview. Got it to connect twice in around 40 tries with app and phone restarts in between.
Using V1.62 on an S8.
```

---
## \#298 Posted by: Titoxd10001 Posted at: 2017-11-18T02:25:27.680Z Reads: 188

```
Since average wh/mile is saved can you use that to estimate range when barely connecting and then after riding a bit it switches to wh/mile during the ride like normal. Would be cool if we can manually set wh/mile it estimates range when barely connecting to

Also the white logo/notification I'm unable to close it when the app freezes. I have to force stop it every time which takes a bit of time. Is there a fix for this.

If I walk away from my board it will freeze pretty much guaranteed
```

---
## \#299 Posted by: gaetjen Posted at: 2017-11-22T18:45:13.452Z Reads: 183

```
Is there any chance that I can extent the range of the blutooth connection? Antenna or somehting like this?
```

---
## \#300 Posted by: louwii Posted at: 2017-11-23T03:07:41.763Z Reads: 188

```
What HM-10 do you guys use with the VESC? Is a cheap one like that working ok ?

https://www.aliexpress.com/item/HM-10-CC2541-CC2540-4-0Bluetooth-UART-Transceiver-Module-Transparent-Serial-Port/32279636502.html
```

---
## \#301 Posted by: rich Posted at: 2017-11-23T19:47:54.618Z Reads: 195

```
Buy this one, @Ackmaniac provided the link somewhere and it works flawlessly...

https://www.aliexpress.com/item/HM-10-BLE-Bluetooth-4-0-CC2540-CC2541-Serial-Wireless-Module/32516357718.html?spm=a2g0s.9042311.0.0.oMpQCM
```

---
## \#302 Posted by: louwii Posted at: 2017-11-24T01:18:33.098Z Reads: 197

```
Thanks ! Super cheap, that's perfect.
```

---
## \#303 Posted by: yaca Posted at: 2017-11-25T14:02:09.680Z Reads: 200

```
I talked about this problem long time ago and still exists for me. I'm the only one who has this strange colours in videos? It only happens when I choose Video Layout - Left and Right. My phone is an Samsung Xcover3 - Android 5.1.1

<img src="/uploads/db1493/original/3X/8/6/86e89fead50ac322cfe71355dd995ae3f7b19e91.jpg" width="240" height="144">

Video Layout - Left - has no Problem

<img src="/uploads/db1493/original/3X/9/1/9167588874f9fff71733f72782ded9e6075a6f8e.jpg" width="240" height="144">
```

---
## \#304 Posted by: Ackmaniac Posted at: 2017-11-30T23:04:06.314Z Reads: 187

```
Just released a new version of the app which hopefully fixes the main error for crashes. Please let me know if you still have trouble with the new version.
```

---
## \#305 Posted by: b264 Posted at: 2017-12-01T02:30:06.473Z Reads: 185

```
Where can we find the source code?
```

---
## \#306 Posted by: Titoxd10001 Posted at: 2017-12-09T01:22:40.578Z Reads: 182

```
Since the newest update some of my values are not saving as soon as turn off the screen. Min voltage, max speed, power and temperature. Worked beforehand
```

---
## \#307 Posted by: BigBoyToys Posted at: 2017-12-09T01:28:03.194Z Reads: 169

```
Have you had anymore crashes? Im planning a long ride this weekend and would really like to have all the stats on one log.
```

---
## \#308 Posted by: Titoxd10001 Posted at: 2017-12-09T02:21:17.123Z Reads: 166

```
I believe I had one frozen screen but probably my fault because I keep forgetting to move module outside of carbon enclosure. Would be nice if it reconnected automatically as it always freezes if I walk a couple of yards away from my board. Even if app freezes at least total distance, total wh and wh/mile are saved on vesc.
```

---
## \#309 Posted by: Titoxd10001 Posted at: 2017-12-10T08:43:12.009Z Reads: 189

```
<img src="/uploads/db1493/original/3X/0/3/03383db3313514824b7bc9a7f89c08c4e59d8d35.jpg" width="381" height="500">

<img src="/uploads/db1493/original/3X/6/9/69b631dacff89e136c20829dde89bf492032db39.jpg" width="690" height="151">
```

---
## \#310 Posted by: BigBoyToys Posted at: 2017-12-10T09:10:33.245Z Reads: 199

```
@Ackmaniac  I rode for 7hrs strait today using your app the whole way. Sadly Im still having freezing issues but I still think It's improved from a few versions back. I had to restart the app about 5 times and force end it twice over my 7hrs and 102mile ride. 

I also noticed something weird with the battery percentage. At the 55mile mark it read 50%. Then, 5 miles later it suddenly dropped to 36%, then by 65miles it was back up to 40%.

Also, I noticed a few times there was no battery percentage displayed then it would magically reappear. Is the perecent based off of the whr capacity I enter off the cell voltage?

Awesome app!
<img src="/uploads/db1493/original/3X/0/8/0820c6093177da86bcb77dbb4e8b515796941786.jpg" width="690" height="335"><img src="/uploads/db1493/original/3X/5/0/50fea6e2cfed75fc68264356663a1e908c51827f.png" width="690" height="500"><img src="/uploads/db1493/original/3X/f/0/f0431ee2f9569c98583930ba2738890a1f5eedc1.jpg" width="690" height="500">
```

---
## \#311 Posted by: Exiledd_Top Posted at: 2017-12-10T16:14:37.929Z Reads: 180

```
What build did u use .... Holy shit... 7 hours of nonstop fun that battery must be big to push you that far
```

---
## \#312 Posted by: BigBoyToys Posted at: 2017-12-10T18:35:56.618Z Reads: 179

```
12S 36Ah 1600whr Lipo. I just took the Carvon motors off the evo deck and put them on the Trampa I won the 4wd challenge on.
```

---
## \#319 Posted by: mmaner Posted at: 2017-12-12T19:05:25.636Z Reads: 172

```
whats with all the flag happiness?
```

---
## \#320 Posted by: ShutterShock Posted at: 2017-12-12T19:07:00.327Z Reads: 175

```
Probably non-relevance to the thread.  Not sure
```

---
## \#321 Posted by: BigBoyToys Posted at: 2017-12-12T22:12:43.456Z Reads: 177

```
Yeah, we started talking about how to mount Carvons on a Trampa deck. My apologies for the clutter @Ackmaniac.
```

---
## \#322 Posted by: Ackmaniac Posted at: 2017-12-12T22:55:43.535Z Reads: 179

```
no problem!
```

---
## \#323 Posted by: caustin Posted at: 2017-12-12T23:13:04.377Z Reads: 177

```
My bad, back to topic!
```

---
## \#324 Posted by: Trdolan03 Posted at: 2017-12-20T18:27:59.538Z Reads: 173

```
@Ackmaniac When I go to switch from FOC to BLDC or BLDC to FOC, I accept that the board needs to restart but the mode stay the same. Am I missing a step?
```

---
## \#325 Posted by: Ackmaniac Posted at: 2017-12-20T20:50:58.605Z Reads: 170

```
Did you configure both modes?
Does it switch? 
Can you hear the difference by the motor sound?
```

---
## \#326 Posted by: Trdolan03 Posted at: 2017-12-20T21:11:19.769Z Reads: 174

```
It was not switching based upon the sound and the display still had it as FOC. My VESC won't connect to my computer anymore after I attempted to update firmware though another phone app to test it.
```

---
## \#327 Posted by: Ackmaniac Posted at: 2017-12-21T00:13:47.130Z Reads: 178

```
My app only allows to switch the motor mode when both (BLDC and FOC) are configured.
Configured means they don't have the default values anymore.
This way i make sure that the users don't do mistakes, or at least i try to avoid them.
And you need to use my firmware to switch the motor and control mods.
```

---
## \#328 Posted by: Titoxd10001 Posted at: 2017-12-26T08:11:39.309Z Reads: 180

```
Wh/ah bug when I switched modes

<img src="/uploads/db1493/original/3X/3/f/3fcac3dfe0ec7214a975a0dbdb515c60de1eb32e.png" width="395" height="500">
```

---
## \#329 Posted by: Ackmaniac Posted at: 2017-12-26T08:42:54.603Z Reads: 171

```
Don't really see a issue. Can you explain in detail?
```

---
## \#330 Posted by: Titoxd10001 Posted at: 2017-12-26T08:59:21.014Z Reads: 178

```
I made a class with very low settings. 100watts max and 18mph max. When I switch to it my wh/mile is under 4 but it should be closer to 15. Also data showed I was only pulling like 60watts and 2 amps going 18mph which is unlikely. I'm not sure if the weird numbers I was getting is specific to that class with low values
```

---
## \#331 Posted by: Ackmaniac Posted at: 2017-12-26T09:28:14.084Z Reads: 177

```
Switch to the new mode and make a video with the app. Then it is much easier to analyse.
```

---
## \#332 Posted by: Titoxd10001 Posted at: 2017-12-26T22:42:50.758Z Reads: 185

```
In the screenshot above my wh/mile is 3.4 so my estimated range on 12s7p would be 250+ miles. Here are some screenshots to better understand what I mean. They're about the same speed just different modes.

Default
<img src="/uploads/db1493/original/3X/6/4/64f470968f2c088b7855b472a2627c60df6d3340.jpg" width="690" height="335">

Low watt mode.
<img src="/uploads/db1493/original/3X/1/9/19509bc60928b81dcc23273d388d25b7de811f9e.jpg" width="690" height="335">
```

---
## \#333 Posted by: Ackmaniac Posted at: 2017-12-26T22:57:21.521Z Reads: 171

```
In your last picture the WH/km are correct. I think you just played around with the "No of Motors".
When this is set to one then it only count's the values of one VESC. So to see the total consumption it should be set to number of motors you have on your board.
```

---
## \#334 Posted by: Titoxd10001 Posted at: 2017-12-26T23:36:23.198Z Reads: 181

```
I didn't change the number of motors, they're both set to 2. This was just around the block so my wh/mi just gets lower and lower which you can see in the last row wh/mi both under acceleration one is 14.8 and the low watt mode is 6.5, both feel the same while riding

Unrelated from above issue. I made trip and distance traveled was jumping around one minute apart. Real numbers should be 10.3 miles traveled with about 18wh/mile
<img src="/uploads/db1493/original/3X/7/7/779effc5f6e2af98ad29423b3a0c2e3ac32b0ef6.png" width="243" height="500">

<img src="/uploads/db1493/original/3X/d/0/d004c9e9bf6ce8f629ef8850acde67c5ef77876d.png" width="243" height="500">
```

---
## \#335 Posted by: ducktaperules Posted at: 2017-12-26T23:43:14.854Z Reads: 170

```
For what it's worth I feel like I have been having a similar problem to this. I get the same data for trip 1, 2, 3 and total. And the more I ride the less my wh/mile seems to be getting
```

---
## \#336 Posted by: Ackmaniac Posted at: 2017-12-26T23:55:12.950Z Reads: 179

```
I can see that the distance get's more but the wh drawn and charged stay the same. Then of course the calculation get's wrong. Need to have a look how this can be caused.
```

---
## \#337 Posted by: Ackmaniac Posted at: 2017-12-31T20:10:45.711Z Reads: 176

```
Just released a new version which fixes the issue that min and max values were not updated when the screen was switched off in between and the videos are now full screen without navigation bars when you have a phone that has no physical buttons.
```

---
## \#338 Posted by: thisguyhere Posted at: 2017-12-31T20:55:36.423Z Reads: 185

```
totally unnecessary idea, but....

when recording video with overlay, have an option to turn on solid color, green probably, so one can key out the color and overlay onto another video in post editing. 

I find hand holding my cell phone while riding somewhat dangerous, I've completely destroyed a phone while doing so. 

a lot of us have gopros and such mounted to helmets or otherwise.  it'd be nice to be able to layer the telemetry onto another video file.
```

---
## \#339 Posted by: scepterr Posted at: 2017-12-31T20:58:40.674Z Reads: 188

```
Btw, working on my phone at least, with Android 8.0.0, I believe the fix was in the kernel

https://www.electric-skateboard.builders/t/bluetooth-hm-10-not-discoverable-on-android-8-0-8-1-oreo/36713/41
```

---
## \#340 Posted by: guyguy Posted at: 2017-12-31T21:08:23.202Z Reads: 186

```
You can recorded screen of the app (just its regular telemetry view, not video recording mode) while riding and insert it into your go-pro ride videos.
```

---
## \#341 Posted by: Ackmaniac Posted at: 2018-01-01T23:55:59.786Z Reads: 186

```
I just released a new version where i added the altitude information. It is shown to the left of the actual distance value.
But be aware that the altitude which is detected by GPS isn't the most reliable. And it also takes a little while until there is good GPS signal. But just give it a try. I hope that altitude changes can then be seen in the videos. Maybe even the climb degrees can be calculated then. But need to do more test drives to see how good and quick the height detection is.
```

---
## \#342 Posted by: Sebike Posted at: 2018-01-02T00:09:28.838Z Reads: 178

```
I never got the app to work with GPS, ie never got GPS speed reads. Running a SONY Xperia Z3. Anyone else having this issue and a possible solution?
```

---
## \#343 Posted by: Ackmaniac Posted at: 2018-01-02T00:11:19.533Z Reads: 180

```
In the app you have to go to settings and enable "Save GPS position".
And on your device GPS needs to be enabled of course.
```

---
## \#344 Posted by: Sebike Posted at: 2018-01-02T00:13:46.145Z Reads: 177

```
That's been enabled, but still doesn't work. GPS needs to be enabled on my phone or it won't pair with the BT module..
```

---
## \#345 Posted by: Sebike Posted at: 2018-01-02T14:36:36.610Z Reads: 181

```
Don't know if you changed something in your latest 2 updates, but for the first time GPS readings work! TY
```

---
## \#346 Posted by: Ackmaniac Posted at: 2018-01-02T14:41:20.881Z Reads: 187

```
You have to test the GPS feature outside. Inside you don't get a GPS signal if your roof is too thick and even outside it might take a couple of seconds before a signal is detected.
```

---
## \#347 Posted by: Sebike Posted at: 2018-01-02T14:43:59.756Z Reads: 193

```
Sure. I've been having the GPS enabled all the time though when riding (outside lol), but never got any reads until now. One can see that on previously posted uploads with app overlays. Glad it seems to be working now.

https://youtu.be/hHey1FhLqeI
```

---
## \#348 Posted by: Flapjackz Posted at: 2018-01-08T05:00:22.260Z Reads: 184

```
Will this work in conjunction using the Nunchuck as the controller?
```

---
## \#349 Posted by: Mathias Posted at: 2018-01-17T03:56:50.803Z Reads: 186

```
First, thanks @Ackmaniac  for all the work and for this awesome app!

Did you share the source code somewhere? I can't seem to find it in your git hub repository. I'm trying to monitor the battery temperature and figured the easiest way would be to hook it up to the motor temperature slot. But it seems the app doesn't monitor it (well, it's useless for 99.9% of the builders here). I thought if I could have a look at your code, I could easily find a way to monitor the temperature on my phone while riding!
```

---
## \#350 Posted by: chrisongtj Posted at: 2018-01-20T08:54:38.452Z Reads: 187

```
is there a way to save data to a log file instead of video?
```

---
## \#351 Posted by: Ackmaniac Posted at: 2018-01-20T13:47:37.698Z Reads: 181

```
It does that automatically. Just click on the gallerie button in the status bar and you can see the files.
```

---
## \#352 Posted by: chrisongtj Posted at: 2018-01-20T14:05:16.111Z Reads: 178

```
Ok will try, thanks!
```

---
## \#353 Posted by: louwii Posted at: 2018-01-22T07:12:08.811Z Reads: 184

```
Hi there,

I finally have everything put together. I tried your app since it really looks neat, but it wasn't able to find my bluetooth module, the list stays empty in the app.
When going to bluetooth devices, my phone sees the HM10 module (listed as MT05 I believe).

I tried another app, VESC CONNECT, and it did see and connected to my VESC (but it throws a firmware not up to date error, which is bullshit since I've updated my firmware yesterday). That app doesn't really look nice though, I'd prefer to use yours !

I checked the connection, everything seems to match, VCC to 5V, GND to GND, TX to RX and RX to TX. I'm not sure what else I can do to debug it.
```

---
## \#354 Posted by: Ackmaniac Posted at: 2018-01-22T07:45:01.159Z Reads: 173

```
Did you set the baudrate to 9600? And sometimes a smartphone restart helps.
```

---
## \#355 Posted by: louwii Posted at: 2018-01-22T07:51:51.196Z Reads: 183

```
Yep, baudrate to 9600. I'll try to reboot my phone.

Here's the rest of the config, if any of that matters.

![VESC bluetooth module|690x167](upload://eP1bPVOj6b7N6yS75bd8Kr4Q4Rl.PNG)
```

---
## \#356 Posted by: louwii Posted at: 2018-01-23T02:42:38.387Z Reads: 177

```
Looks like I was being stupid. I activated the localization and the app worked right away !
```

---
## \#357 Posted by: paul15578 Posted at: 2018-01-24T04:58:28.793Z Reads: 187

```
Hi @Ackmaniac 
The app is great thanks,I mostly  love having all the max stats which Metr doesnt do,

A few things if you are looking for feedback from my few months of use.
1) I have lots of crashes of the app on two different android phones - you might have been getting my "send feedbacks"  htc m7 and samsung s7. Its random when it crashes but it freezes up, sometimes caused by the bluetooth disconnect when I turn the board off, (turning the board back on doesnt reconnect it, the app remains frozen), seems I have to wait for android to work out its crashed and show a wait or send feedback popup,.while troubleshooting I turn off bluetooth on the phone and try to close the app, which doesnt usually work unless I then wait, but I usually have to turn the bluetooth off to get it to reconnect by allowing the app to turn bluetooth back on itself through the popup request
2) sometimes I connect to the module and it shows no stats, I have to go back and connect again, sometimes multiple times, before it shows stats. It sometimes displays connect in the top right but even clicking that doesnt make it connect, I have to go back to click on my red module name
3) I have a phone velcro stuck to my board where I can see the "always on" screen, the speed is big and red and really easy to see but I cant really see any other stats, could there be a zoom factor introduced? and a custom ticking of which items to display?
4)  I was trying to use the record function the other day, it was connected but either straight away or after a few seconds it freezes up and shows either no stats at all or the stats that were showing when it froze.
5) Are you planning on allowing it to work with vesc 6 firmware please?

Sorry if this seems all negative but I am really just trying to see if it helps improve the app. Thanks
Regards
Paul
```

---
## \#358 Posted by: Bensaida Posted at: 2018-01-25T22:18:18.134Z Reads: 164

```
@Ackmaniac  Why dont modes work with my VESCs using your app? Im using FW 3.100 Maytech VESCs, using Ackmaniac watt mode.
```

---
## \#359 Posted by: Ackmaniac Posted at: 2018-01-25T23:11:29.226Z Reads: 164

```
You can't use Watt mode with firmware 3.100 because current control works now like watt mode. Change it to current control and see if it works.
```

---
## \#360 Posted by: Bensaida Posted at: 2018-01-25T23:17:38.914Z Reads: 168

```
Can i switch to current control from the app?
```

---
## \#361 Posted by: Ackmaniac Posted at: 2018-01-25T23:20:28.292Z Reads: 174

```
There isn't a such called watt control mode in the Ackmaniac-tool. And yes you can choose current control in the app. In 2.54 the is watt control and in 3.100 current control works the same as watt control in the previous firmware.
```

---
## \#362 Posted by: Bensaida Posted at: 2018-01-25T23:21:10.783Z Reads: 172

```
Hmm. So i am currently using current control. Still doesnt explain why changing modes doesnt do anything to the board
```

---
## \#363 Posted by: Ackmaniac Posted at: 2018-01-25T23:25:42.215Z Reads: 177

```
But you can see the realtime data?
```

---
## \#364 Posted by: Bensaida Posted at: 2018-01-25T23:28:01.537Z Reads: 180

```
Yes i can 10char
```

---
## \#365 Posted by: louwii Posted at: 2018-01-25T23:52:18.752Z Reads: 182

```
@Ackmaniac I always wondered, why is your custom VESC firmware not based on the most recent version ?
```

---
## \#366 Posted by: gaetjen Posted at: 2018-01-30T17:31:54.898Z Reads: 187

```
Since I saw the duell between the raptor2, the evolve gt and the boosted board on youtube I wanted to check my time on a 50m and 100m sprint with my board to compare them. Is it possible that you include something like this into your app. I know you have the 0-30kmh time stopping funktion, but maybe you can enhance that function :slight_smile:
```

---
## \#367 Posted by: louwii Posted at: 2018-01-30T18:36:56.978Z Reads: 189

```
Oh yeah, esk8 drag-race. And then we can generate a leaderboard.
```

---
## \#368 Posted by: Ackmaniac Posted at: 2018-01-30T19:04:22.386Z Reads: 196

```
Will think about it.
```

---
## \#369 Posted by: Brando Posted at: 2018-02-03T19:16:19.287Z Reads: 191

```
I read through this thread but couldn't see if anyone got this app working with VESC 3.34 firmware. can anyone confirm this?
```

---
## \#370 Posted by: louwii Posted at: 2018-02-03T19:23:12.982Z Reads: 201

```
I've updated my VESC in January 2018 to the latest version available at that time and the app is working fine with it.
```

---
## \#371 Posted by: Brando Posted at: 2018-02-03T19:34:56.324Z Reads: 203

```
Awesome! time to get a Bluetooth module!
```

---
## \#372 Posted by: Martinsp Posted at: 2018-02-06T14:25:59.650Z Reads: 208

```
![sketch-1517927022313|281x500](upload://diyFI04B9J0ME19FfqX1icU751u.png)
Nothing important, just a little mistake. Thought I would let you know if there are any significant updates worth making this might be easy to fix. BTW: great app, appreciate your work! :)
```

---
## \#373 Posted by: TarzanHBK Posted at: 2018-02-06T14:32:34.542Z Reads: 197

```
It´s carnival time here, so a Costume is totally fine :monkey:
```

---
## \#374 Posted by: Ackmaniac Posted at: 2018-02-06T15:11:36.342Z Reads: 195

```
Thanks for the hint. will be fixed in the next version. Currently working on a more reliable bluetooth connection.
```

---
## \#375 Posted by: Brando Posted at: 2018-02-08T21:09:52.056Z Reads: 195

```
When I connect to my module it isn't reading any values. It just shows the main screen with all stats displaying zero. I am running on the 3.34 firmware updated via the VESC Tool.
```

---
## \#376 Posted by: louwii Posted at: 2018-02-10T02:38:27.363Z Reads: 196

```
Have you enabled UART on your VESC ?
Baud rate to 9600 ?
```

---
## \#377 Posted by: Brando Posted at: 2018-02-10T04:15:23.600Z Reads: 193

```
I use RC remote so its set to PPM and UART. I tried both 115200 and 9600. but I'll try 9600 again.
EDIT: The Vesc Connect Pro app says VESC firmware is too old.
```

---
## \#378 Posted by: louwii Posted at: 2018-02-10T22:18:00.094Z Reads: 193

```
VESC connect pro is crap, it says the same thing for me but my VESC works well with @Ackmaniac's app.
```

---
## \#379 Posted by: Brando Posted at: 2018-02-10T22:41:00.334Z Reads: 195

```
I tried his app as well. It showed up as BT05, but when I tried connecting to it, all the stats on screen we're zero. I tried tapping the disconnect and connect button in the top right and it didn't seem to do anything. I may have to try a different device. I'm using my Android 7.1.2 tablet because my phone runs Android Oreo and BLE won't work.

EDIT: seems like my VESC had bigger problems. I had to reset the firmware with an ST-link because not even the usb connection would work. Bluetooth works great now! I have no idea what happened to my vesc though...
```

---
## \#380 Posted by: louwii Posted at: 2018-02-11T04:22:05.415Z Reads: 187

```
Weird. I had issues at first because I didn't activate the localisation. The app needs Bluetooth and localisation to work properly. 
Once I did that, the app found my board, I tapped it, gave it a name and setup pulleys and battery settings and that was it.
```

---
## \#381 Posted by: Ackmaniac Posted at: 2018-02-11T10:59:59.242Z Reads: 195

```
Yes it needs the right to read the location. Took me a couple of hours to find out that this is necessary for android to be able to use Bluetooth low energy.

@Brando did you set the baud rate to 9600 and crossed TX and RX on vesc and bluetooth module?
```

---
## \#382 Posted by: Sebike Posted at: 2018-02-11T23:12:04.432Z Reads: 191

```
Can the app handle dual vescs that are not connected to each other or do I need to switch between modules?
```

---
## \#383 Posted by: Ackmaniac Posted at: 2018-02-11T23:58:51.685Z Reads: 194

```
You have to switch between them. But I recommend to connect them via CAN.
```

---
## \#384 Posted by: junwoo091400 Posted at: 2018-02-18T07:53:38.421Z Reads: 189

```
@Ackmaniac I could see strange values coming in(FW2.18), and slow update speed. It is maybe a result of an EMI. And I wonder why that really happens. And I have a question, if I configure Bluetooth module & VESC to use 115200 baudrate, would it work with the Vesc-Monitor app? Thank you for your time&effort for building this amazing app :)
```

---
## \#385 Posted by: Ackmaniac Posted at: 2018-02-18T10:10:00.679Z Reads: 184

```
The app will work with 115200 as well. And I don't know why you have a slow update rate and strange data. Maybe try to switch to a newer version.
```

---
## \#386 Posted by: junwoo091400 Posted at: 2018-02-18T11:35:05.547Z Reads: 192

```
Thank you for response, here is my screenshot of the log where 'Wrong' values are logged
![VESC_Log_weirdValueAtOnce_capture|689x171](upload://aqgTDUVS9AXTdmGsp4i1Z6QNosc.JPG)
=> I am pretty sure somehow transmission data was corrupted/un-synced at those 2 moments.

And do you mean the bldc firmware or bldc-tool firmware by saying 'newer version'?? In that case, I got my VESC from @torqueboards and I am afraid I might mess up the drv-chip. What software can I upgrade, from Hardware v4.12 ?
```

---
## \#387 Posted by: rich Posted at: 2018-02-20T21:16:07.561Z Reads: 195

```
This is such a great App :heart_eyes: @Ackmaniac!

How much I have to donate for a second selectable theme like this? :laughing:

![VESC-Monitor-DARK|281x500](upload://hNTUxNCn9WoP8ZENNRuLw2gZJDT.jpg)

It would be great at night and even at day imo with grey numbers and the main ones in white.
```

---
## \#388 Posted by: Ackmaniac Posted at: 2018-02-20T21:55:57.258Z Reads: 186

```
I will give it a thought. Donations are always welcome.
```

---
## \#389 Posted by: AntiPusher Posted at: 2018-02-23T19:01:10.740Z Reads: 186

```
looks great!
```

---
## \#390 Posted by: Ackmaniac Posted at: 2018-03-07T20:44:03.138Z Reads: 190

```
I just released a new version of the app which has a changed BLE connection which should help to improve the stability of the connection.
It also has a black layout which can be activated via the settings.
And when you press on the distance box you activate drag measurement which shows you how lang you need for 0-25m, 0-50m, 0-75m, 0-100m, 0-125m, 0-150m, 0-175m and 0-200m meters from a standstill.

Google will need a couple of hours to provide the new version.
```

---
## \#391 Posted by: FabianOdermatt Posted at: 2018-03-07T20:48:48.039Z Reads: 178

```
Thank you so much for your work!
```

---
## \#392 Posted by: Acido Posted at: 2018-03-07T20:53:37.650Z Reads: 182

```
Is there a way for you to somehow make BLE work without location turned on?
And please add that black theme its so sexy!
```

---
## \#393 Posted by: Ackmaniac Posted at: 2018-03-07T21:05:27.946Z Reads: 179

```
I added the black theme in the new version. And BLE always needs the right to reed the location. For whatever reason. Can't avoid it. But after you gave the right you can simply switch off GPS on your mobile phone. BLE still works. It only needs the right.
```

---
## \#394 Posted by: Clonkex Posted at: 2018-03-07T21:59:54.115Z Reads: 177

```
I suspect it has something to do with the Google Beacons mentioned on this page: https://developer.android.com/guide/topics/connectivity/bluetooth-le.html
```

---
## \#395 Posted by: Jyrofpv1 Posted at: 2018-03-10T16:30:01.700Z Reads: 182

```
The board works correctly in default but when I select a mode it only changes one esc. Any ideas ![1520699328434306928573|690x388](upload://rLmTY2gi1Vh619QyqauDUKbE0PK.jpg)
```

---
## \#396 Posted by: GJHS Posted at: 2018-03-10T18:55:57.410Z Reads: 178

```
Are you connected through Can bus?
```

---
## \#397 Posted by: Jyrofpv1 Posted at: 2018-03-10T19:59:13.228Z Reads: 192

```
![Screenshot_2018-03-10-11-58-13|281x500](upload://yvITleGY6XJ6s9etx7C1ddMdM9.png)![Screenshot_2018-03-10-11-58-08|281x500](upload://noOXnAQmbHSUEGxhi5Ze3DUlhpK.png)
```

---
## \#398 Posted by: Jyrofpv1 Posted at: 2018-03-10T20:01:16.723Z Reads: 184

```
I tried both of these and I got the same results it would load in from the mode I selected  but only affect one ESC. I checked it by bench test with two different throttle curves and the throttle Curve will only affect one side
```

---
## \#399 Posted by: Ackmaniac Posted at: 2018-03-10T22:16:20.791Z Reads: 187

```
The throttle curve always only affects one side. Because you only need it at the master.
```

---
## \#400 Posted by: Jyrofpv1 Posted at: 2018-03-10T22:33:09.622Z Reads: 189

```
Ok thanks so its normal to only effect the master side at bench test when setting throttle curve and speed limit ? So I can ride it and under load it will be ok?
```

---
## \#401 Posted by: Ackmaniac Posted at: 2018-03-10T22:38:28.025Z Reads: 189

```
Just change the motor or battery amps with a new mode and check that these changes are also changed on the slave vesc
```

---
## \#402 Posted by: Jyrofpv1 Posted at: 2018-03-11T13:44:07.743Z Reads: 185

```
Cant figure how to see the individual ESC settings in the vesc monitor app.
```

---
## \#403 Posted by: Ackmaniac Posted at: 2018-03-11T17:23:47.930Z Reads: 181

```
You can't see all the actual settings. Only the motor amps, max speed and control mode can be seen in the upper left box.
```

---
## \#404 Posted by: Jyrofpv1 Posted at: 2018-03-11T17:30:04.106Z Reads: 183

```
Ok thanksss
```

---
## \#406 Posted by: Ackmaniac Posted at: 2018-03-22T21:07:18.723Z Reads: 185

```
This is how the dark theme looks like
![Screenshot_20180322-220402|250x500](upload://ascg8e4sWirbQOAVgxw6lCCsVFL.png)
```

---
## \#407 Posted by: rich Posted at: 2018-03-22T21:50:09.155Z Reads: 184

```
Thanks for reminding me to donate what I did right now :laughing:
If someone else want to show some love[ here you can donate](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=GJ59FXYPUQHUY).

I love the dark theme, already used it twice :grin:
Is it possible to use the dark theme in the video overlay as well? 

https://youtu.be/WIdTK5-xKyg
```

---
## \#408 Posted by: Ackmaniac Posted at: 2018-03-22T23:07:37.259Z Reads: 182

```
Sure it's possible but takes some hours. Need to find the time. Which firmware are you using? Because I see a little mistake of the app in your video which I want to fix.
```

---
## \#409 Posted by: Sender Posted at: 2018-03-22T23:15:42.585Z Reads: 187

```
Always on the job. You're the man!
```

---
## \#410 Posted by: scepterr Posted at: 2018-03-22T23:26:13.974Z Reads: 189

```
Is wireless tcp bridge something you've considered implementing?
```

---
## \#411 Posted by: rich Posted at: 2018-03-22T23:52:00.976Z Reads: 192

```
[quote="Ackmaniac, post:408, topic:20888"]
Sure it’s possible but takes some hours. Need to find the time.
[/quote]

ok I thought it could be quickly done, it's not that important, the main thing is the app anyway :wink:

I'm using the latest official FW 3.34 (vesc tool 0.87) with vesc 6
```

---
## \#412 Posted by: Acido Posted at: 2018-03-23T06:31:53.074Z Reads: 189

```
Could you make it possible to change voltage values with the app? 
It would practical, especially if you are "tuning" your board and have a lot of screws :)
```

---
## \#413 Posted by: advongunten Posted at: 2018-03-24T14:49:00.914Z Reads: 192

```
![ACKMANIAC_printscreens|590x500](upload://6sANYPZiYTUQcesdDd33XCbogmi.jpg)

@Ackmaniac
I've got your newest Version(1.70) of your VESC Monitor(Android) and found some wrong values,
but otherwise i loove it! Nice work! :slight_smile: 
- My "max km/h" was 217... I know i'm fast but... wrong gps-values maybe?
- red: I think there should be "km" instead of "m". As I changed it to miles, it was obviously.
  ("Distance" looks mess too, but i think not, because between the printscreens are 5 minutes of driving.)

What about a "used mAh" somewhere in a Panel?
So everyone with a DIY board could guess how big the capacity of the battery pack still is at the end of the trip btw if the battery is empty. 
I know with the percentage its like a redundancy... but coulomb measurement is more reliable imho and 
its more or less easy to implement because you already have all values.
```

---
## \#414 Posted by: Ackmaniac Posted at: 2018-03-24T16:24:29.751Z Reads: 180

```
used mAh is already there
![image|195x119](upload://msKW1ixJGh7WLMgbY70JQXAdFwG.jpg)

i will have a look for the m km issue
```

---
## \#415 Posted by: Ackmaniac Posted at: 2018-03-26T22:32:56.971Z Reads: 177

```
Thx for reporting the UI bugs.
I released a new version V1.71 which has now a dark theme in videos and fixed the range bug.
Also the Battery % and the range will keep it's values even if the board is switched off. This way it is possible to have a quick look how far you can still ride and at which state the battery is.
```

---
## \#416 Posted by: lazerusrm Posted at: 2018-03-28T06:33:42.207Z Reads: 174

```
Finally got it working with a different hm10 adapter off Amazon. amazing!!

is there documentation on how this works with dual vesc6? I was hitting some high amps scaring myself to death with brutal acceleration, and there is still more punch left! hit 96A...

Thank you for your work on this app. it's awesome! and thanks to Benjamin Vedder for being a complete badass.
```

---
## \#417 Posted by: Theos Posted at: 2018-04-04T14:01:31.145Z Reads: 175

```
Hi @Ackmaniac, First :big thank for you amazing app !! :wink:

since the update of my phone under Oreo (android 8.x) I have not reliable gps information in my logs when the screen of my phone is off (and the coordinates gps are ok if the screen is on)

I think it's related to the management of background task under Oreo 
( see here: https://developer.android.com/about/versions/oreo/background-location-limits.html )

can you confirm? an update of your app will solve this problem ?

thank for your help :grinning:
```

---
## \#418 Posted by: Chad Posted at: 2018-04-04T16:40:08.520Z Reads: 175

```
Do you need a phone that is connected to a data plan to use the map?
```

---
## \#419 Posted by: Ackmaniac Posted at: 2018-04-06T23:51:23.069Z Reads: 172

```
Thanks for the hint. I added some code which might fix the problem. Sadly i don't have a Android Oreo phone. So please give the new version a try which should be available in a couple of hours.
```

---
## \#420 Posted by: Theos Posted at: 2018-04-07T07:52:57.084Z Reads: 162

```
Thank 😁I will test tomorrow and report
```

---
## \#421 Posted by: Theos Posted at: 2018-04-08T17:26:00.784Z Reads: 160

```
Big Thank. It s OK with the last version 👍
```

---
## \#422 Posted by: SeanHacker Posted at: 2018-04-08T18:01:25.784Z Reads: 165

```
So are you running this app on Oreo? I still have yet to get it working on Oreo. It might be because we run custom AOSP. Not really sure yet though. 

![Screenshot_Settings_20180408-110059|281x500](upload://ciqXo3H2vuhDASRMfKA9HoyNj2q.png)
```

---
## \#423 Posted by: Theos Posted at: 2018-04-09T05:26:59.107Z Reads: 152

```
Yes running on mate9 on stock oreo build without root.  Maybe it's your rom..? What your problem exactly?
```

---
## \#424 Posted by: SeanHacker Posted at: 2018-04-09T12:05:10.186Z Reads: 153

```
With the latest update I can't even connect with my spare phone running Nougat that I've used solely for this app. @Ackmaniac Anything changed in the latest update that would do this?
```

---
## \#426 Posted by: MartyMcFly88 Posted at: 2018-04-09T14:40:21.780Z Reads: 157

```
What was the problem before, because i have a HM10 module that used to work, but doesn’t anymore since i updated my phone to android 8?
```

---
## \#427 Posted by: lazerusrm Posted at: 2018-04-09T15:00:03.512Z Reads: 159

```
mine didn't work at all before upgrading to android 8.. I ended up having to buy a different module off amazon, and it works fine for me using a verizon Samsung s8 plus, and the new module. maybe it's a permissions issue for some people?
```

---
## \#428 Posted by: MartyMcFly88 Posted at: 2018-04-09T15:03:10.812Z Reads: 159

```
could you link the module that you used?
```

---
## \#429 Posted by: lazerusrm Posted at: 2018-04-09T15:14:20.248Z Reads: 171

```
This is the one I ordered, and it worked just fine with ackmaniacs app, and ackmaniac firmware no modification required, and no voltage divider or anything, running on the vesc6 5v rail.

https://www.amazon.com/gp/aw/d/B06XH2CL43/ref=yo_ii_img?ie=UTF8&psc=1
```

---
## \#430 Posted by: Ackmaniac Posted at: 2018-04-09T15:25:44.152Z Reads: 172

```
Did you restart your phone already. Sometimes it happens that BLE has issues which only can be fixed by a restart. Running Nougat on my phone without issues.
```

---
## \#431 Posted by: SeanHacker Posted at: 2018-04-09T15:33:55.707Z Reads: 175

```
Yep. I rebooted my phone. Cleared data for the app. Fixed permissions. Nothing. Which is weird because I can't even connect to my R2 now either it seems. I've actually been running your app with no issues on Oreo with my R2. Do you have the previous version I could grab from you to test some things? I'll run a logcat when I get home and hooked up to my phone tonight.
```

---
## \#433 Posted by: Skitzor Posted at: 2018-04-16T15:30:57.228Z Reads: 173

```
OK, I will start to look into the android 8.0 (and above BLE issues). 
Got an S8+ No connection possible
Also bought a Metr module. No connection possible.
Fired up my second phone A5 (2017) on android 7. Both modules work instantly.

EDIT: Already found an important note from android which the DEVs could look in to

> Android 8 includes changes that bring both good and bad news. The bad news is that the existing workarounds will no longer work to let you detect beacons when you app is not in the foreground. The good news is that new APIs give you new ways of doing these same detections,

http://www.davidgyoungtech.com/2017/08/07/beacon-detection-with-android-8
```

---
## \#434 Posted by: Ackmaniac Posted at: 2018-04-16T18:27:45.132Z Reads: 162

```
Does the app detect the Bluetooth module or do you see no device?
```

---
## \#435 Posted by: SeanHacker Posted at: 2018-04-16T18:45:27.675Z Reads: 156

```
So now where I'm at is the R2 works now (on Oreo) just fine. But I still can't get my original module I've been using to connect unless on Nougat. Thinking I may just need to get a different module. Going to get the same one that's in my R2. 

The app sees the module, but its greyed out and not able to connect if I remember right. I can do some debugging tonight or tomorrow when I get home.
```

---
## \#436 Posted by: Skitzor Posted at: 2018-04-16T19:03:24.998Z Reads: 153

```
@Ackmaniac. It looks like the "old version" HM-10 modules could need a firmware update to comply with the new bluetooth standards of Android 8. Or as I've read, a different Bluetooth API needs to be used to comply (Oreo filters these packages from the beacon) with the old standards.
```

---
## \#437 Posted by: Teitanblood Posted at: 2018-04-16T19:04:43.875Z Reads: 155

```
For the last few days I'm not able to connect to my FOCBOX anymore through the Arckmaniac app (Android 7.0). The app actually sees the HM10 module but the numbers remain at zero when I try to connect. If I disconnect and try to connect again, the app freezes and I have to kill it. Everything was working flawlessly before. Maybe this is related with other's problems....
```

---
## \#438 Posted by: Skitzor Posted at: 2018-04-16T19:11:32.078Z Reads: 154

```
Doublecheck the Baudrate on the UART tab of that focbox. Standard should be 115200

EDIT: Standard for Enertion HMsoft BLE 4.0 module is baudrate 9600
```

---
## \#439 Posted by: rey8801 Posted at: 2018-04-16T19:37:10.743Z Reads: 173

```
@Ackmaniac I finally tested the app. I can connect and get the telemetry, although I then found the single ride split it in different files and if I make the video you can see that most of the time the app stops showing the data and the only thing still alive is the video and the GPS speed.  Talking about the speed I get 4kmh different between the speed tracked by the app and the one from the GPS (in the app). Another thing I set my max watt to 925 but then I see that the board draws more.
![vescmonitor|281x500](upload://fpYdM9iCzenoSRHB4kcWDsTeUuU.png)![vescmonitor|281x500](upload://nc5Pt2qRrR9W8t2XIszFmQAO1Q4.png)

I then tried to lower the watt and see if I can get the board really slow. I set it to 10watt and it was slower but still drew more. Do you know why?

Edit: @Ackmaniac  I read again your first post and my bad. I see that the value got multiple by 2 in case of dual set up. It makes sense, sorry. So the only thing that doesn't work properly with me is the module getting disconnected during the rides multiple times and the difference between the GPS speed and the ERPM one. Thx for your work
```

---
## \#440 Posted by: Teitanblood Posted at: 2018-04-16T19:38:00.493Z Reads: 148

```
Really? Everything was working juste fine before. I don't see why the baudrate would have changed...
```

---
## \#441 Posted by: Skitzor Posted at: 2018-04-16T19:43:06.304Z Reads: 158

```
[quote="Skitzor, post:436, topic:20888, full:true"]
@Ackmaniac. It looks like the “old version” HM-10 modules could need a firmware update to comply with the new bluetooth standards of Android 8. Or as I’ve read, a different Bluetooth API needs to be used to comply (Oreo filters these packages from the beacon) with the old standards.
[/quote]

Ok So I made some progress. I got the luxury of having 3 BLE modules for testing.

1. Chinese clone HM-10/BL-05 
2. Metr HM-10 (Probably chinese, no offence intended it looks identical to nr1) 
3. HMsoft BLE4.0 HM-10

Number 1 and 2 stopped working since android 8. I just got number 3 working on my S8+. So only the HMSoft firmware is complying Android 8 bluetooth low energy standard.

I got these modules, if there are any tests I can help you with. I gladly do the testing. I'm sure this is affecting lots of your users who upgraded to android 8 and are using cheap modules.

>This is why there is no issue with our out of box example and why I suggested you try this project. It appears your module vendor (or someone else) modified the firmware but didn't comply to the formatting described in BT4.x, Vol 3, Part C, Sec 11 which Android8 now adheres to. The BLE Stack will not enforce this as it's up to the application to comply with the layout. There are some custom applications that don't use this format, that's why we don't enforce it. 

Source: https://e2e.ti.com/support/wireless_connectivity/bluetooth_low_energy/f/538/p/670467/2472298
```

---
## \#442 Posted by: Ackmaniac Posted at: 2018-04-16T23:30:10.507Z Reads: 142

```
Maybe you can try to upgrade the firmware on the module. Fully occupied with my daytime job and use all my rare freetime for a new Ackmaniac-Esc firmware update at the moment.
```

---
## \#443 Posted by: xBRAZILx Posted at: 2018-04-18T17:09:41.255Z Reads: 148

```
yesterday i started the tests with a HM10 module that i bought.
after connecting the module to my vesc in my first test ride i had a problem that i´ve never had before.
once in a while my control shutdown for 1,5 second and i get the following error on the APP:

ERROR: FAULT_CODE_ABS_OVER_CURRENT

i am using the turnigy vesc 4.10 with firmware 2.18.
could be something with the module? i ´ve never had this problem with my control.

ps: the app is killer
```

---
## \#444 Posted by: SeanHacker Posted at: 2018-04-18T17:15:39.050Z Reads: 144

```
Totally understandable. Just ordered a programmer. I'll see what happens when updating the firmware for it.
```

---
## \#445 Posted by: rey8801 Posted at: 2018-04-19T12:47:28.578Z Reads: 155

```
I have already posted about it but I didn't get an answer yet. So sorry for me asking twice. Basically my initial problems was the speed not been the same as GPS measured and I understood that the problem is the gear setting. I am using hub motor (Meepo style) and the problem is that I do not know how many motor magnets to go with. I know my set up can go to 39kmh top speed so I will try to adjust to match it. If someone has same setup please share it is setting.
Second and main problem is that my bluethooth module keeps disconnectong as long I start to ride the board. I have notice that it keeps collecting the data although the app doesn't show any live streaming telemetry. I am using the AT-09 module which is basically the same as Hm-10. I realized too late (AT-09 !!!Android IOS HM-10 BLE Bluetooth 4.0 CC2540 CC2541 Serial Wireless Module
 http://s.aliexpress.com/Ariqm2MJ?fromSns=Copy to Clipboard) but it does connect, change VESCs setting ecc... But it disconnects frequently during the ride.
Next to this problem I also don't have any GPS data in the library. I don't know if  we hold get also a map out of it since in the app you can enable "save GPS position" but I don't get any GPS speed too. Here the last ride from this morning (speed completely wrong :persevere: ) 
![vescmonitor|281x500](upload://zj9gQ5Pmfri8rGTxCWT8KtnrZKa.png)  
Is it possible to post the whole session, as in metr app? Anyhow I don't see any GPS trace. Thx for the help.
```

---
## \#446 Posted by: linsus Posted at: 2018-04-19T12:57:32.288Z Reads: 134

```
I'm just going to go ahead and toss it out there since hes abit silent on here. BV is almost finnished with his app for the vesc6, going to be avaible through the playstore. With on the fly motor detection etc. Not sure on the ETA, but I've tried it myself and seems pretty  flawless.
```

---
## \#447 Posted by: DeathCookies Posted at: 2018-04-19T12:57:58.632Z Reads: 132

```
You can use the [VDLA](http://gct-hp.de/VDLA) app
```

---
## \#448 Posted by: rey8801 Posted at: 2018-04-19T13:08:44.362Z Reads: 145

```
I didn't know about. Thx! I should be put it in the first post. Anyhow I didn't see how to share the entire session since you can only download a picture and not a playable file. Anyhow I can see that the GPS location was recorded but the GPS speed as aspect ed is not showed![chart|690x459](upload://1h116M5eqUNNgVIsQJIIjYMlSB2.png)
Someone knows why?
```

---
## \#449 Posted by: DeathCookies Posted at: 2018-04-19T13:11:42.924Z Reads: 146

```
Because the line is hidden by Default. To make it visible just click on the greyed Label "GPSSpeed" and it will appear.
Everything is documented in its own thread:
https://www.electric-skateboard.builders/t/vesc-data-log-analyzer-vdla/16582
```

---
## \#450 Posted by: Ackmaniac Posted at: 2018-04-19T13:15:07.108Z Reads: 144

```
Try to place the BLE Module as far away from the battery or phase wires as possible. Especially when you draw current the signal can get disturbed. So try to place it away from the other components in your enclosure.
```

---
## \#451 Posted by: rey8801 Posted at: 2018-04-19T13:20:05.904Z Reads: 140

```
Ah ok thx. The thing is it is place as far as possible from the battery but right above the phase wire. The role that I don't have a space when it is far from both. That probably why it keeps disconnecting when I accellarate. Because the current in the phase wires increase. Although it records most the time the data in background. Wierd
```

---
## \#452 Posted by: Ackmaniac Posted at: 2018-04-19T13:25:31.033Z Reads: 140

```
When it continues to record in the background then it seems to be another issue which is maybe more related to your phone's android version. But first try to place it a bit better, maybe it helps.
```

---
## \#453 Posted by: rey8801 Posted at: 2018-04-19T13:28:51.847Z Reads: 151

```
Ok thx. Another question if possible. I made different  modes. Specifically one to let's people try out the eskate. When I switch to the slow one I feel the board slower but it still goes way faster than the speed I set. ![vescmonitor|281x500](upload://5ESJriPMHBC9fcw4WwErYu3hU3G.png)
Do yuo know why?
```

---
## \#454 Posted by: rey8801 Posted at: 2018-04-19T13:30:12.691Z Reads: 146

```
Thx for the help. Definitely the speeds doesn't fit![chart|690x459](upload://lkKw4B2LlzHxfuMZQydTC2FGBkc.jpeg)
A constant 3-6kmh difference

Edit: doesn't download the GPS speed. Wierd
![chrome|281x500](upload://rEexX2lL6csD2szXgSoyHR4zpaq.png)
```

---
## \#455 Posted by: DeathCookies Posted at: 2018-04-19T13:31:14.544Z Reads: 138

```
[quote="rey8801, post:453, topic:20888"]
When I switch to the slow one I feel the board slower but it still goes way faster than the speed I set.
[/quote]

@Ackmaniac i noticed the same bug! r2 max kmh of 5 does not work as expected. The watt is a bit lower and the difference is notable but the end Speed is not caped
```

---
## \#457 Posted by: xBRAZILx Posted at: 2018-04-19T14:13:08.263Z Reads: 140

```
![stranger_error|690x322](upload://yH8ZJJSBWoDwCVHQgxLzUB5HAQv.png)

after connectin the HM10 module to my VESC and collect the info with ack app i´m having this FAULT_CODE_ABS_OVER_CURRENT.
like you can see in the picture below the erro ocurred 7x in a short distance. Analysing the graph i coulnd´t understand why i am having this problem. it looks like i am not over anything, could somebody help me?
```

---
## \#458 Posted by: DeathCookies Posted at: 2018-04-19T14:17:59.546Z Reads: 139

```
Do you run FOC on 12S and the error happens when you accelerate hard?
Otherwise i have no clue
```

---
## \#459 Posted by: xBRAZILx Posted at: 2018-04-19T14:26:46.646Z Reads: 142

```
10s / bldc. smoothly acceleration
```

---
## \#460 Posted by: rey8801 Posted at: 2018-04-19T18:50:27.379Z Reads: 149

```
I just tried again the app. It does record in background. I don't know why it get stock on live streaming, also during a video recording with the app. I got a pretty accurate speed estimation with 20 poles. So for who has the Meepo style hub that is the setting that works the best with me. ![chrome|690x388](upload://C2FYJxg9ov7OMW5mxvDSUw2k0A.png)
```

---
## \#461 Posted by: Ackmaniac Posted at: 2018-04-19T19:48:46.303Z Reads: 144

```
Which smartphone do you use?
```

---
## \#462 Posted by: rey8801 Posted at: 2018-04-19T20:45:20.030Z Reads: 148

```
Xiaomi mi5 it uses miui that is based on Android. Usually I do not have compatibility problem. Could be this one the case?
```

---
## \#463 Posted by: Ackmaniac Posted at: 2018-04-19T21:56:05.548Z Reads: 150

```
Could be. My guess is that the performance of the phone is not enough and it kills tasks automatically. Happens also with slow phones when the video function is used and the realtime data overlay freezes.

Edit: had a quick look and the performance of your phone shouldn't be a issue. Maybe it's the Android implementation of it.
```

---
## \#464 Posted by: rey8801 Posted at: 2018-04-19T23:13:24.730Z Reads: 150

```
Indeed my phone should be power enough. Probably is the Android compatibility that is not 100% accurate. Thx for the help. Really appreciated. As also other mentioned before do you know why when we set lower speed and lower watt the board clearly slow down but still goes faster than what was supposed to go?
```

---
## \#465 Posted by: Ackmaniac Posted at: 2018-04-19T23:42:44.113Z Reads: 143

```
I don't have issues with that. You should test that ständing on the board. On the bench you can get false results. Maybe it also had to do with a wrong motor magnets setting in the app.
```

---
## \#466 Posted by: rey8801 Posted at: 2018-04-20T04:23:51.768Z Reads: 145

```
I tested by standing on the board. I will try again now that the ERPM and the GPS are almost the same. Thx!
```

---
## \#467 Posted by: TarzanHBK Posted at: 2018-04-20T08:03:38.998Z Reads: 152

```
![0e958de4675e1879f177caa051160c7c9f634389_1_281x500|281x500](upload://sTRMLvsDMw4rkVPssluLJx5tyiK.jpg)

20 magnets it is ;)
```

---
## \#468 Posted by: rey8801 Posted at: 2018-04-20T08:40:24.229Z Reads: 148

```
I went with the experimental way :sweat_smile:
I also found this picture that shows both magnet and motor ![wx_camera_1516597249069|690x500](upload://lWwdBijBBviEDLztSIdwA0oW6L4.jpg)
Now the two speed are really closed.
```

---
## \#469 Posted by: Ackmaniac Posted at: 2018-04-20T14:12:26.802Z Reads: 146

```
Just released a little update of the app:

When the app runs in the background and you switch off your board you should be able to open the app and still see the last statistic data like average consumption, amps, watts, time and so on.
```

---
## \#470 Posted by: rey8801 Posted at: 2018-04-20T14:15:39.322Z Reads: 144

```
That's good! Thx a lot. So we should see version 1.74? Correct?
```

---
## \#471 Posted by: Ackmaniac Posted at: 2018-04-20T14:16:38.108Z Reads: 142

```
Correct, Google needs a couple of hours to publish it.

And good news for everybody. Checked my bank account and saw that there is still enough space for some donations. So feel free ...
```

---
## \#472 Posted by: rey8801 Posted at: 2018-04-21T05:38:02.264Z Reads: 154

```
I am going to try the new version. I notice that in 5he modes configuration on the app we still have the option watt or current no reverse with brakes. I know that in vesc tool the current mode is watt mode but in the app what do we have to select in order to choose watt mode? Because you can also enable the use max watt in the other settings ![vescmonitor|281x500](upload://coDOkOGHUxBdHePpYL2si2dPMcj.png)
By heart I would say that current no reverse with brakes and enable use max watt should be the way to go. I started doubting when I see that in the VDLA app along the board setting the max watt value is 0.
![chrome|690x388](upload://ajIM5n2kuW38g23UXcMGdou8mM0.png)
Thxs
```

---
## \#473 Posted by: Ackmaniac Posted at: 2018-04-21T11:23:50.275Z Reads: 149

```
Thanks for the info. Released new Version 1.75 which should fix that issue.
@DeathCookies maybe you can have a look as well.
```

---
## \#474 Posted by: rey8801 Posted at: 2018-04-21T11:58:55.129Z Reads: 155

```
You are welcome. Anyhow the upgrade that the app shows the last ride even when the board is not connect works as long you don't close completely the app. Then us not possible anymore. Just ti let you know.
I also think I understand why when I set the lower speed and watt it really slow down but doesn't respect the limit. I made a video and basically the left motor spins faster  (master VESC with uart module attached) than the slave. This thing doesn't happen to me when I ride in the let's say full power mode. Here the video, I couldn't go full throttle without weight because the motors start rattling, probably because they try to overpass the watt limit.
https://www.youtube.com/watch?v=cp030j4thec
Hope it helps

Edit: Is the master connected motor that spins slower, which make sense because it is the one that send the signal to the slave. So is the slave that spins faster in the movie. Sorry for the misunderstanding.
```

---
## \#475 Posted by: rey8801 Posted at: 2018-04-21T12:10:23.602Z Reads: 143

```
Just to know the VDLA shows still no watt max
![chrome|690x388](upload://g4hk45nhc0lJE67kcgZ6qkGQc8r.png)
```

---
## \#476 Posted by: Ackmaniac Posted at: 2018-04-21T14:23:03.626Z Reads: 141

```
Try it with higher values and stand on the board. 10 watts limit is extremely tight. It's like limiting a car to 0,5  hp.
```

---
## \#477 Posted by: rey8801 Posted at: 2018-04-21T14:34:00.257Z Reads: 142

```
As I said with full power mode I do not have it. I just wanted to let you know in case you see something more. To me was not a coincident that the slave Vesc is the one that can not keep the limits in this case. Nevermind, It does slow down the board for people that wanna try it, so fine for me :grin:
Thx
```

---
## \#478 Posted by: MartyMcFly88 Posted at: 2018-04-24T13:07:14.207Z Reads: 135

```
This might be helpful for you: https://blog.yavilevich.com/2018/04/should-you-throw-away-your-cc41-hm-10-clones-now-that-android-8-is-here/
```

---
## \#479 Posted by: rey8801 Posted at: 2018-04-24T13:15:21.728Z Reads: 131

```
Form the same blog how to spot a clone https://blog.yavilevich.com/2016/12/hm-10-or-cc41-a-module-automatic-arduino-ble-module-identification/ Basically by the breakdown board and the lack of one oscillator you can discriminate between the original and clones.
It doesn't means that the clones won't work with the Ackmaniac software. I also have a clone. Original arduino is also more expensive.
```

---
## \#480 Posted by: Ackmaniac Posted at: 2018-04-24T21:54:25.827Z Reads: 127

```
Released a new version (1.76) of the app. Refactored a lot of the code in the background. So please report if you have new issues and write which version of the firmware you use.

The Dark theme was not shown correct in videos. So please give it another try now. I think it looks great now.

It can take a couple of hours before the new version is available at Google Play.
```

---
## \#481 Posted by: MartyMcFly88 Posted at: 2018-04-24T22:04:17.210Z Reads: 135

```
So your clone version works with oreo? do you happen to know which clone version you have? 

 ".. While trying to mimic the original HM-10 by “Jinan Huamao technology Co” they differ by firmware, breakout board and daughter board. When ordering online it is very difficult to know which exact combination you will get..."

and where you got it from? If yours works, I could just order that one instead of waiting for the arduino and flashing the new software. 
I would love to get Ackamiacs app working again!!
```

---
## \#482 Posted by: SeanHacker Posted at: 2018-04-24T22:04:18.214Z Reads: 129

```
Downloaded and going out for a test run now. Thanks dude!
```

---
## \#483 Posted by: Ackmaniac Posted at: 2018-04-24T22:08:10.051Z Reads: 131

```
Think the newest version isn't available yet. just have a look at the top of the app if it shows version number 1.76
```

---
## \#484 Posted by: MartyMcFly88 Posted at: 2018-04-24T22:11:19.710Z Reads: 130

```
did you have any luck? Version 1.76 is still not working for me, probably due to HM-10 Clone +Oreo :'(
```

---
## \#485 Posted by: SeanHacker Posted at: 2018-04-24T22:27:16.264Z Reads: 142

```
Lol. I made sure it was the latest. Works great too!

![Screenshot_20180424-152535|281x500](upload://6x3sjsT3yIGiVS71ynEBsaZgEZt.png)
```

---
## \#486 Posted by: SeanHacker Posted at: 2018-04-24T22:28:09.168Z Reads: 129

```
I haven't checked on my main phone. I've been having to use a different phone to use this app. Thinking I'm just going to buy some new modules as updating them seems to be more of a hassle.
```

---
## \#487 Posted by: MartyMcFly88 Posted at: 2018-04-24T22:31:43.411Z Reads: 132

```
But how would you make sure to order genuine HM-10 modules?
```

---
## \#488 Posted by: SeanHacker Posted at: 2018-04-24T22:35:40.022Z Reads: 134

```
That I haven't figured out yet.
```

---
## \#489 Posted by: MartyMcFly88 Posted at: 2018-04-24T22:36:31.935Z Reads: 136

```
:sweat_smile:
```

---
## \#490 Posted by: SeanHacker Posted at: 2018-04-24T23:07:40.576Z Reads: 137

```
Just a little test while I had a minute. I really wish I knew how to edit!!! I strapped an old phone to my helmet this time to see how it worked. Not bad. 

https://youtu.be/Bg_7t1sLwhY
```

---
## \#491 Posted by: Mikenopolis Posted at: 2018-04-24T23:11:41.745Z Reads: 141

```
@SeanHacker off topic, seeing that you are using a GT2B, can you turn off your board and remote, then turn on JUST your board and see if goes full throttle after 30 or so seconds? Mine and @danielz is having that issue
```

---
## \#492 Posted by: danielz Posted at: 2018-04-24T23:16:45.021Z Reads: 134

```
Im not anymore, i trimmed the throttle to 1500ms, so the silly gt2b receiver cant run my board into a ditch.
```

---
## \#493 Posted by: danielz Posted at: 2018-04-24T23:17:11.496Z Reads: 135

```
Helmet cam works quiet well. Might try it myself.
```

---
## \#494 Posted by: Ackmaniac Posted at: 2018-04-24T23:18:16.966Z Reads: 135

```
I see you have a lot of signal interruptions. Guess that's coming from the carbon enclosure. Maybe try to position the module outside of the enclosure. When i ride i have more or less zero interruptions.
```

---
## \#495 Posted by: SeanHacker Posted at: 2018-04-24T23:21:36.030Z Reads: 128

```
I remember a very long time ago I had that same issue. I don't have it anymore because I needed to set the failsafe. I really can't remember the process though as it was soooooo long ago.
```

---
## \#496 Posted by: danielz Posted at: 2018-04-24T23:23:15.956Z Reads: 129

```
its not a failsafe issue, the gt2b ignores the failsafe at 30 seconds after power on IF the controller isnt connected. It moves the timing to stock 1500ms. So if you failsafe isnt near 1500ms bye bye boardy. At least thats what mine does.
```

---
## \#497 Posted by: SeanHacker Posted at: 2018-04-24T23:23:40.009Z Reads: 126

```
Yeah. I've actually been testing a couple different modules lately. I think this one isn't very good because that doesn't happen on the others. Going to switch back to my old trusty tonight or tomorrow.
```

---
## \#498 Posted by: Ackmaniac Posted at: 2018-04-24T23:51:11.709Z Reads: 129

```
Just decided to modify the refresh rate because it was too fast in the videos. Was hard to read the data when it changes with every frame. So it set it down to 6 realtime data updates a second.

New version is 1.77. @SeanHacker Maybe it also results in a more reliable connection for you.
```

---
## \#499 Posted by: rey8801 Posted at: 2018-04-25T01:38:03.386Z Reads: 137

```
I didn't mean that mine clone works with oreo. It works in general. I don't have Oreo to test it. I would say that the options are update the firmware on the module as you said (actually new clone firmware should be oreo compatible) or by real hm-10 module (HM-10 Transparent Serial Port Bluetooth 4.0 Modules Bluetooth Serial Port With Logic Level Transformation
 http://s.aliexpress.com/FJBJJ3qI?fromSns=Copy to Clipboard). The lates is the only one I found it identical to the description in the blog before mentioned. Still not sure you get exactly this one. You can ask them as picture before shipping. Otherwise buy it through other channels for more.
```

---
## \#500 Posted by: rey8801 Posted at: 2018-04-25T01:57:53.298Z Reads: 131

```
I actually have version 1.78 now. I will try it later on. Thx
```

---
## \#501 Posted by: xBRAZILx Posted at: 2018-04-25T11:40:22.376Z Reads: 129

```
has anyone having problems with the 1.78 version?
i am getting all crazy negative numbers in battery/power/motor current/battery current boxes...
```

---
## \#502 Posted by: rey8801 Posted at: 2018-04-25T12:06:22.913Z Reads: 125

```
I didn't using during ride yet. But by just check it on bench the value are ok. As I said I didn't have the chance to try it on road yet. I am painting!
```

---
## \#503 Posted by: Ackmaniac Posted at: 2018-04-25T12:15:27.923Z Reads: 126

```
Which firmware version do you use?
And it would be easier to analyse if you can make a video with the app.

Edit: Found the bug, i guess you use 2.18 or 2.54.
Relased a **new Version 1.79** which should fix that problem. Thanks for the info.
```

---
## \#504 Posted by: xBRAZILx Posted at: 2018-04-25T12:45:19.592Z Reads: 135

```
you are right. using 2.18.
i´ll update, test and record as soon as update

thank YOU for this great APP
```

---
## \#505 Posted by: SeanHacker Posted at: 2018-04-25T12:50:05.729Z Reads: 138

```
Nice! I'm going to be strapping the phone to my head again tonight to test on my way home from work. Thanks dude!
```

---
## \#506 Posted by: xBRAZILx Posted at: 2018-04-25T16:57:26.202Z Reads: 147

```
had the same weird info. 
i double checked if some wire was a little loose on the vesc. but it was ok.
i made a video showing what is going on.
if you need some extra information i´ll be glad to help.
ps: later i can open the bldc in my computer and double check the terminal...


https://youtu.be/h6rveT319mA
```

---
## \#507 Posted by: Ackmaniac Posted at: 2018-04-25T17:25:03.246Z Reads: 140

```
Do you have already version 1.79?
```

---
## \#508 Posted by: xBRAZILx Posted at: 2018-04-25T17:26:48.292Z Reads: 142

```
yes, i updated before making the video.
```

---
## \#509 Posted by: Ackmaniac Posted at: 2018-04-25T17:33:05.673Z Reads: 137

```
You double checked with the version number it shows in the app? (First screen at the top left)
```

---
## \#510 Posted by: xBRAZILx Posted at: 2018-04-25T17:58:18.941Z Reads: 138

```
![Screenshot_20180425-143821 (1)|281x500](upload://uQcB7ttvF75DRQYEqRPoPrxRxBy.png)![Screenshot_20180425-113939|281x500](upload://6syEQcmP2ED680NkkmBH0OAbmWv.png)

later i´ll check the bldc terminal/real data. thanks
```

---
## \#511 Posted by: Ackmaniac Posted at: 2018-04-25T19:22:19.572Z Reads: 132

```
**New Version 1.80 available:**

Now i finally found the nasty bug. Found and fixed also another issue that could result in connection losses.
So please give it another try.
@SeanHacker Would be great if you can test this version as well with the Module from your previous video. Maybe it works now without interruptions.
```

---
## \#512 Posted by: SeanHacker Posted at: 2018-04-25T19:52:32.364Z Reads: 131

```
Definitely will. I'll have a video up in about 3-4 hours when I get off work today.
```

---
## \#513 Posted by: xBRAZILx Posted at: 2018-04-25T22:21:13.511Z Reads: 138

```
update to 1.80 and tested. here are things that i could noticed...

1)Default box isn´t showing my board´s info.

2)Motor Current is showing more than my max motor amp is set in the vesc (motor and battery is set to 45A)

3)The "POWER" is showing is a a little bit higher than i used to have. (until 1.75 i was getting 1100 watts) but now i am having something like 1700 watts. 

4) the header's boxes was painted with green / red according speed up / speed down. now only duty has color in the header

ps: youtube delete my video for some weird reason... so i put the .mp4 file in mailbigfile

link to download the video (sorry for the inconvenient)
https://free.mailbigfile.com/01742a8ebdc18fc931fabff107e11954/listFiles.php

do you have the 1.73 apk version, just to test and compare?
thanks
```

---
## \#514 Posted by: Ackmaniac Posted at: 2018-04-25T23:38:25.274Z Reads: 141

```
Just released a new version 1.81 to improve stability.

I have 2 different brands of modules and one is working totally reliable and the other one is more sensitive and can loose the connection which seems to result in a a software exeption on the module iself. After a power cycle it works fine again. So i tried to improve the stability by forcing a break for a couple of ms after each message. Seems to make it better but not perfect yet.

@xBRAZILx If you have a dual drive and told the app that you have 2 motors then the motor, battery, power and average consumption values will be doubled. So when you set 80A max then you could reach 160A.
```

---
## \#515 Posted by: SeanHacker Posted at: 2018-04-25T23:42:22.837Z Reads: 135

```
Being as tired as I am I totally forgot to update the app to test on my way home. Going to wait for the newest update (I usually get app updates quick) and then I'll go for a test ride. Thanks again!
```

---
## \#516 Posted by: Chris604 Posted at: 2018-04-26T00:22:38.541Z Reads: 132

```
My raptor 2 is showing red on the power section and %588 volts what does that mean? How Can I get it To read out a proper persentage? I have it set to custom 400wh and 10 cells. Everything else is default. @Ackmaniac
```

---
## \#517 Posted by: xBRAZILx Posted at: 2018-04-26T01:07:52.412Z Reads: 138

```
just get the 1.81 version and we are back to the business.:sunglasses: 

funny you mentioned about the "No of Motors (Vesc)" because i double checked and for some stranger reason was set 2. i have a single drive and i didn´t change this. (i guess haha) The "Save GPS position" parameter was unchecked and i always leave checked this option. about other issues:

1)my board info is back; 

2)the green/red header is back. 

3)about motor/battery amps and motor watts i havent tried riding yet, but tomorrow morning i´ll and i think was something related with "No of Motors (Vesc)" like you mentioned

thanks for the app update

edit: i also update to 1.82
```

---
## \#518 Posted by: EssEnn Posted at: 2018-04-26T20:34:25.242Z Reads: 123

```
Everything works great for me other than GPS does not seem to be working. Anyone else have the same issue?
```

---
## \#519 Posted by: Mathias Posted at: 2018-04-26T21:15:11.034Z Reads: 126

```
I have version 1.82 and FW 3.37 (stock) with HM-10 and Android 7. The app says it's connected but there is no readout. All numbers are 0. 
I haven't used it since the weekend and apparently there were many updates recently so I can't really tell with which update it stopped working. 
Does anyone else have this problem?
```

---
## \#520 Posted by: Ackmaniac Posted at: 2018-04-26T21:19:47.507Z Reads: 128

```
Did you try to restart the app a couple of times to see if it helps?
```

---
## \#521 Posted by: Mathias Posted at: 2018-04-26T21:22:44.514Z Reads: 129

```
Yes. Really killing it and starting again a few times. Also just waiting for a minute or so while it's connected. Sometimes it just takes a while until the values are read out. 
But I'm not at home now and will do some more testing tonight.
```

---
## \#523 Posted by: Ackmaniac Posted at: 2018-04-26T21:29:26.034Z Reads: 124

```
So it works sometimes?
```

---
## \#524 Posted by: Mathias Posted at: 2018-04-26T21:31:12.296Z Reads: 128

```
Since the last updates it hasn't. Last time it worked was on Saturday, I think. But as I said, I can't recall which version I had then.
```

---
## \#525 Posted by: Ackmaniac Posted at: 2018-04-26T21:33:53.779Z Reads: 130

```
Please switch off the board as well when you restart the app so that the bluetooth module get's restarted. Have one type of modules that has issues and only works after i switched the power off and on again.
```

---
## \#526 Posted by: Mathias Posted at: 2018-04-26T21:36:18.982Z Reads: 129

```
OK, thanks for the advice! I restarted the board a few times, but as I said: I'll do some more testing tonight.
```

---
## \#527 Posted by: SpartanFrench Posted at: 2018-04-26T21:57:25.340Z Reads: 134

```
:+1::+1::+1: @Ackmaniac :+1::+1::+1: 
Just awesome, thank you for your app
```

---
## \#528 Posted by: maker7 Posted at: 2018-04-27T02:11:14.136Z Reads: 131

```
Love this app!  The only problem I have is the video is upside down.  I have a Nexus 5x.  Anyone else have this issue?
```

---
## \#529 Posted by: Ackmaniac Posted at: 2018-04-27T06:23:04.290Z Reads: 137

```
Go in the video settings of the app and select the layout "left and right".
```

---
## \#530 Posted by: MartyMcFly88 Posted at: 2018-04-27T10:26:53.953Z Reads: 133

```
@ackmaniac do you think it might be possible to explain about the hm10clone-oreo trouble in the description of your app at the Start of this thread? This Problem will not resolve itself and there will only be more oreo users as time goes by.. Once we know a source for genuine hm10 Modules you could link those.. But as of now if a new user tries this with oreo it will not work!
```

---
## \#531 Posted by: rey8801 Posted at: 2018-04-27T11:45:48.621Z Reads: 129

```
Based on the blog I linked here https://www.electric-skateboard.builders/t/vesc-monitor-android-app/20888/479?u=rey8801. On Ali I found this HM-10 that seems to be original. HM-10 Transparent Serial Port Bluetooth 4.0 Modules Bluetooth Serial Port With Logic Level Transformation
 http://s.aliexpress.com/FJBJJ3qI?fromSns=Copy to Clipboard more expensive then the clones but still rather cheap. You can always ask to the seller ci formation that you are going to get the ordinal one and not a copy.
```

---
## \#532 Posted by: MartyMcFly88 Posted at: 2018-04-27T12:36:35.264Z Reads: 128

```
I just ordered this one: [HM-10 Aliexpress](https://www.aliexpress.com/item/Free-shipping-HM-10-transparent-serial-bluetooth-4-0-bluetooth-serial-port-module-with-logic-level/32276092839.html?spm=2114.search0104.3.1.52dd7f02PS0G4Q&ws_ab_test=searchweb0_0,searchweb201602_3_10320_10152_10321_10065_10709_10151_5722917_10344_10068_10342_10547_10343_5722817_10322_10340_10341_10548_5722617_10697_10193_10696_10194_10084_10083_10618_10304_10307_10710_10302_5722717_10180_10059_5711217_10184_308_100031_10319_10103_441_10624_5722517_10623_10622_10186_10621_10620_5711317,searchweb201603_36,ppcSwitch_4&algo_expid=93ccc62f-fce8-47fc-a019-75a2728fe4aa-0&algo_pvid=93ccc62f-fce8-47fc-a019-75a2728fe4aa&priceBeautifyAB=0)
It is sold by the "keyestudio Official Store" so it seems to be legit .. I will let you now if it works with oreo once it arrives ..
```

---
## \#533 Posted by: rey8801 Posted at: 2018-04-27T13:35:14.899Z Reads: 131

```
The breakout board brand seems the same with different design. I hope it's good one.
```

---
## \#534 Posted by: SpartanFrench Posted at: 2018-04-27T15:18:46.124Z Reads: 141

```
@Ackmaniac, 3 question 

1. Is there a way to customize notifications receive on my android watch  from your apps? I only see battery % but i would also like to see speed .

2. Do you know why my temperature box is red even if temp is at 30 degree ?

3. Why the apps freeze when I push my home button and try come back to the apps ?
```

---
## \#535 Posted by: maker7 Posted at: 2018-04-27T16:48:26.038Z Reads: 145

```
Thanks for the quick reply.  Unfortunately it still does not work.  I think I found out why.  Apparently, the sensor is mounted in the phone upside down from the factory for space considerations....  Here is the article, if you are interested:

https://www.gottabemobile.com/how-to-fix-nexus-5x-upside-down-photos/

Thanks again,  Love the app still.

Paul
```

---
## \#536 Posted by: asken92 Posted at: 2018-04-28T10:42:08.318Z Reads: 134

```
awsome app @Ackmaniac  !! I have some problems though. since it was the fastest i bought a bluetooth HC-06 locally since i didnt want to wait for like a month for a hm-10 module. But i cannot connect to it, actually i dont really know if the app detects it at all. My phone's bluetooth detection shows HC-06. I guess my questions is does this work with HC-06 module with 9600 baudrate? or do i need to get a HM-10 module. Thanks in advance 

Niklas
```

---
## \#537 Posted by: Ackmaniac Posted at: 2018-04-28T11:30:47.847Z Reads: 129

```
You need to get a hm-10
```

---
## \#538 Posted by: asken92 Posted at: 2018-04-28T11:54:32.643Z Reads: 127

```
Alright, as i thought :) thanks for the fast answer !
```

---
## \#539 Posted by: Nexo Posted at: 2018-04-28T19:31:13.102Z Reads: 143

```
![31461011_1581437145236996_8084333365492187136_n|281x500](upload://9QbtetUzBjHsgYxMuJIdTCk90W5.jpg)

I took a quick ride today, but I can not get few things from app.

max km/h: 41,9? I don't think that I was going so fast... what can cause that misscalculation? :stuck_out_tongue: (wheels set to 230mm, gearing 8/48)
 
range: hard to believe it :face_with_raised_eyebrow: battery was loaded to 93%, I did 8,38km (12s cells, 25Ah)

Any suggestions?

![31402773_1581475828566461_5922014213257035776_n|281x500](upload://1YTJz6hF5C6xJREHhniFpwYUXhB.jpg)
![31402806_1581475818566462_7274358866257641472_n|281x500](upload://fqheiCxP00yq1MUZYbYrsfQpSH6.jpg)
![31487799_1581475791899798_1602428607097995264_n|281x500](upload://kAei1GX6ZcJK4D6EOMc3TcaFqZq.jpg)
```

---
## \#540 Posted by: Ackmaniac Posted at: 2018-04-28T19:58:59.532Z Reads: 137

```
Guess you lifted the baord once and let them spin at full speed for a short time. That is neough to reach max speed for the app. It takes the wheels speed and not gps for max speed.

And at a average consumption of 17.520 Wh / km you can get max of 63.3 km. And 76% of that is around 48.1 km. And that would mean you need to drain the battery totally.

In reality you won't even get that far with that consumption because you have losses here and there. And you would need to empty the battery completely. So i recommend to set only 85% of your theoretical Wh. So in your case 1110 * 0.85 = 944 Wh which would give you a range of around 40 km with 76 % battery left like in the picture.

And you have 9 inch tyres and a 8/48 ratio. Very unusual, can you give some more details.

And you battery settings are for sure not realistic. For your E-Golf batterys i don't know exactly but i would recommend Li-Ion values:
100% - 4.2
90% - 4.07
80% - 4.02
70% - 3.94
60% - 3.86
50% - 3.79
40% - 3.715
30% - 3.635
20% - 3.525
10% - 3.435
0% - 3.26
```

---
## \#541 Posted by: Nexo Posted at: 2018-04-28T20:22:28.548Z Reads: 132

```
[quote="Ackmaniac, post:540, topic:20888"]
And you have 9 inch tyres and a 8/48 ratio. Very unusual, can you give some more details.
[/quote]

chain drivetrain, 8 teeth on motor, 49 on wheel, 05b-1 chain

[quote="Ackmaniac, post:540, topic:20888"]
but i would recommend Li-Ion values:

100% - 4.2
[/quote]
I don't know why, but my charger is reaching only 4.1V, can I load it with lipo profile so it will be loaded to 4.2V?

BTW, thank you for answer :smiley:  having that BT connection is kinda new for me, but very exciting at the same time and your app is a king :smiley:
```

---
## \#542 Posted by: Ackmaniac Posted at: 2018-04-28T20:44:34.697Z Reads: 131

```
[quote="Nexo, post:541, topic:20888"]
I don’t know why, but my charger is reaching only 4.1V, can I load it with lipo profile so it will be loaded to 4.2V?
[/quote]

I have no idea. Google is your friend. But i don't know a Li-Ion cell that should be charged to 4.1V max.
```

---
## \#543 Posted by: Ackmaniac Posted at: 2018-04-28T20:50:24.731Z Reads: 133

```
just released a new version 1.84.

Status Bar notofications now also have the speed as value. And it is possible to activate "Fast status notifications" in the settings so that each data update is also forwarded to the notifications. This should help that the you can see the actual speed on your smartwatch. I don't have one so it would be great if you can give it a try and report if it works.

And the Board Info screen now shows the values for both motors together. Before it was only for one motor. So maybe it's good to reset the value by doing a long click in the board info screen. Or at least you can reset one of the trip meters.
```

---
## \#544 Posted by: guilhem74 Posted at: 2018-04-28T21:59:04.104Z Reads: 130

```
Your apps look incredible but I have an issue.
I am using an HC-05 and i'm able to connect to the vesc with the BLDC tool on my PC through bluetooth.
It is connected on my Master vesc with PPM+UART mode. (Uart in 9600bps)
When I try to use your app I can't find my module in the list of device. I can find anything else but not it. (And it is not paired with something else)
Any idea why ?
Thanks
```

---
## \#545 Posted by: Ackmaniac Posted at: 2018-04-28T22:03:36.714Z Reads: 135

```
Because the app needs a Bluetooth Low Energy connection. And the HC-05 is for standard Bluetooth which the app doesn't support.
```

---
## \#546 Posted by: guilhem74 Posted at: 2018-04-28T22:08:39.244Z Reads: 133

```
Crap, I can't find any application which work with that module.
Thanks for the answer.
Would you share the code than I could adapt it ? (Couldn't find it on your github :slight_smile: )
```

---
## \#547 Posted by: Ackmaniac Posted at: 2018-04-28T22:45:07.372Z Reads: 127

```
It's not open source.
```

---
## \#548 Posted by: Fiori Posted at: 2018-04-28T23:01:31.813Z Reads: 130

```
@Ackmaniac Iv'e been using your app for the past week and it's awesome. Thanks for all the hard work.
```

---
## \#549 Posted by: guilhem74 Posted at: 2018-04-28T23:15:06.716Z Reads: 133

```
OKay, thanks anyway.
I will buy an HM-10 to use your fantastic work
```

---
## \#550 Posted by: Sebike Posted at: 2018-04-28T23:20:08.212Z Reads: 132

```
Updated to latest version (from 1.80) and app shuts down as soon as I try to connect to the BT-module. 

Worked fine on previous versions.
(Running off a Sony Xperia z3)
```

---
## \#551 Posted by: Ackmaniac Posted at: 2018-04-28T23:38:25.763Z Reads: 134

```
Seems i made a mistake somewhere. I just released a new version 1.85 which hopefully fixes the issue.
If not then i need to have a look tomorrow.
```

---
## \#552 Posted by: SpartanFrench Posted at: 2018-04-29T03:32:52.126Z Reads: 135

```
I will update the apps and test with my smartwatch. I will keep you posted.
```

---
## \#553 Posted by: Sebike Posted at: 2018-04-29T13:22:11.966Z Reads: 133

```
The issue remains. As mentioned, last version that was working for me was 1.80. 

Never tried the 81 to 83.
```

---
## \#554 Posted by: SpartanFrench Posted at: 2018-04-29T13:33:37.365Z Reads: 137

```
@Ackmaniac V 1.85 crash as soon as I click on my bluetooth module  to access my board main panel
```

---
## \#555 Posted by: Ackmaniac Posted at: 2018-04-29T13:36:12.829Z Reads: 152

```
Will fix the issue today. Currently no access to a board
```

---
## \#556 Posted by: Ackmaniac Posted at: 2018-04-29T16:52:43.636Z Reads: 151

```
Issue is fixed in new Version 1.87. 

Also updated the notifications. they look like this now
![image|201x40](upload://e1eyPfCPvsua2XFMCXs1NqKbbqE.png)
Speed on top
then battery%, battery voltage, distance and range

Hope they look good on the smartwatch
```

---
## \#557 Posted by: gaetjen Posted at: 2018-04-29T17:14:52.217Z Reads: 150

```
Version 1.86 caused the app to crash. Previous versions all worked fine.
```

---
## \#558 Posted by: gaetjen Posted at: 2018-04-29T18:08:29.321Z Reads: 148

```
Problem seems to be fixed with the new version
```

---
## \#559 Posted by: SpartanFrench Posted at: 2018-04-29T18:39:26.866Z Reads: 149

```
**V 1.87** : I can confirm there is no more crash from logging to my board.

**Smartwatch notification** : Being able to see speed is awesome ! 
However, on my side Speed is updated only every 5 or 10 sec. 
It might be my watch* but It would be awesome to get real time data

*Note : I'm using a Polar V800 and notification are push to my watch through a 3rd party app.
```

---
## \#560 Posted by: Ackmaniac Posted at: 2018-04-29T18:45:09.168Z Reads: 143

```
Just have a look in the settings. There is a checkbox "Fast status notifications". Just activate it and enjoy.

And please make a picture of it so that I know how it looks.
```

---
## \#561 Posted by: SpartanFrench Posted at: 2018-04-29T19:27:19.516Z Reads: 146

```
Perfect, I will test hit during my next ride and will upload photos of my screen.

**Landscape mode** : @Ackmaniac: how difficult it would be for you to make the app orientation responsive depending of phone inclinaison or just with a button in settings ? (portrait and landscape) It could be a nice feature to have in the next version.
```

---
## \#562 Posted by: SeanHacker Posted at: 2018-04-29T19:30:21.687Z Reads: 140

```
Going out now to see if I can test before the rain hits. Thanks for all the fast updates dude! You're a beast!!!
```

---
## \#563 Posted by: Ackmaniac Posted at: 2018-04-29T19:48:45.628Z Reads: 139

```
Hope your dog is doing well.
```

---
## \#564 Posted by: Sebike Posted at: 2018-04-29T20:00:12.967Z Reads: 143

```
No crashes! And a lot easier to switch between modules now, as one doesn't have to disconnect BT on the phone to reconnect to a previously connected module.. Does it make sense? Anyways, seems to work a lot better.

:+1:t3:
```

---
## \#565 Posted by: SeanHacker Posted at: 2018-04-29T20:49:50.586Z Reads: 145

```
Thanks dude. From what we've heard she's doing better now and we might be able to get her back tomorrow if she doesn't require surgery. 

I know I said I'd test the app but my emotions are getting the best of me at the moment and I'm pissed. The app works great as usual. You are a beast with these updates!!!
```

---
## \#566 Posted by: SpartanFrench Posted at: 2018-05-01T04:07:52.187Z Reads: 139

```
@Ackmaniac, here is what happen on my watch when I turn on the _"Fast status notifications”_
My watch is vibrating and beeping non stop.

https://youtu.be/LfaYvw2pB3A
```

---
## \#567 Posted by: SuperBen Posted at: 2018-05-01T23:29:01.158Z Reads: 141

```
@Ackmaniac Hey man I ran motor detection via usb for FOC and can now easily switch between FOC and BLDC via your app. Super cool feature!

But now having done that and switched back a couple times I can no longer connect to the vescs via USB. Is this related to the app? I can still control both vescs via remote, still view stats in VESC Monitor, and still switch between motor types if I want to. I have tried multiple cords on two different PCs, including two confirmed working cables on the same ports of two confirmed working PCs that I had previously used to program the vescs.

Both PCs are windows 10, were able to connect before, but when I power on the vescs windows does not notice anything had been plugged in. Any Ideas?
```

---
## \#568 Posted by: Ackmaniac Posted at: 2018-05-01T23:51:09.276Z Reads: 136

```
Hope you switched only when the motor was not moving. I did it many times and it works the same as switching in the tool. If you did while riding there might be the chance something is in the wrong state during the switch. But it also  another problem which is most likely. Just check the USB connector properly  if it is physically OK.
```

---
## \#569 Posted by: Ackmaniac Posted at: 2018-05-01T23:52:25.294Z Reads: 137

```
Would say that this is then a issue of your smartwatch which can't process that many updates in such a short time.
```

---
## \#570 Posted by: SuperBen Posted at: 2018-05-02T00:41:13.246Z Reads: 139

```
Yeah its strange, it's possible the USB port is damaged I guess, because it still functions normally otherwise. I just switched it and saved as default from the app again right now without issue, but I've tried at least 7 different USB cables and none connect.
```

---
## \#571 Posted by: Jaeson Posted at: 2018-05-02T16:44:42.853Z Reads: 135

```
@Ackmaniac Hey I have an HM10 module that connects to my iPhone just fine and sends info to my “eSkate Vesc app” without any issues. But when I try to open the Android app on my chrome book or tablet, the app won’t find the Bluetooth connection. The devices show “BT05” but the app won’t find it. What am I doing wrong or what do I need to do to make the app work?
```

---
## \#572 Posted by: Ackmaniac Posted at: 2018-05-03T17:48:28.081Z Reads: 132

```
Just released a new version 1.92 which hopefully makes the app more stable when in the background.
```

---
## \#573 Posted by: louwii Posted at: 2018-05-04T02:26:15.315Z Reads: 128

```
On your phone, make sure the localization is enabled.
```

---
## \#574 Posted by: Sebike Posted at: 2018-05-04T21:03:30.378Z Reads: 127

```
Back to the app reading 0 för GPS speed. Was working with the latest app version in early January. 

Now running 1.92 and no GPS speed. Save GPS position enabled.
```

---
## \#575 Posted by: Ackmaniac Posted at: 2018-05-04T21:04:23.331Z Reads: 143

```
I your GPS switched on at the phone?
```

---
## \#576 Posted by: Sebike Posted at: 2018-05-04T21:06:09.908Z Reads: 139

```
Sure. Without that the app won't find the BT modules.
```

---
## \#577 Posted by: Ackmaniac Posted at: 2018-05-04T21:25:15.025Z Reads: 134

```
Just didn't change anything in the GPS speed integration. At least not that i am aware of.
```

---
## \#578 Posted by: Sebike Posted at: 2018-05-04T21:28:08.351Z Reads: 135

```
oh ok, that's weird. Never got the GPS speed to work on my phone before, and then when I tested again in early January it was actually working. 

Tried it again several times this last week, but it reads 0 again.

I am getting GPS speed reads when using other apps though.
```

---
## \#579 Posted by: Ackmaniac Posted at: 2018-05-04T21:29:47.268Z Reads: 133

```
does it work with other apps? And stupid question. Are you sure you have a working connection? Means not testing inside or in area with too many buildings?
```

---
## \#580 Posted by: Sebike Posted at: 2018-05-04T21:31:09.159Z Reads: 139

```
Yes. Works with other apps. Tested in areas with virtually no buildings.. (outside lol)
```

---
## \#581 Posted by: Ackmaniac Posted at: 2018-05-04T21:58:58.523Z Reads: 144

```
Released Version 1.93 which is a try to fix the GPS issues. Please let me know if it helped?
```

---
## \#582 Posted by: Sebike Posted at: 2018-05-04T22:01:18.050Z Reads: 142

```
Thanks. I'll get back to you as soon as I have tested with this version. :+1:t3:
```

---
## \#583 Posted by: ducktaperules Posted at: 2018-05-05T09:46:57.425Z Reads: 145

```
i love the app @Ackmaniac but i have 1 question.

Im using the newest vesc tool firmware 3.36 or 3.38 i think. Can i use the "modes" in the app or are these only avalable if im running your firmware as well?
```

---
## \#584 Posted by: Sebike Posted at: 2018-05-05T10:16:45.970Z Reads: 141

```
Now working 👌👍
```

---
## \#585 Posted by: Sebike Posted at: 2018-05-06T18:22:44.754Z Reads: 138

```
Not a biggie.. But the voltage read in the app (as well as in the vesc tool) is off by about 0,80 volts in my build. 

Would it be possible to put in the diff somewhere so that the app shows the real voltage or is this a bad idea?
```

---
## \#586 Posted by: Ackmaniac Posted at: 2018-05-06T18:25:28.178Z Reads: 135

```
Would be possible. But of course the vesc has its own cutoff settings which wouldn't take care about this offset. And wouldn't it be better to know the voltage that the vesc thinks is real?
```

---
## \#587 Posted by: Sebike Posted at: 2018-05-06T18:33:51.333Z Reads: 136

```
Sure. Those that calibrate this value would be aware of how far off the value that vesc believes is real is though. But, as I said, it's not a biggie. 

I've adjusted the percentage levels in the app, as full battery read ~90-sthing-percent, so the percentage reads are already pretty accurate.
```

---
## \#588 Posted by: The_Dude Posted at: 2018-05-07T11:10:29.864Z Reads: 135

```
Hi @Ackmaniac ,
just made an update to V1.93 on my phone - wanted the dark theme. The temporal actual values on the screen seem to be ok, also the integrated values like distance, but the data displayed from the csv recording is not. 
On the VESC4.12 I'm using there is probably not the most current firmware. Do I also have to update the firmware to get the csv-data right or am I supposed to to something different in addition? Thanks,
Dude
```

---
## \#589 Posted by: Ackmaniac Posted at: 2018-05-07T13:50:37.945Z Reads: 137

```
What do you mean by not ok? It's missing or wrong? Currently fixing a issue with the data logging when the app runs in the background or when the screen is switched off. But if the app is in the foreground it should work.
```

---
## \#590 Posted by: The_Dude Posted at: 2018-05-07T14:07:12.119Z Reads: 136

```
"Not ok" means that all values are constantly 0 beside 2 or 3 spikes, except temperature and voltage (they seem to be ok). I started the app and then put the phone in my pocket ... so the app was running in the foreground, probably the screen switched off after some time. But the recorded values look this way right from the start. Will try with the screen visible in my hand in the evening. Thanks!
```

---
## \#591 Posted by: Ackmaniac Posted at: 2018-05-07T14:15:24.678Z Reads: 136

```
Seems that each Android Version has it's own way of handling apps in the background.
Expecially Samsung Galaxy devices seems to work different.

Just released version 1.94 which hopefully fixes that problem, so please give it a try.
```

---
## \#592 Posted by: Battosaii Posted at: 2018-05-07T14:25:24.055Z Reads: 133

```
Wish this app would work with my Samsung gear s3
```

---
## \#593 Posted by: Ackmaniac Posted at: 2018-05-07T14:54:53.084Z Reads: 134

```
You should be able to see notifications with a smartwatch. If not then maybe somebody else can help who got it working already.
```

---
## \#594 Posted by: Battosaii Posted at: 2018-05-07T14:57:52.261Z Reads: 137

```
Unfortunately the Samsung Gear watches do not use google smartwatch os they use a Samsung OS called Tizen and it won't show notifications from this app.
```

---
## \#595 Posted by: Ackmaniac Posted at: 2018-05-07T15:01:23.806Z Reads: 142

```
@SpartanFrench maybe you can help. You said you got it working via 3rd party app.
```

---
## \#596 Posted by: The_Dude Posted at: 2018-05-07T16:46:14.512Z Reads: 132

```
True, true. Just tested 1.94 - as soon as the screen switches off, the data records are 0. What I also mentioned (maybe it helps) is, that there is no new folder generated like before, and the csv-file is put in the apps root directory ...
```

---
## \#597 Posted by: Ackmaniac Posted at: 2018-05-07T19:16:01.783Z Reads: 131

```
Well i am a bit out of ideas. On my device it works without any issues. Even for hours. 
The file will be put in a folder which has the new name when the file is finished. So it happens when you close the realtime screen or when you manually disconnect to the device. Then the file should be available. 
But it only happens once the motor moved at least for one time. So the app doesn't record all the data when you switch on your board. Only when you moved it will start to record.
```

---
## \#598 Posted by: The_Dude Posted at: 2018-05-07T19:49:25.314Z Reads: 133

```
I will try to describe what I'm doing. Using Android Version is 6.0 on my LG Spirit 4G. Please tell me, if I can provide you with some additional information. The version of the app I used before worked without this issue - I think it was the first version where you implemented the dark scheme.

I connect the device and start pulling the trigger with the screen on. The realtime screen displays the correct data. After some seconds I turn off the display (still connected). After some additional seconds I disconnect the device.
The csv file is access able in all cases (sorry, right now I discovered that the new file went also in the timestamp-directory, but with some delay to be seen on my LG phone). In the cvs file, the values except temperature and voltage drop down to zero at the moment I turned off the screen.
```

---
## \#599 Posted by: Ackmaniac Posted at: 2018-05-07T19:59:19.172Z Reads: 125

```
Just send me a csv file via skype. Maybe i find something helpful. have already a idea what can cause it but need a file to find out if that's the case.

And are you sure you removed the app from the "Battery optimisation" apps in the Android settings?
```

---
## \#600 Posted by: The_Dude Posted at: 2018-05-08T05:39:10.824Z Reads: 125

```
Thanks for the hint Nico. I send you an PM with the link to the dropbox csv-files.

Edit: finally found the option ... "Akku-Optimierung wird ignoriert" is selected for your app, so this should not be the reason.
```

---
## \#601 Posted by: Giga Posted at: 2018-05-08T17:17:24.442Z Reads: 135

```
[quote="Ackmaniac, post:385, topic:20888"]
The app will work with 115200 as well.
[/quote]

I got 3 different "HM-10" (some are clones). They all work at 9600Bauds (VESC and Module) then I connected one to PC and changed Bauds to 115200 (AT+BAUD4, Answer: OK+Set:4 ). Then I reconnect with  115200 Bauds to PC to verify and test (AT, Answer: OK). Now I connect to VESC via USB and set UART to 115200 Bauds (yes I did press write config, 9600Bauds module stops working as well) and connect the modified module to VESC (just swap for the other one). But now the app doesn't work anymore (gets connected but doesn't display anything) :confused:

Did I miss something? 
Do I have to change something in the APP?
```

---
## \#602 Posted by: Ackmaniac Posted at: 2018-05-08T18:57:42.330Z Reads: 131

```
The app doesn't care about the Bluetooth module serial connection with the vesc.
```

---
## \#603 Posted by: Giga Posted at: 2018-05-08T20:46:46.954Z Reads: 139

```
Ok, but where is my mistake?
I am using the UART port at 115200 Bauds for an arduino remote, but I think it is handy to swap cables (maybe even via switch) and use my phone to tune settings.
```

---
## \#604 Posted by: Ackmaniac Posted at: 2018-05-08T22:00:39.041Z Reads: 137

```
Maybe the module doesn't wok reliable at this speed. Issue with low energy is that a package can be at maximum 20 bytes long. So if the message is longer it is splitted in multiple packages. At this baud rate this split might happen too fast for the module. Maybe for the app as well. But i heard that people used the app already with 115200. Maybe somebody can confirm.
```

---
## \#605 Posted by: MartyMcFly88 Posted at: 2018-05-09T17:48:05.614Z Reads: 142

```
I can confirm that the Module i linked above works with android oreo! :) :) awesome to have this great app working again! @Ackmaniac this module is shown as "HMSoft". Is there a way to transfere the stats from my previous rides to the "new" Board?
```

---
## \#606 Posted by: Theos Posted at: 2018-05-15T12:01:47.272Z Reads: 139

```
Hi @Ackmaniac, 

I have  application freeze since the last build of your app,
everything worked perfectly on the build of 08 april with the "oreo gps fix"

can you help me ? you need a log ?
have you a mirror of the previous build ?  ( edit-> i have found à mirror 1.73 to 1.94 i will test...)

Thank for your help :)


edit2 --> @Ackmaniac , No freeze with V1.88, the problem is between v1.88 and V1.94, have you make a fix with 1.95 ?
```

---
## \#607 Posted by: Ackmaniac Posted at: 2018-05-16T23:15:13.071Z Reads: 139

```
I released a new Version 1.95 of the app.

I added the feature to define a single cell voltage at which a warn sound should be played the the desired charge voltage is reached.

You can define a voltage between 3.80V and 4.25V. The warn sound will be played 3 times with a delay of 15 seconds.

This way you can be warned if you only have a simple charger and want to charge your battery to like 4.10V to safe battery cycles.

You can activate the warings by clicking on the Volt Box where the actual battery percent and voltage is visible.
A popup screen will appear which lets you choose the desired single cell charge voltage.

Each time you want to be warned you have to activate it again. So you will only hear the sound when you want it.
```

---
## \#608 Posted by: Maxid Posted at: 2018-05-17T03:59:43.821Z Reads: 135

```
Wouldn't this eliminate the crucial constant voltage phase of the charging? I doubt it is a good idea to just stop a charging process once you hit a voltage threshold. The pack has not balanced at this point and might have drifting cells. Could get worse and worse each time you charge this way.
```

---
## \#609 Posted by: 91stantheman Posted at: 2018-05-17T14:27:25.262Z Reads: 134

```
You could just do a full charge every 3 or so charges. Realistically tho a quality pack that isn't starting to crap out will stay relatively balanced through quite a few cycles, at least in my experience.
```

---
## \#610 Posted by: mmaner Posted at: 2018-05-17T14:30:58.001Z Reads: 132

```
I think this is for people that are running a BMS-ess battery pack, that balance charge the pack manually. Also, charging  to 90 % will more than double the lifetime of a lithium ion battery pack.
```

---
## \#611 Posted by: MartyMcFly88 Posted at: 2018-05-17T18:19:10.033Z Reads: 130

```
Wouldn't this mean you leave the vesc connected during the charging of the battery? I thought it was adviced to avoid this..?
```

---
## \#612 Posted by: mmaner Posted at: 2018-05-17T18:19:58.574Z Reads: 130

```
I always have, most BMS's even require that the pack be on to charge...
```

---
## \#613 Posted by: Ackmaniac Posted at: 2018-05-17T18:38:44.649Z Reads: 131

```
The Vesc doesn't care if it is on during charging or not.
```

---
## \#614 Posted by: The_Dude Posted at: 2018-05-22T08:27:00.837Z Reads: 138

```
Hi Nicomaniack,

if you don't mind I have a feature request for the camera recording. Would be great if I can switch between front and rear camera of my phone while recording a video in your app or just choose from the beginning. 
In "normal" camera mode of the phone I do this by just wiping over the screen. Seems that this option is not valid in video recording mode of your app? Is it possible to enable this feature or is there a workaround for me?

As always, thanks for your excellent work :star_struck:.
```

---
## \#615 Posted by: Ackmaniac Posted at: 2018-05-23T20:37:57.912Z Reads: 145

```
My girlfriend bought a Google Pixel 2 so that i am able to test Android 8.0 and above. I have different Bluetooth modules and these in the link below seem to work. Did not buy it from there but they look 100% the same as the ones i have in hand.

https://de.aliexpress.com/item/HM-10-transparent-serial-bluetooth-4-0-bluetooth-serial-port-module-with-logic-level-transformation/32238168582.html?spm=a2g0x.search0104.3.226.7211358b8UYaTW&ws_ab_test=searchweb0_0,searchweb201602_5_10320_10152_10321_10065_10151_10344_10068_5722815_10342_10547_10343_10322_10340_10341_10548_5722915_10193_5722615_10194_10696_10084_10083_10618_10304_10307_10302_5722715_5711215_10059_308_100031_10319_10103_10624_10623_10622_5711315_5722515_10621_10620_10814_10815,searchweb201603_19,ppcSwitch_5&algo_expid=a7986537-3842-4a77-8c51-0ba6bcf86536-32&algo_pvid=a7986537-3842-4a77-8c51-0ba6bcf86536&transAbTest=ae803_1&priceBeautifyAB=0

Maybe all modules with the black back work. Maybe not.
```

---
## \#616 Posted by: rok Posted at: 2018-05-24T05:45:25.878Z Reads: 137

```
Hey i have a little problem with riding modes. I set my default mode on bldc tool with normal values for my setup and it works great. But as i was about to add a different mode through your app, in this case "POLICE" mode, the wheel and therefore the motor spins in the opposite direction. So the board goes backwards istead forward like in default mode. I'll leave the screenshot of my settings here.
![Screenshot_20180523-160925_ESC Monitor|243x500](upload://g1dFLD7fpqBHLSkar4STjcrIOPR.jpg)
```

---
## \#617 Posted by: Ackmaniac Posted at: 2018-05-24T05:49:25.338Z Reads: 132

```
I guess you use your remote in the wrong direction. Which one do you have?
```

---
## \#618 Posted by: rok Posted at: 2018-05-24T05:50:45.436Z Reads: 137

```
Benchwheel, and no, i dont use my remote in the wrong direction :joy:
I push the throttle  forward to go forward.
```

---
## \#619 Posted by: Ackmaniac Posted at: 2018-05-24T05:52:31.795Z Reads: 134

```
Can you change direction of the throttle commands in the remote? If yes then do that and change motor direction in the vesc settings. And yes, your using it in the wrong direction. For the vesc you go backwards when you press forward at the moment.
```

---
## \#620 Posted by: rok Posted at: 2018-05-24T06:03:16.725Z Reads: 136

```
I don't have that button to change the direction on my remote.
I set my defoult values on your bldc tool so why does it work on defoult and not when i set it through the app.
Either way, even if i set it up as current with reverse, it doesn't matter which direction i push the throttle it will always go backwards. So pushing forward, the board goes backwards, pushing backwards, the board is still going backwards.
```

---
## \#621 Posted by: rok Posted at: 2018-05-24T06:04:27.689Z Reads: 136

```
[quote="Ackmaniac, post:619, topic:20888"]
For the vesc you go backwards when you press forward at the moment.
[/quote]

And who the f**k said OK to this?
```

---
## \#622 Posted by: Slak Posted at: 2018-05-24T13:52:54.558Z Reads: 134

```
Different speeds for the wheels can occur on the bench but not when weighted. Test in ride !
```

---
## \#623 Posted by: rey8801 Posted at: 2018-05-24T13:54:23.416Z Reads: 142

```
I was testing it while I was riding. Anyhow I solved. I had to figure it out the exact number of the motor poles.
```

---
## \#624 Posted by: piepolitb Posted at: 2018-05-24T13:54:53.113Z Reads: 148

```
Hi @Ackmaniac, I just wired up the HM-10 and installed your App. I'm running Android 7 on my cellphone.

here are my problems
- The APP crashed if I select the "Modes Setup" (just sent you the feedback anda data log on crash)
 - No data is retrieved, even though the module is connected.
- If presson "?" + "chack for Faults" I get " ESC not connected"

could you pleas help?
I would love to use your APP.

Giuseppe
```

---
## \#625 Posted by: Slak Posted at: 2018-05-24T13:57:10.692Z Reads: 150

```
No, I'm talking about the speed rotation of the wheels; not the speed of the board :

You said : "I made a video and basically the left motor spins faster  (master VESC 
with uart module attached) than the slave. This thing doesn’t happen to 
me when I ride in the let’s say full power mode. Here the video, I 
couldn’t go full throttle without weight because the motors start 
rattling"
```

---
## \#626 Posted by: rey8801 Posted at: 2018-05-24T14:10:51.026Z Reads: 149

```
Ah sorry It has been a while ago. At that time I just noticed this behavior on the slave connected motor side once I use to set the watt really low. ANyhow thanks for the suggestion.
```

---
## \#627 Posted by: Ackmaniac Posted at: 2018-05-24T15:57:42.482Z Reads: 145

```
Maybe try to uninstall and install again to fix the Mode problem.
```

---
## \#628 Posted by: piepolitb Posted at: 2018-05-24T16:23:03.826Z Reads: 143

```
Tried that...it didn't worked
```

---
## \#629 Posted by: SuperBen Posted at: 2018-05-24T18:13:09.988Z Reads: 143

```
Do you have a single or dual drive setup?

If dual, is the uart connected to master or slave? If slave, make sure the option to "Send Status To CAN:0) is selected, provided your master is set to 0 in BLDC tool of course
```

---
## \#630 Posted by: piepolitb Posted at: 2018-05-24T18:34:29.525Z Reads: 144

```
SORRY SORRY GUYS

my bad, I didn't activated UART with the correct baudrate
```

---
## \#631 Posted by: Ackmaniac Posted at: 2018-05-24T19:20:42.945Z Reads: 138

```
Good to know that the app crashes when the baudrate is wrong. Never gave that a try.
```

---
## \#632 Posted by: Ackmaniac Posted at: 2018-05-24T20:31:00.346Z Reads: 141

```
Maybe you should have a look in the tool at the ppm values to find out what is going on. Hard for me to understand what is going on. Maybe make a video which shows the live values in the tool.
```

---
## \#633 Posted by: rok Posted at: 2018-05-24T21:21:23.839Z Reads: 141

```
ok so i should write it as a default in the app and then read it in the vesc tool and check for ppm values. if so, i'll do that this weekend.
```

---
## \#634 Posted by: Aeroquiv Posted at: 2018-05-26T04:18:15.084Z Reads: 138

```
Wait so the original HM-10's that you linked from awhile back won't work with the Pixel 2's?
```

---
## \#635 Posted by: Ackmaniac Posted at: 2018-05-26T08:05:25.865Z Reads: 142

```
Right, because they were clones from China.
```

---
## \#636 Posted by: gaetjen Posted at: 2018-05-27T19:09:32.081Z Reads: 138

```
So, I had a weird incident today. My nephews wanted to ride my board, so I put on my "kinder" modus and instead of moving forward when pulling the trigger, the board went backwards. When I pulled the trigger in the other direction it even went faster backwards. Luckily, no one was on the board. This didn´t happen when I used my "ludicrous" mode. After trying other modes and changing values I found out that doesn´t happen when the motor amp is at 30 or higher. Before that I had it at 15 and it moved backwards. Does any of you have the same problem?
```

---
## \#637 Posted by: rok Posted at: 2018-05-27T20:47:37.483Z Reads: 137

```
[quote="rok, post:620, topic:20888, full:true"]
I don’t have that button to change the direction on my remote.

I set my defoult values on your bldc tool so why does it work on defoult and not when i set it through the app.

Either way, even if i set it up as current with reverse, it doesn’t matter which direction i push the throttle it will always go backwards. So pushing forward, the board goes backwards, pushing backwards, the board is still going backwards
[/quote]


I do. Scroll some posts higher up. There is a ''SOLUTION''.
```

---
## \#638 Posted by: Ackmaniac Posted at: 2018-05-28T11:47:33.943Z Reads: 130

```
Please check if the PPM mode in "kinder" is the same as in "ludicrous". And do you use BLDC or FOC. I never experienced that behavior and need to have a look. But i need more information (modes, parameters a.s.o.).
Maybe you can make screenshots of your different modes. That would help me a lot.
```

---
## \#639 Posted by: gaetjen Posted at: 2018-05-29T16:34:53.526Z Reads: 143

```
![vescmonitor|281x500](upload://sjoDe2jikvYIN7qCNsft4Zo9uaH.png)
These are the values when the board accelerates in the wrong direction. As soon as I switch the motor amps to 30 it accelerates normal.
```

---
## \#640 Posted by: Ackmaniac Posted at: 2018-05-29T16:41:07.222Z Reads: 141

```
Interesting. Do you use FOC or bldc? And which firmware version?
```

---
## \#641 Posted by: gaetjen Posted at: 2018-05-29T16:44:43.431Z Reads: 143

```
newest firmware (3.101) and Bldc, but it also happens in FOC. Tried both. I can also send you a video if neccessary
```

---
## \#642 Posted by: Ackmaniac Posted at: 2018-05-29T20:31:12.636Z Reads: 151

```
Jesus. Now I see the problem. It happens when motor max is lower than motor min. Will work on it and provide a fix soon.
Man that's scary.
```

---
## \#643 Posted by: Ackmaniac Posted at: 2018-05-29T22:02:02.331Z Reads: 161

```
Found the issue in the software and fixed it. I will try to release a new version tomorrow which fixes that issue.
Thx a lot to @gaetjen and @rok who didn't gave up to convince me that the problem isn't on their side.
```

---
## \#644 Posted by: rok Posted at: 2018-05-29T22:07:39.400Z Reads: 175

```
Never! :grinning:
You're the man, thanks!
```

---
## \#645 Posted by: Ackmaniac Posted at: 2018-05-31T20:53:17.138Z Reads: 243

```
@rok and @gaetjen
http://www.electric-skateboard.builders/t/extended-ackmaniac-esc-tool-based-on-vesc-tool/35116/459?u=ackmaniac
```

---
## \#646 Posted by: Ackmaniac Posted at: 2018-05-31T21:15:29.781Z Reads: 240

```
**Just released new Version 1.97**

it improves the connection and has one very cool new feature. You are now able to connect to Ackmaniac-Tool or VESC-Tool via the app. 
To do so you need to press the question mark sign on top and then in the menu the entry "Start TCP Connection"
![image|275x500](upload://2D67fiIM9bTrD5Oqt2su99UCoTD.png)
Then a popup window will appear that shows you the IP of your smartphone and the Port you need to connect to.
![image|273x500](upload://nw7wqoqAJztO1KnLAsEVITnqQN8.png)

Then in the Ackmaniac-Tool go to connections, select the TCP tab and enter the id and port. Then press connect.
![image|690x142](upload://iZiVf8vU5vNw5t2zcoXlWocxZCb.png)

If it doesn't work at all then please stop and restart the Wifi connection of your phone. Of course your Smartphone and PC need to be in the same network for this.
If you are outside and have your Laptop then you can activate a Hotspot on your Phone and connect to the Hotspot with your Laptop. 
Hope it works for everybody.

[Donations](https://www.paypal.com/donate/?token=Elb6MIetetKzhbKfPkWSH02R1OVV5HTsxnqnUmWsnx7ajXOmDkijLH5SDDPEsOHgP6f0W0&country.x=DE&locale.x=DE) are always welcome and will be invested directly in :coffee: which i had a lot in the last days for the new firmware and app version.
```

---
## \#647 Posted by: rey8801 Posted at: 2018-05-31T21:32:59.107Z Reads: 205

```
That's awesome, so I guess in order to be able to work wireless with both of the vesc we would need to bluetooth modules connected to the vescs. Is it correct? Anyhow I can connect via TCP. Thx
```

---
## \#648 Posted by: Ackmaniac Posted at: 2018-05-31T21:47:25.190Z Reads: 199

```
You can connect via CAN with the app and also with the ACKMANIAC-Tool or VESC-Tool.
```

---
## \#649 Posted by: rey8801 Posted at: 2018-05-31T21:54:30.809Z Reads: 197

```
Sorry I didn't explain properly. I know I can change the motor battery setting through the app and via CAN be transfered to the slave VESC. My question was about firmware update. Is it possible to update the firmware om the VESC via TCP? Do O need 2 bluetooth modules km that case? Thx
```

---
## \#650 Posted by: Sebike Posted at: 2018-05-31T21:58:35.929Z Reads: 194

```
That's a cool feature! Quick question. 

Anything that is limited on the Ack-tool when connecting to the app via TCP? For instance, would motor detection work?
When reading real time data in the tool via app it looks like the ack-tool looses connection/read once every few seconds, so it doesn't run very smooth. Is this just how it is when running though TCP ?
```

---
## \#651 Posted by: Ackmaniac Posted at: 2018-05-31T22:04:27.371Z Reads: 193

```
No firmware updates won't work. Over Bluetooth it happens that packages get lost. And for a firmware update it needs to deliver like 20000 packets. So that won't work. But motor detection, and read and write of settings works.

[quote="Sebike, post:650, topic:20888"]
When reading real time data in the tool via app it looks like the ack-tool looses connection/read once every few seconds, so it doesn’t run very smooth. Is this just how it is when running though TCP ?
[/quote]
@Sebike I don't understand what you want to say.
```

---
## \#652 Posted by: rok Posted at: 2018-05-31T22:12:28.872Z Reads: 186

```
Thats the dream @Ackmaniac! Wireless, wireless everything :heart_eyes:
```

---
## \#653 Posted by: Sebike Posted at: 2018-05-31T22:19:47.233Z Reads: 192

```
Ok, so here is realtime data taken from the vesc when connected via USB and then via the app (TCP) 

USB
https://youtu.be/UDgZIsBXybc

TCP
https://youtu.be/ZFO3LuMil2o
```

---
## \#654 Posted by: SuperBen Posted at: 2018-05-31T22:21:39.194Z Reads: 173

```
@Ackmaniac you are the man! Connecting wireless to the pc tool is the only thing I've been missing!

donation incoming :D
```

---
## \#655 Posted by: Ackmaniac Posted at: 2018-05-31T22:27:19.965Z Reads: 182

```
Yes the connection isn't as stable as with USB. Best is to place the phone and Laptop close to your WIFI Router and the board close to the Phone. Also be aware that the reliability of your Bluetooth connection can be very different in portrait (vertical) and Landscape (horizontal) position.
And if you want a faster connection you could increase the baud rate of your Bluetooth module via AT commands.
And Heart Beat (Heart sign) should best be deactivated because it occupies the connection a lot.
Samples will also not work. Just simply see it as a possibility to read and modify your settings without taking the enclosure off.
```

---
## \#656 Posted by: Sebike Posted at: 2018-06-01T07:57:32.321Z Reads: 181

```
I've been writing a couple of times about not getting KV reads in the terminal of the Ackmaniac-tool, so as the feature was implemented with the app I thought I'd try it, but unfortunately with the same disappointing results = 

it just says measured kv: 0.00 rpm/v. ERPM reads are fine when checking for that, but not kv. 
I've tried this on both motors (running dual focboxes). 

Any thoughts why?
```

---
## \#657 Posted by: Ackmaniac Posted at: 2018-06-01T08:31:29.037Z Reads: 176

```
Because the motors need to spin to detect the kv. So just speed them up, release the throttle and immediately enter the kv command while they still spin.
the value you will see then needs to be devided by (number of magnets/2).
So when you get 1330 then devide it by (14/2). 1330 / 7 = 190

If you have a 6374 190kv motor then don't be surprised when you get a value in the 170kv range.
```

---
## \#658 Posted by: Sebike Posted at: 2018-06-01T08:42:19.912Z Reads: 176

```
Yes, this is what I'm doing getting 0.00 rpm/v

full throttle, 50% throttle, release throttle with motor spinning... weird
```

---
## \#659 Posted by: rey8801 Posted at: 2018-06-01T09:18:34.465Z Reads: 173

```
I tested on different PC, but basically I can connect easy via TCP but I can not read the configurations present on the VESC both motor and app. Do you have any idea why?
```

---
## \#660 Posted by: Ackmaniac Posted at: 2018-06-01T09:57:40.840Z Reads: 170

```
Post a video when you try to connect and read the settings. That might help.
```

---
## \#661 Posted by: rey8801 Posted at: 2018-06-01T18:57:10.848Z Reads: 171

```
So I tried with another pc and this time it worked. Perfect. I see the parameters but if I try to change them and click write the motor configuration it doesnt do anything and if I check again it still have the old value.

Second thing I tried the KV detection. I get 634 rmp/volt and my hubs have 20 magnets so I get 15 KV when should be around 75. Did I do something wrong? Thx

![vescmonitor|281x500](upload://7nqUjTsOlCQirbRTTlJvVM34KSD.png)
```

---
## \#662 Posted by: Ackmaniac Posted at: 2018-06-01T19:13:03.431Z Reads: 155

```
Its magnets / 2. So 634 / (20/2)  = 634 / 10 = 63,4

And with the write i also saw the the green Text at the bottom right doesn't appear with the write. But in my case the write worked. Just change a value, press write maybe multiple times and then read to see if it changed the values.
Think i know why it doesn't appear but don't have the time right now to spent time on it. So maybe in the next days.
```

---
## \#663 Posted by: rey8801 Posted at: 2018-06-01T19:24:54.915Z Reads: 153

```
Thx! I read the formula too fast :laughing:

I will try again the writing function. Thx
```

---
## \#664 Posted by: rey8801 Posted at: 2018-06-02T06:57:13.477Z Reads: 158

```
Update: With me it does,t work. App vers 1.98 I can connect to pc via TCP but I only get the green text for connection but not the ones that tell about read motor and app conf. Indeed I do not see the value present on the VESC anymore. Moreover after 3 minutes connected the app crashes.

May I ask you something. I have dual hubs motor, 10s3p 30Q battery and I set a max watt of 1950 watt (975*2) with batt max 30A, motor max 50A motor min -45 and att min -6. Now my question is why I always see in the telemetry chart that for instance I get 1400 watt (700*2) out of it? the batt current never go more than 40A (I guess is times 2 in the app so 20A per VESC) and motor current reaches 45A (so 2.25A per VESC). MAybe it is just the physical system limit for my motor and battery. I just would like to ask you your opinion. Thx
```

---
## \#665 Posted by: Quezacotl Posted at: 2018-06-02T08:38:52.942Z Reads: 168

```
Tiny little suggestion on the android app :smile:
 When changing the screen resolution, the infoboxes won't follow. Would be nice to have them staying full screen all the time or adjustable in options.
![Screenshot_20180602-102037|281x500](upload://gyoXzFBixRSSb9fIP7bUouWRbPN.png)
![Screenshot_20180602-102023|281x500](upload://kCKjJsggbP2iC8YE2BfRQjATeMO.png)
```

---
## \#666 Posted by: Ackmaniac Posted at: 2018-06-02T09:49:47.874Z Reads: 148

```
[quote="rey8801, post:664, topic:20888"]
I set a max watt of 1950 watt (9752)
[/quote]

What does the 9752 in brackets stand for.
Do you use a BMS that might limit the power output.
What firmware do you use?

A watt max of 1950 doesn't male much sense when you your battery max is at 30A. Because with a 10S battery that is fully charged you will get a voltage of roughly 36V under load. And 36V * 30A = 1080. So the max watts can't be reached in any case and battery max sets your limit.

How do you try to reach max power. By doing full throttle at full speed?
```

---
## \#667 Posted by: rey8801 Posted at: 2018-06-02T10:50:12.742Z Reads: 157

```
Wrong typing it means 1950 watt from the sum of two vescs (975 watt x 2). My bms is a 60A constant current with burst current at way higher A. So should be fine.
I thought the max watt would be the sum of the two motors and vescs. I am running dual hub motors, so 30A on each vesc and 50A on each motors.

![vescmonitor|281x500](upload://tQN9URF9tIS4zSBd3rLEW7QDZ5w.png)
```

---
## \#668 Posted by: Ackmaniac Posted at: 2018-06-02T10:57:10.606Z Reads: 144

```
Settings lookok. How do you test the max power output?
```

---
## \#669 Posted by: rey8801 Posted at: 2018-06-02T11:12:25.116Z Reads: 158

```
From the ride logs.

![vescmonitor|281x500](upload://zKm0tGpshwEysGEAkRTvR4LMEi1.jpg)

As you can see even at full throttle I am far from my watt limit. Maybe are the motor that can not perfome more. Although they can not decide it, they should give until death :laughing:

I know @ElskerShadow is running a simili set up on his spud deck. Could you please check which value you get with the same hubs and almost same currents settings (of course you have telemetry in that board). Thx a lot :grin:
```

---
## \#670 Posted by: Ackmaniac Posted at: 2018-06-02T11:24:14.189Z Reads: 154

```
When you only answer half or none of my questions it is hard to help. So to make it easy please make a video with the app. And try to reach the maximum power output in the video by accelerating, braking and accelerating again.
If you are already at full speed and do full throttle you can't reach the maximum performance. Especially when your board does 35 km/h max.

And please don't full this thread with problems that are not really related to the app. Feel free to open your own topic.
```

---
## \#671 Posted by: rey8801 Posted at: 2018-06-02T11:25:53.431Z Reads: 156

```
Ok I will try. Sorry I though the ride logs could help.
```

---
## \#672 Posted by: rey8801 Posted at: 2018-06-02T11:26:16.642Z Reads: 162

```
Donations sent. 

https://www.electric-skateboard.builders/t/esk8-flea-market-eu-us-small-cheap-parts/57463/5?u=rey8801
```

---
## \#673 Posted by: ElskerShadow Posted at: 2018-06-02T16:11:23.126Z Reads: 163

```
I can do that for sure!
```

---
## \#674 Posted by: rey8801 Posted at: 2018-06-02T16:27:11.290Z Reads: 163

```
Sweet :grin: thx a lot man!
```

---
## \#675 Posted by: Ackmaniac Posted at: 2018-06-02T21:45:47.131Z Reads: 165

```
No i see you started sell BLE Modules with the possibility to leave a donation for me. Nice idea Thx a lot.
```

---
## \#676 Posted by: rey8801 Posted at: 2018-06-02T21:50:49.645Z Reads: 160

```
No problem, my pleasure. I though we mostly use them with your app, so in that way we can support your work.
```

---
## \#677 Posted by: Maxid Posted at: 2018-06-03T10:30:27.576Z Reads: 166

```
Do we have a supplier in Germany that is knkown to work well with Oreo? I don't want to wait weeks for the china one to arrive.
```

---
## \#678 Posted by: Ackmaniac Posted at: 2018-06-04T07:50:36.991Z Reads: 163

```
**Just released a new Version 1.99**
Before when you were connected to the ACKMANAIC-Tool via TCP and the app then you couldn't see when you were writing the settings. This bug is fixed now.
```

---
## \#679 Posted by: rey8801 Posted at: 2018-06-04T09:21:18.443Z Reads: 163

```
Tested it out and now everything works...fantastic. I can connect, move tot the slave vesc via CAN. I see the motor and app writing. The only thing that doesn't work for me is the motor detection, the part of BLDC detection. I mean the motor spin and everything but I do not get any value out of it. I just wanted to report it.
```

---
## \#680 Posted by: Ackmaniac Posted at: 2018-06-04T13:56:36.509Z Reads: 156

```
will have a look.
```

---
## \#681 Posted by: Ackmaniac Posted at: 2018-06-04T17:17:47.661Z Reads: 154

```
**just released version 1.100.**
Motor detection works now as well.
```

---
## \#682 Posted by: rey8801 Posted at: 2018-06-04T17:21:12.636Z Reads: 150

```
Fantastic...I will try and let you know
```

---
## \#683 Posted by: rey8801 Posted at: 2018-06-04T18:44:52.591Z Reads: 150

```
Tried...now everything works properly. I did moto detection, ppm mapping ecc... all fine. Thx a lot!
```

---
## \#684 Posted by: accrobrandon Posted at: 2018-06-04T21:53:45.352Z Reads: 155

```
hi,

so just to make sure i got it right... I use OSX so use the bldc tool and flash this bin file 

"VESC_Ackmaniac_Mod_2_54.bin.cpgz"

then i can make the changes via BT after redoing all motor detections and setting initial values? 

thx
```

---
## \#685 Posted by: Ackmaniac Posted at: 2018-06-04T23:12:02.624Z Reads: 148

```
No you can't because it won't work with 2.54. Only with 3.100, 3.101, 3.102 of you want to use my firmware mod or the original vesc-tool firmwares. So more or less everything that as a 3 at the beginning.
```

---
## \#686 Posted by: Thunkar Posted at: 2018-06-05T14:19:25.291Z Reads: 150

```
@Ackmaniac I'm having some trouble on a Xiaomi Mi A1 (Android 8.0). I used the app for a while and it run perfectly, but after some time (sorry, can't remember the version), it only seems to work right after it has been updated. It works once, then it connects but doesn't show any info. Trying to check for faults yields the message "ESC not connected". Clearing cache and data app doesn't help either. Thanks for all your hard work, I hope you can point me in the right direction!
```

---
## \#687 Posted by: rey8801 Posted at: 2018-06-05T14:23:43.433Z Reads: 144

```
I also have Xiaomi but mi5. I found that the app runs way better if you give it all the permissions. I do not know if with Android 8 you meant that your phone has actually Android or if it's like mine that runs MIUI which is based on Android. If yours is the second case, then go into permission and allow the app to work in background and  give it all the rights.
```

---
## \#688 Posted by: Thunkar Posted at: 2018-06-05T14:41:16.839Z Reads: 143

```
Thanks for the idea, but my phone runs stock Android (it is included in the Android One project, Xiaomi only makes the hardware). I've given the app all the permissions and I actually can see a fixed system notification saying it is running in the background, but still doesn't work.
```

---
## \#689 Posted by: rey8801 Posted at: 2018-06-05T14:43:20.540Z Reads: 140

```
It was wothed a try :wink:
```

---
## \#690 Posted by: Ackmaniac Posted at: 2018-06-05T14:50:04.714Z Reads: 142

```
Just decativate bluetooth and activate it again, or restart your phone. If that doesn't help then ???.
Maybe check if the app is deactivated in the list of apps that should be optimized for battery life.
```

---
## \#691 Posted by: DeathCookies Posted at: 2018-06-05T14:53:05.136Z Reads: 143

```
Sometimes i had the same Problem... couldnt connect properly to my board.

The following worked for me:
1. Turn on remote
2. Turn on app
3. turn on board
4. connect to the board
```

---
## \#692 Posted by: Thunkar Posted at: 2018-06-05T15:06:34.513Z Reads: 146

```
Tried all that, still problems. My GF has the same phone and the behavior is the same. Maybe more Android 8 crazyness? Thanks anyway, please let me know if there's any way in which I can send you debugging info.
```

---
## \#693 Posted by: accrobrandon Posted at: 2018-06-06T02:07:35.793Z Reads: 160

```
So is there a 3.xx bin file somewhere? Or do I have to use your tool which is only for PC? Cuz I dont see any bin files in the newest folder on Dropbox.... Unless I'm missing something
```

---
## \#694 Posted by: Maxid Posted at: 2018-06-06T09:12:35.916Z Reads: 168

```
I just wanted to inform you guys that a non-working HM10 can be updated to one that is recognized by Android Oreo. I just tested it with a CC2541 clone and my Galaxy S8. Once updated the phone is able to find the module again and it shows up in the app. i have not hooked it up to a VESC yet but that seems trivial now.
All you need is an Arduino and the following steps: https://forum.arduino.cc/index.php?topic=393655.0
I used an Arduino DUE (because it already runs at 3.3V) and soldering the three pins was the most time consuming part (so all in all it really only takes a couple minutes). So I am off to update my second module :D

Edit: second module successful :+1:
```

---
## \#695 Posted by: Pimousse Posted at: 2018-06-06T09:26:56.670Z Reads: 169

```
Did worked for me as well, using this link : https://blog.yavilevich.com/2018/04/should-you-throw-away-your-cc41-hm-10-clones-now-that-android-8-is-here/
I did updated metr.at module as well, but for now the app doesn't seem to find it (but could be app restriction also, need to investigate more).

2 remarks though between clone FW and official one :
- AT commands are not exactly the same
- State pin isn't affected to the same CC2540 IO (but who cares ?)
```

---
## \#696 Posted by: Maxid Posted at: 2018-06-06T09:31:05.344Z Reads: 159

```
I think metr modules have some sort of protection that might get erased once you update the firmware. i thought it was mac-address based but if you have problems after updating then the protection might be just programmed. Did you change the name to its original form?
```

---
## \#697 Posted by: rey8801 Posted at: 2018-06-06T09:36:41.887Z Reads: 160

```
I also tried this process but it didn't work for me with the module I had. Basically the process fails when I run the firmware update in the terminal. I get this error:

Waiting for respond from Arduino...
No chip detected!
Upload Failed!
File closed!
Comport closed!

Anyhow here a video explanation that always helps https://www.youtube.com/watch?v=ez3491-v8Og&lc=z23nwhdxqsf5svdu5acdp43brk0rmcash2ctnjuwrmhw03c010c.1527327978908921
```

---
## \#698 Posted by: Pimousse Posted at: 2018-06-06T09:40:52.612Z Reads: 148

```
Check the wiring.
I had this issue as well because I swapped 2 wires.

@Maxid, Sure, I changed the name. I also checked that UUID didn't change.
You're right, some settings should maybe be tweaked to allow the comm. with the app.
```

---
## \#699 Posted by: rey8801 Posted at: 2018-06-06T09:49:10.340Z Reads: 157

```
I still have the pictures. I have tried at least 15 times, with 3V, 5V everything...if you find the error...then I love you :rofl:!

![IMG_20180526_005019|690x388](upload://5e8pqcMuaM4zyAY4EESm5rfMcBK.jpg)![IMG_20180526_004821|690x388](upload://d4MxK86ZHMHE0lsuL9PLCvngb15.jpg)![IMG_20180526_004442|690x388](upload://e2L4D962vkJ0Ljgd1LXm7L30pMh.jpg)![IMG_20180526_005007|690x388](upload://sROoZ8VQ7IgtZOXj7ZOX5uIDQmv.jpg)

I was thinkg that maybe the module I used has a different diagram. It was a classic HM-10 clone CC2541
```

---
## \#700 Posted by: Pimousse Posted at: 2018-06-06T10:12:34.069Z Reads: 156

```
Here was my setup : 
![IMG_20180508_070341|375x500](upload://i5ITFigBFnhKAlUAVrBUgVrhwsQ.jpg)

![IMG_20180508_083248|666x500](upload://Ao4J7YuJD9HJmAkrE2AfCILDGYV.jpg)
```

---
## \#701 Posted by: rey8801 Posted at: 2018-06-06T10:39:24.274Z Reads: 148

```
the only difference I see is that I used the pins of the breakout board to power the module instead of solder the jumper pins to pin 12 and 13 of the module as you did it. I do not know if it matter, but I will give it a try. 
@Maxid did you also follow the same scheme? meaning soldering the jumpers on the 3.3V and GRD ports on the module and not using the male pins of the breakout board. The same one that you use whe nyou prepare the module to be connected to the VESC.

Thx for the help
```

---
## \#702 Posted by: Maxid Posted at: 2018-06-06T10:42:23.492Z Reads: 155

```
That's how I did it [img]upload://4a6ey0XKSQUpC2UrDwt0JJp1TN9.jpg[/img]
```

---
## \#704 Posted by: rey8801 Posted at: 2018-06-06T10:44:46.408Z Reads: 146

```
Yeh same I did it. I do not know what I am doing wrong.
```

---
## \#705 Posted by: Pimousse Posted at: 2018-06-06T10:45:06.870Z Reads: 149

```
Well, for metr module, I powered it up via connector (5V from Arduino).
I used a little software instead of terminal.
Check my link above.
```

---
## \#706 Posted by: Maxid Posted at: 2018-06-06T10:51:41.817Z Reads: 152

```
Honestly your wiring looks a little sketchy to me. Did you try sending AT commands? Did that work? I'd clean up the wiring and make sure everything is soldered properly. I also used a different ccloader.exe  called CCLoader_x86_64.exe. Did you try it several times with for example an Arduino reset it between? Maybe the old "turn it off and on again" works here as well.

@moderators : I feel like we went quite a bit off-topic here. Sorry @Ackmaniac. You guys should probably move this to its own thread.
```

---
## \#707 Posted by: rey8801 Posted at: 2018-06-06T10:52:23.331Z Reads: 148

```
OK I will. No off topic anymore.
```

---
## \#708 Posted by: Ackmaniac Posted at: 2018-06-06T18:41:18.385Z Reads: 151

```
Feel free to discuss this. Great when you can find a easy and reliable way to do it so that others can use the app again with Android 8.0
Didnt find the time to give it a try myself yet.
```

---
## \#709 Posted by: rey8801 Posted at: 2018-06-06T19:41:16.859Z Reads: 152

```
Thx man!
10ch
```

---
## \#710 Posted by: Ackmaniac Posted at: 2018-06-06T21:04:18.969Z Reads: 164

```
Tested it myself and it works. You don't need to solder the wires to the pins. Just take a needle and make a little hole at the pins. Then stick the wire in and hold it in place with your hand or with tape. Of course I fucked it up the first time by mixing up 2 wires (like a curse, happens every time). 
And I had the problem that I couldn't use my original ports 26 and 37. Seems only low numbers are accepted so I had to change it to the number 2 in windows device manager. 
![IMG_20180606_222929|375x500](upload://dKCHveKLhIWv8i4SGKvNvKZZ22V.jpg)
```

---
## \#711 Posted by: Ackmaniac Posted at: 2018-06-06T21:18:54.464Z Reads: 152

```
Did you upload the sketch to the arduino? Just make sure it had no faults during writing
```

---
## \#712 Posted by: rey8801 Posted at: 2018-06-06T22:01:57.545Z Reads: 151

```
Yes everything works until I try to upload the firmware to the module. I will give it another try for sure.
```

---
## \#713 Posted by: Ackmaniac Posted at: 2018-06-06T22:07:49.371Z Reads: 154

```
Just check again your connections. Should look like this ![image|262x109](upload://9xpi2ZEpNHSGJKa3oWiv3B9KrdC.png)
```

---
## \#714 Posted by: rey8801 Posted at: 2018-06-06T22:10:28.541Z Reads: 153

```
Yes I know. I watched the video and read the tutorial 20 times. I think I maybe made weaker connection by soldering not properly so I will give it another try.
```

---
## \#716 Posted by: Ackmaniac Posted at: 2018-06-06T23:30:47.506Z Reads: 153

```
Just released a new version 1.101. Trying to automatically reconnect in case you lost connection in a couple of seconds.
```

---
## \#717 Posted by: rey8801 Posted at: 2018-06-07T03:32:06.851Z Reads: 159

```
Sweet. I was wondering, maybe it's already like that but when you want to detect fault in the app and the Bluetooth it's connected to the master VESC, does it actually check for faults also for the slave VESC or is it only possible for the master side? Same question in case you connect to vesc tool via TCP and move to the slave VESC via CAN.
Thx
```

---
## \#718 Posted by: Ackmaniac Posted at: 2018-06-07T06:34:29.856Z Reads: 159

```
When you are connected to the master(CAN or directly doesn't matter) then the app will check at start which slaves are connected and check for faults of all members. But after that first initial check it only recognizes the faults of the one you are currently watching.
```

---
## \#719 Posted by: rey8801 Posted at: 2018-06-07T07:00:27.203Z Reads: 159

```
Ok perfectly good to know. Because I read the sometimes to detect DRV faults you need to spin the motor so I'm this case only the one directly connected can be detected.
I was wondering if to allow the firmware upload through the app via TCP you would only need a faster baud than 9600. I also understand that you  would need to modify each module via AT commands...which makes everything less friendly use.
```

---
## \#720 Posted by: Ackmaniac Posted at: 2018-06-07T07:26:14.186Z Reads: 148

```
Firmware upload works already. I was surprised as well. But the firmware uploads will only work with my firmware because there i use a default baud rate of 9600. The original firmware uses 115200.
```

---
## \#721 Posted by: rey8801 Posted at: 2018-06-07T07:34:26.748Z Reads: 154

```
Man you should highlighted it! Or an I the only one that missed it? Fantastic. I am using your firmware BTW. I guess it would just be just slightly slower. Next step for you would be make a VESC tool app version with your firmware :laughing: Not that I need it, it's just nice...
```

---
## \#722 Posted by: Thunkar Posted at: 2018-06-07T17:44:55.652Z Reads: 151

```
Hi, I just tried the new version. It worked for me a few times, but now it's back to the bad behavior...however, I noticed one odd thing:

If I deactivate the location services on my phone, or just refuse to give the app the permissions to access the GPS, the bluetooth device list remains empty. If I had my board registered, it appears greyed out. Also, even with all the services activated and giving it the permissions, it still shows the "functionality reduced" prompt. Could it be a permissions issue?
```

---
## \#723 Posted by: Ackmaniac Posted at: 2018-06-07T17:49:06.373Z Reads: 146

```
Bluetooth low energy needs GPS permissions. Even if it doesn't activate GPS. Don't ask me why.
```

---
## \#724 Posted by: Thunkar Posted at: 2018-06-07T19:54:27.533Z Reads: 147

```
Well, didn't know that, sorry. I'll report if I find anything new, thanks anyway!
```

---
## \#725 Posted by: rey8801 Posted at: 2018-06-09T07:43:17.697Z Reads: 153

```
Update: I received the update 1.103 and now when the app is connected to the vesc a blinking message says "No storage folder found" is appering. I see in the logbook that the app created the new file although the messagge is always there. PLus the TCP connection is more instable, I could connect via CAN to the slave and also the motor and app writing/reading worked only sometimes. WIth the 1.101 I everything worked proberly.
I just wanted to report to you @Ackmaniac. Thx!
```

---
## \#726 Posted by: Maxid Posted at: 2018-06-09T15:35:24.412Z Reads: 148

```
Just came back from a ride with the Lou and thought about a useful new feature: an upload button to @DeathCookies'https://gct-hp.de/VDLA/ to get a better visualization of the ride.
```

---
## \#727 Posted by: rey8801 Posted at: 2018-06-09T15:41:16.633Z Reads: 152

```
True. Would also be nice the possibility to share it with the all ride data as metr does.
```

---
## \#728 Posted by: Ackmaniac Posted at: 2018-06-09T18:19:47.738Z Reads: 149

```
Isn't a video the a much better way to share your ride? Especially with realtime data.
```

---
## \#729 Posted by: rey8801 Posted at: 2018-06-09T20:23:43.041Z Reads: 151

```
Yes it's super nice. I just suggested another option. The nice thing of having a shareable interacting data log is that you can go through the ride and share the whole data on forum to better understand if there is problem whatsoever while with the video you can not actually quick see it because you see the real data but they are in steaming so more difficult to compare than an organize chart.
Anyhow do you have a public folder where it's possible to find the old apk of the app? As I said before the new update made it worse in my case when the 1.101 was working just fine. Thx
```

---
## \#730 Posted by: Ackmaniac Posted at: 2018-06-09T20:35:56.641Z Reads: 151

```
Released already another update. Please give it a try
```

---
## \#731 Posted by: rey8801 Posted at: 2018-06-09T20:39:22.619Z Reads: 146

```
I will report back in 20 minutes :grin:
```

---
## \#732 Posted by: Ackmaniac Posted at: 2018-06-09T20:40:27.860Z Reads: 146

```
If you flashed your BLE module or have a decent HM-10 I recommend to execute the AT command AT+POWE3 which sets it to the highest transmitting power of 6dbm. This is then about 4 times as strong as standard.
```

---
## \#733 Posted by: rey8801 Posted at: 2018-06-09T20:48:25.879Z Reads: 146

```
Cool! I will try with another module first. Because mine is inside the enclosure, with hot glue ecc... A pain to remove it :grin: anyhow I have really stable signal now. Once you suggested to move far from the motor wires and indeed now the connection is stable.
```

---
## \#734 Posted by: rey8801 Posted at: 2018-06-09T21:12:27.796Z Reads: 142

```
Tried 1.105. It's even more stable than 1.101. Works perfectly now. Thx
```

---
## \#735 Posted by: Ackmaniac Posted at: 2018-06-09T22:08:38.372Z Reads: 150

```
I think the stability of the TCP connection has also to do how far away you are from your router and to your board. So it's best to bring board router and smartphone close together.

@rey8801 thx for testing and feedback.
```

---
## \#736 Posted by: rey8801 Posted at: 2018-06-09T22:29:31.343Z Reads: 156

```
At the time of the 1.103 I tried also really close to the router and with Hotspot that usually was really stable but nothing. Now with 1.105 I was on wifi. Far from the router and no problem. Better like that :sunglasses:
```

---
## \#738 Posted by: Thunkar Posted at: 2018-06-10T16:03:38.649Z Reads: 162

```
@Ackmaniac hi again! After the latest update I'm still not seeing any info, but now I get a "No storage found to save file prompt" every few seconds. After checking, I saw that the app is able to create a folder for itself even if I delete it manually, but the files inside of it are 0 bytes each and corrupted. It has the storage permissions granted. Could the file writing API have changed in Android 8? Could you please add a toggle to disable file logging and see if I can at least get the live data? Thanks a lot!
```

---
## \#739 Posted by: Ackmaniac Posted at: 2018-06-10T17:32:08.331Z Reads: 157

```
Sure you are using the latest version, please have a look if there is a update available. And ignore the file that is in the main folder. After finishing the ride the file will be saved to the correct folder of today.
```

---
## \#740 Posted by: gaetjen Posted at: 2018-06-10T18:54:54.082Z Reads: 157

```
Can you elaborate on that a little bit more? How can I  extend the range of the bluetooth connection?
```

---
## \#741 Posted by: Skifree Posted at: 2018-06-12T04:05:35.840Z Reads: 157

```
If you are connected to the module via bluetooth, open the app "serial bluetooth terminal", then select the bluetooth module in the devices tab under the hamburger menu. Then go back to the terminal selection and press the connect button next to the trash bin. Then you should see a constant flow of stuff. At the bottom of the screen enter AT+POWE3 press the little enter button that looks like an arrow and it should send the command over to the module. There are many more commands or queries that you can make as well. Search for AT commands HM-10 and you should be able to find some links to the commands.

Hopefully that will work for you.
```

---
## \#742 Posted by: gaetjen Posted at: 2018-06-12T21:44:06.331Z Reads: 161

```
[quote="Skifree, post:741, topic:20888"]
Then you should see a constant flow of stuff
[/quote]

I am connected, but I don´t see that and if I type in commands and send them, I don´t get an "answer". Any idea what the problem could be?
![serial_bluetooth_terminal|281x500](upload://9n1bMN6DEzqwLt6PCSmuEbVksNx.png)
```

---
## \#743 Posted by: Ackmaniac Posted at: 2018-06-13T01:02:22.548Z Reads: 155

```
Normally the devices are not configured to be programmed from the client side. So by default they only can be programmed when no client is connected. But they can be set to another mode where they also accept AT commands form the client. But for that you ned to connect to them via arduino anyway to give that commend. And once you have that sorted out you could configure them right away, so no need to configure them from client anymore.
```

---
## \#744 Posted by: Skifree Posted at: 2018-06-13T03:10:40.654Z Reads: 154

```
That's odd, mine would originally return a bunch of jiberish text when I sent a command, but I paired my phone to my garmin watch hoping to get notifications and now I'm getting the same thing.... 
@Ackmaniac Could mine be different because it is an MLT-BT05? Also thanks for the killer app!
```

---
## \#745 Posted by: Ackmaniac Posted at: 2018-06-13T23:32:15.060Z Reads: 168

```
Just released a new Version 1.106 with some nice new features.

There is a new magic button in the main screen
![image|273x500](upload://ihATBVlQurLrEKPEsH184pM22bx.png)

When you press that one you come to a new screen
![image|273x499](upload://y8HCo9csOEgjYlyFKfHrwMWvA5E.jpg)
If you don't like that screen you can go back to the previous by pressing the button on the bottom right again.

If you like it you will see that the data comes in a new dress with reduced and easier to consume data for the lazy user.
At the same time your path will be tracked while you ride and be visible by a blue line on the map.
you can change the map layout by a long press on the map and by that it switches to "satellite view", then next to the "satellite view with street names" and next to the "drawing map" where you can try to paint pictures by riding around in the world. Just give it a try.

It extends the path every 10 meters. And if you want to drag the map around and don't want to be disturbed by automatically going to your current position you can click the map once so that the map stays where you are. If you want to activate it again press the compass button on the top right of the map.

To change modes you need to go back to the previous screen and press the mode box. But i am open for ideas where to add that button at this screen.

This is the first roll out so please let me know if you have trouble.

If you like it [Donations](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=GJ59FXYPUQHUY) are always welcome.
And if you hate it but still love to give donations then here is your chance.
```

---
## \#746 Posted by: SeanHacker Posted at: 2018-06-14T02:02:36.242Z Reads: 162

```
Only thing I can thing of after the UI changes (which I love dude! Thanks!) is landscape for all. Thanks as always dude!!! ;)

I use an old Galaxy S6 because none of my Oreo running phones work with my old modules. But it works because I have a ton of old android phones. This is why I want landscape dude. I use this app as my speedometer and everything else. ;)

https://www.youtube.com/watch?v=ZNibZaew2kM&feature=youtu.be

https://youtu.be/zWDv1FNzFjw
```

---
## \#747 Posted by: ulangreg Posted at: 2018-06-14T02:09:29.577Z Reads: 160

```
[quote="Ackmaniac, post:745, topic:20888"]
time your path will be tracked while you ride and be visible by a blue line on the map.
you can chan
[/quote]

Love your work! I donated for your amazing progress. Not a huge issue but, For some reason on my google pixel 2XL battery outside board.![Screenshot_20180613-215854|250x500](upload://l6wDdchkUJkONPNnfcDwQrYDxjT.png)
```

---
## \#748 Posted by: Ackmaniac Posted at: 2018-06-14T06:44:28.659Z Reads: 156

```
Oh need to fix that. But no time today.
Does the map work for you. Seems that it only works on my device. There is always something.
```

---
## \#749 Posted by: rey8801 Posted at: 2018-06-14T07:38:10.050Z Reads: 159

```
Tested. It seems all fine except I can't see the map. Thx @Ackmaniac. 
![vescmonitor|281x500](upload://cGHNH7xjRkxCcEbooVXW5zLZpJb.png)
```

---
## \#750 Posted by: ROFEN13 Posted at: 2018-06-14T10:05:13.064Z Reads: 154

```
No map for me as well. Also, the distance is all in km on that screen, but miles on main. I didnt see an option to change units on the new AWESOME screen. 
BTW, i love it!
```

---
## \#752 Posted by: Ackmaniac Posted at: 2018-06-14T19:46:55.618Z Reads: 150

```
Just released an ew Veriosn 1.108 which should fix the mentioned problems. Please let me know if the map is visible now.
```

---
## \#753 Posted by: MartyMcFly88 Posted at: 2018-06-14T20:29:27.189Z Reads: 149

```
got the update, tested at home .. still no map although i have a gps fix. that sounded a bit harsh...
Just wanted to let you know, I love the app the way it is :)
```

---
## \#754 Posted by: Ackmaniac Posted at: 2018-06-14T21:41:19.145Z Reads: 150

```
Just released version 1.109. hopefully the map works this time. F***ing google api's
```

---
## \#755 Posted by: wafflejock Posted at: 2018-06-14T22:02:49.103Z Reads: 154

```
Seriously unreal how such a massive engineering company can do such a piss poor job of maintaining their documentation, at least back when microsoft was relevant enough for me to hate on them they had their sh!t together with MSDN.  Trying to find the right version of an API from google that is going to be supported for more than 6 months or doesn't already have an alternative API suggestion is impossible.
```

---
## \#756 Posted by: Ackmaniac Posted at: 2018-06-14T22:04:54.461Z Reads: 154

```
I can get it working on my develop version easily. But getting a released version that works is hard. Because there is no strait forward  instruction that tells you what to do. And in 2 days they will change the api again.
BUt let me know if it works this time if with version 1.109
```

---
## \#757 Posted by: MartyMcFly88 Posted at: 2018-06-14T22:47:31.617Z Reads: 151

```
Looking good :) got a map and dott where I am.. Will go for a Linie tomorrow ;)
```

---
## \#758 Posted by: Ackmaniac Posted at: 2018-06-14T22:49:00.928Z Reads: 152

```
Awesome. Now I know what needs to be done to get it released with the app. Sad that in 2 years when I need it again for another app everything changed for sure.
```

---
## \#759 Posted by: Thunkar Posted at: 2018-06-14T23:32:12.089Z Reads: 157

```
No changes, tried all versions since last comment (currently at 1.110). I'm going to try with another Bluetooth module just in case, thanks anyway!
```

---
## \#760 Posted by: SeanHacker Posted at: 2018-06-14T23:36:35.787Z Reads: 162

```
Map is working now. Good job dude. I'll give it a test run later after work. Thanks!!!
```

---
## \#761 Posted by: rey8801 Posted at: 2018-06-15T05:02:46.497Z Reads: 165

```
Yes map is working now. Maybe I am wrong but how many maps options do we have? Because of I long press on the map field I get the satellite one, then the same one with the name of the streets, then one that doesn't work with white background and the last one with a blue background and the name of the street. I do not know whether we should have 3 options then they all work plus we have one white screen left. Or 5hey should be 4 and 1 doesn't work. Not a big deal, I just wanted to let you know. Thanks!
```

---
## \#762 Posted by: Ackmaniac Posted at: 2018-06-15T06:33:55.589Z Reads: 158

```
The white one is the "drawing mode" or "artist mode". It's also usefull if you want to take a Screenshot to share it here but don't want to show where you live exactly.
```

---
## \#763 Posted by: rey8801 Posted at: 2018-06-15T07:07:28.743Z Reads: 154

```
Perfect! Thx man...
```

---
## \#764 Posted by: guyguy Posted at: 2018-06-15T13:45:28.428Z Reads: 156

```
Just got a firmware update on my galaxy s-7 and can't find my board on BT scan. It was visible and I was able to connect on an older version of the app I had on an old tablet.
```

---
## \#765 Posted by: rey8801 Posted at: 2018-06-15T13:53:22.555Z Reads: 153

```
Maybe you update to Oreo on your phone. Could you check it? With Oreo old clone HM-10 modules won't work anymore. Here is when we talk about it and you can see how to update the firmware on your module. Otherwise I have some modules plug in that I can send it  https://www.electric-skateboard.builders/t/esk8-flea-market-eu-ww-small-cheap-parts-hm-10-bluetooth-android-oreo-compatible-volt-meter-3dprinting/57463?u=rey8801
```

---
## \#766 Posted by: skatardude10 Posted at: 2018-06-15T13:57:18.075Z Reads: 150

```
The HM-10 I got from BKB works great with my Oreo device. Maybe it came pre-loaded with compatible firmware?
```

---
## \#767 Posted by: rey8801 Posted at: 2018-06-15T14:02:49.616Z Reads: 153

```
How does it show up on your phone? I mean the name of the BLE module
```

---
## \#768 Posted by: skatardude10 Posted at: 2018-06-15T14:05:34.049Z Reads: 153

```
I can't remember since I renamed it, but it was "MLT-Bsomethingnumber" or something along those lines.
```

---
## \#769 Posted by: rey8801 Posted at: 2018-06-15T14:07:55.189Z Reads: 150

```
yes MLT_BT05 is a clone that usually wokrs. I also use that one with Oreo.
```

---
## \#770 Posted by: skatardude10 Posted at: 2018-06-15T14:15:14.499Z Reads: 152

```
Ah, nice, yep that's it.
```

---
## \#771 Posted by: rey8801 Posted at: 2018-06-15T14:16:56.356Z Reads: 153

```
I read so many forum on this modules tha now I cna recognize them by eyes :joy:
```

---
## \#772 Posted by: xBRAZILx Posted at: 2018-06-15T14:21:24.600Z Reads: 154

```
just one question, how did you change your bluetooth module name?
```

---
## \#773 Posted by: skatardude10 Posted at: 2018-06-15T14:22:35.128Z Reads: 154

```
In the ackmaniac app, connect to your module, then go to settings and change board name. From then on when you connect it doesn't show the module name, it will show the board name instead.
```

---
## \#774 Posted by: rey8801 Posted at: 2018-06-15T14:23:34.617Z Reads: 162

```
In my case it shows both the board name and the module name.

Edit
![vescmonitor|281x500](upload://zx2bLdf5GQhVNnEJs97I11rmmnL.jpg)
```

---
## \#775 Posted by: skatardude10 Posted at: 2018-06-15T14:24:52.549Z Reads: 161

```
You got me curious now, I'll have to check when I get home if mine does the same... I only remember seeing the board name in big bold red letters off the top of my head... Maybe I'm just not paying attention to detail 😎
```

---
## \#776 Posted by: skatardude10 Posted at: 2018-06-15T14:25:45.057Z Reads: 165

```
Huh! Yeah pretty sure mine doesn't do that... Hmmm
```

---
## \#777 Posted by: rey8801 Posted at: 2018-06-15T14:26:20.520Z Reads: 171

```
to answer your question you actually have to send an AT command to realyl change the name of the module. At least as far as I know.
```

---
## \#778 Posted by: 91stantheman Posted at: 2018-06-15T17:11:21.402Z Reads: 169

```
I guess I'm the only one who is having issues as of right now. The app closes when I try to open the map, then every time after that it closes when I just select the board... I have a up to date galaxy S9+
```

---
## \#779 Posted by: Ackmaniac Posted at: 2018-06-15T17:36:54.132Z Reads: 178

```
Did you give the app all the permissions? And maybe you have GPS disabled which might cause the problem.
```

---
## \#780 Posted by: 91stantheman Posted at: 2018-06-15T18:46:39.417Z Reads: 184

```
![Screenshot_20180615-134411_Package%20installer|243x500](upload://1IX9Yeb4otdc6JWyf4iCbMYrFPK.jpg)

No it's all allowed and GPS turned on.
```

---
## \#781 Posted by: 91stantheman Posted at: 2018-06-15T19:18:58.899Z Reads: 164

```
Um, never mind. It just randomly started working. Thank you for the quick reply hahaha.
```

---
## \#782 Posted by: Ackmaniac Posted at: 2018-06-15T19:37:14.234Z Reads: 169

```
No problem. Sometimes android acts strange. Issue is that each manufacturer has their own add-ons which can cause trouble.
```

---
## \#783 Posted by: Sebike Posted at: 2018-06-15T21:26:04.970Z Reads: 169

```
Same thing happened to me on the first run. Rebooted the phone and now it works as it should.
```

---
## \#784 Posted by: mmaner Posted at: 2018-06-15T21:58:15.682Z Reads: 173

```
@Ackmaniac  can you define the throttle curve types?  Me & @Sender are trying to figure it out.  If you define these and the differences I would be grateful.  thanks

    exponential = (of an increase) becoming more and more rapid.
    expo-natual = ???
    natural = ???
    polynomial = consisting of several terms
```

---
## \#785 Posted by: Ackmaniac Posted at: 2018-06-15T22:13:34.518Z Reads: 170

```
Just have a look at the graph in the app or in the Ackmaniac-tool. You can see how the throttle curve changes. The X axis stands for the amount of throttle in percent and the y axis for the amount of power in percent.
```

---
## \#786 Posted by: Thunkar Posted at: 2018-06-17T09:55:22.744Z Reads: 173

```
@Ackmaniac turns out my bluetooth module was fried :weary: . A new one arrived and worked flawlessly, I feel kinda stupid now. Anyways, thanks a lot! A donation is coming your way, the new update is amazing! :wink:
```

---
## \#787 Posted by: rey8801 Posted at: 2018-06-18T08:25:56.052Z Reads: 172

```
https://www.electric-skateboard.builders/t/esk8-flea-market-eu-ww-small-cheap-parts-hm-10-bluetooth-android-oreo-compatible-volt-meter-3dprinting/57463/22?u=rey8801
```

---
## \#788 Posted by: skatardude10 Posted at: 2018-06-19T06:18:20.342Z Reads: 175

```
I made a post in the ESC Tool thread thinking the problem may stem from there, but after doing some troubleshooting, I think my issue stems from the app not changing control modes like it should be. 

Regardless of control mode type, it always reverts to "Disabled", with the control mode defaulting to what I originally flashed in ESC Tool,  meaning I can't change from Current to Current No Reverse or PID No Acceleration: 

![Screenshot_20180619-001402_ESC%20Monitor|243x500](upload://skalhhQOINmLa0tCdovsCzzkyNm.jpg)![Screenshot_20180619-001415_ESC%20Monitor|243x500](upload://uwt1T8GxpqHdCmTL7zYPOqztEwQ.jpg)![Screenshot_20180619-001338_Package%20installer|243x500](upload://knrGihQ55moA3WA2VwTI8KrtGjF.jpg)
```

---
## \#789 Posted by: rey8801 Posted at: 2018-06-20T05:29:19.359Z Reads: 165

```
https://www.electric-skateboard.builders/t/esk8-flea-market-eu-ww-small-cheap-parts-hm-10-bluetooth-android-oreo-compatible-volt-meter-3dprinting/57463/23?u=rey8801
```

---
## \#790 Posted by: Teitanblood Posted at: 2018-06-20T06:23:18.020Z Reads: 161

```
I discovered yesterday the new black and white screen by mistake. It looks great! However, it made the app crash instantly and now I'm stuck in a crash loop anytime I try to connect to my board... Hope it will come back to normal operation at the next update
```

---
## \#791 Posted by: Ackmaniac Posted at: 2018-06-20T06:31:57.112Z Reads: 164

```
Just restart your phone. Another user had the same issue and could fix it by that.
```

---
## \#792 Posted by: Teitanblood Posted at: 2018-06-20T07:37:22.191Z Reads: 161

```
Yes, I've already tried without success...
I guess it's on my side though so I will just wait
```

---
## \#793 Posted by: Ackmaniac Posted at: 2018-06-20T07:59:03.848Z Reads: 162

```
Does the app crash or go back to the main screen?
```

---
## \#794 Posted by: Teitanblood Posted at: 2018-06-20T08:08:33.464Z Reads: 159

```
No complete cash. The app can scan for the different devices but crashes instantly if I connect to my board.
```

---
## \#795 Posted by: Ackmaniac Posted at: 2018-06-20T08:31:29.448Z Reads: 164

```
Then your smartphne asks you to send the error report which you hopefully did.
```

---
## \#796 Posted by: Teitanblood Posted at: 2018-06-20T09:07:38.332Z Reads: 170

```
No I didn't I will do it as soon as possible
```

---
## \#797 Posted by: skatardude10 Posted at: 2018-06-21T01:46:05.485Z Reads: 195

```
A few weeks ago I did my best to match remaining amp hours linearly with the discharge curve of my 25r cells under ~20A load (trying my best to account for ~3v sag that's typical on my setup to never drop below 28v near 0%), and base percentages off of that. With the default curve, I'd drop to 50-60% relatively quick, always feel like I didn't have much battery left, but always go a lot further than expected.

With these settings I've pretty much noticed a linear drop in percentage as I ride, that nearly matches my battery packs LCD perfectly- A nice added bonus. For anyone interested, let me know what you think:

![Screenshot_20180620-194133_ESC%20Monitor|243x500](upload://wAstiBMsEkOT1K73OAEV1Sw13jX.jpg)
```

---
## \#798 Posted by: flyingox Posted at: 2018-06-21T21:08:33.043Z Reads: 191

```
My esc monitor app stopped working over a month ago, was working with dual Vesc6 v3.31 for a few months then stopped possibly due to a mobile update.   Esc montior version 1.110 connects to Bluetooth module but doesn't talk with the Vesc6 ESC.

Cabling is correct as it was working before, no hardware changes.  App is running on Android 7.1 Nexus 6.  BTW also tried Nexus 7 6.01 same problem.  Data and GPS tried baud rate 9600 and 115000.  

Recently tried upgrading to Metr pro which works with their owned app but not with Esc monitor.

Rebooted the phone, cleared cache, re-installed and knocked my head against the wall for several hours.  As one app works and not the other suggests an issue with the app.

When I open Esc montior and thumb over the motor setting this produces a message esc not connected.

Would be great to hear if someone has the solution.
```

---
## \#799 Posted by: Ackmaniac Posted at: 2018-06-21T21:35:36.106Z Reads: 196

```
Maybe try it with the latest firmware version. And check if you accidently enabled connect via CAN in the app. If yes then disable it and give it a try.
```

---
## \#800 Posted by: flyingox Posted at: 2018-06-28T21:05:15.061Z Reads: 190

```
Finally I got this to work with ACKMANIAC-ESC tool version 3.102,  I had to compiled a version for Ubuntu and that wasn't straight forward. 

At this point using the BT05 Bluetooth client module Ackmaniac ESC monitor works and if I use the Metr-pro BT module and can use the metr Pro but not both at the same time which is a shame.
```

---
## \#801 Posted by: secupol Posted at: 2018-06-30T05:12:35.490Z Reads: 191

```
There was a problem after updating to V1.110 version.
The connection is made but does not receive any data at all.
My smartphone is Galaxy Note 4 and Android version is 6.01.
The firmware of vesc 6 is 3.38.
It worked before the app was updated.
Could you check the problem?
```

---
## \#802 Posted by: Exigent Posted at: 2018-07-01T01:30:06.797Z Reads: 191

```
Two Questions:

1) Can you list an approximate **minimum** Android version number on which this should work? I use an older "I don't care what happens to it" phone when on my board and it's at Android 4.1, and when I go to the play store to download it, it doesn't show up...indicating it's "incompatible". For example: Are you assuming everyone is using an Android 6 phone or better?

2) If you don't already do this, please consider providing a READ-ONLY or "safe" mode so folks can't accidentally screw-up board settings when they're exploring the functionality of your app.
```

---
## \#803 Posted by: SeanHacker Posted at: 2018-07-01T14:03:20.678Z Reads: 183

```
What phone are you using? I might be able to help get you up to date with a newer android version in order to get this working for you if you'd like.
```

---
## \#804 Posted by: Ackmaniac Posted at: 2018-07-01T14:05:14.201Z Reads: 179

```
Version 5.0 is the minimum.
```

---
## \#805 Posted by: Exigent Posted at: 2018-07-01T21:14:19.604Z Reads: 183

```
[quote="SeanHacker, post:803, topic:20888"]
What phone are you using? I
[/quote]
Thoughts and help would be appreciated.
My “I don’t care what happens to it” phone is an LG D-500 "Optimus F6"
Currently running Android 4.1.2, kernel 3.4.0, version D50010h
It's taken some very hard knocks but keeps on ticking. Would be a pity to accidentally brick it with failed jailbreaking, but looks like I may have to try. Or, I could go looking for a refurb phone at higher Android level and justify as a "cost of skateboarding"...sort of?

EDIT to add: 
SeanHacker--Just realized...I don't want to hijack this thread. Please PM if replying on uplifting the LG phone.
```

---
## \#806 Posted by: Exigent Posted at: 2018-07-01T21:15:14.995Z Reads: 177

```
Thank you. Much appreciated info.
```

---
## \#807 Posted by: Jc06505n Posted at: 2018-07-01T21:16:04.595Z Reads: 183

```
Thinking of buying an android device for using the app, anyone have any recommendations ? I really won’t be using any Cellular Features and at most I’ll only be using the app for it
```

---
## \#808 Posted by: L3chef Posted at: 2018-07-02T11:25:09.959Z Reads: 177

```
So I tried to search for this but didn't find the answer.

1 module is enough to change different modes on dual setup right?
```

---
## \#809 Posted by: rey8801 Posted at: 2018-07-02T11:27:25.990Z Reads: 177

```
Yes it is. If the bluetooth module is connected to the master you can also adjust the throttle/braking curve. While only the different mode if you are connected to the slave VESC.
```

---
## \#810 Posted by: L3chef Posted at: 2018-07-02T11:34:38.005Z Reads: 177

```
Thanks! I haven't messed around with throttle brake curve yet. Would you recommend adjusting it ?
```

---
## \#811 Posted by: rey8801 Posted at: 2018-07-02T11:38:33.241Z Reads: 187

```
Depends if you feel your accelleration and braking not smooth enough it definitely helps a lot. I do use both of them.
```

---
## \#812 Posted by: L3chef Posted at: 2018-07-02T11:41:31.187Z Reads: 177

```
Ok. I will check it out someday
```

---
## \#813 Posted by: Ackmaniac Posted at: 2018-07-02T14:33:43.357Z Reads: 187

```
When the ble module is connected to the slave then you can connect with the app to the master via CAN and change modes the same way as if you are connected to the master directly.
```

---
## \#814 Posted by: darkydawson Posted at: 2018-07-06T23:21:18.948Z Reads: 185

```
I just got a new Nokia 7 plus and cant connect it to board. Android 8.1(Can see board in BT settings, not in app). The same board (Raptor 2) works on a samsung A9 pro....
```

---
## \#815 Posted by: sayekim Posted at: 2018-07-06T23:27:08.302Z Reads: 188

```
[quote="darkydawson, post:814, topic:20888"]
I just got a new Nokia
[/quote]

Well I don’t hear that very often these days.
```

---
## \#816 Posted by: PartyPoison Posted at: 2018-07-07T01:02:57.579Z Reads: 179

```
How can i update my 6.6 with ackmaniac fw? Im having i/O error when uploading, vesc is ok with current fw (vesc fw 3.x),
```

---
## \#817 Posted by: Kraz3Sk8r Posted at: 2018-07-10T04:53:46.047Z Reads: 171

```
@Ackmaniac:  I was using your app on three different boards along with your VESC tool on Focboxes, testing on several rides, but now it crashes, giving the notice "Unforunately, ESC Monitor has stopped."  It doesn't work at all on any board.  Do you know how I can fix it?  I have rebooted my phone, plus have reinstalled the app and neither improved it.  Sometimes I can get the operating screen to come up,  but even then it doesn't read the data from the Focbox.  Any help would be greatly appreciated.
```

---
## \#818 Posted by: skatardude10 Posted at: 2018-07-11T15:03:48.962Z Reads: 181

```
Did your telephone recently update to a newer Android version by chance?
```

---
## \#819 Posted by: skatardude10 Posted at: 2018-07-11T15:06:33.106Z Reads: 187

```
I have a feature request: it would be awesome to be able to adjust positive and negative ramping time per mode in the app.

I changed my ramping time to 0.1s to compliment more aggressive riding, but it would be great to be able to change this to say 0.5s or 1s for the chill/beginner modes I've set up.
```

---
## \#820 Posted by: Kraz3Sk8r Posted at: 2018-07-11T18:02:52.903Z Reads: 184

```
No, no new Android version.  Thanks for thinking on it, though.  :slightly_smiling_face:
```

---
## \#821 Posted by: Kraz3Sk8r Posted at: 2018-07-13T20:55:13.557Z Reads: 182

```
Does anyone else have any ideas why the app doesn't work?  Now it works, connects to the boards, but doesn't show data other than zeros, even if I reboot.  @Ackmaniac?
```

---
## \#822 Posted by: rey8801 Posted at: 2018-07-14T13:03:46.637Z Reads: 183

```
Hi, one question if possible. I now have the bluetooth module connecte to the slave VESC because I built a FireFly remote that needs the UART port too. I enable send over CAN "0" in the app and I can change the setting ecc... the only thing that doesn't write on the master is the throttle/brake curve adjustments. I don't remember whether it is suppose to do it now? Not a big deal because I use the TCP connection to fix it, but just out of curiosity.
Thx!
```

---
## \#823 Posted by: Ackmaniac Posted at: 2018-07-14T14:50:59.165Z Reads: 186

```
It is important to deactivate "Send status over CAN" at the master. Please check that.
```

---
## \#824 Posted by: rey8801 Posted at: 2018-07-14T14:59:18.908Z Reads: 186

```
You are totally right, it was on. I do not remember that I changed it. Now it works! Perfect, thanks!
```

---
## \#825 Posted by: koralle Posted at: 2018-07-15T14:57:04.051Z Reads: 196

```
Is there a reason the app shouldn't work with vedders new nrf51 Bluetooth dongle firmware?
```

---
## \#826 Posted by: Ackmaniac Posted at: 2018-07-15T15:59:43.594Z Reads: 196

```
No idea. Never gave it a try.
```

---
## \#827 Posted by: koralle Posted at: 2018-07-15T16:06:06.028Z Reads: 191

```
I'll report back.
```

---
## \#828 Posted by: L3chef Posted at: 2018-07-16T20:57:36.575Z Reads: 193

```
[quote="Ackmaniac, post:1, topic:20888"]
If it is connected to the master and you use a PPM controller then you need to activate PPM+UART.
[/quote]
@ackmaniac
PPM+UART on master only or on both vesc's if running dual?
```

---
## \#829 Posted by: rey8801 Posted at: 2018-07-16T21:10:41.414Z Reads: 188

```
Only for master :wink:
```

---
## \#830 Posted by: L3chef Posted at: 2018-07-16T21:11:27.046Z Reads: 184

```
yeah I just figured it out. I´m an idiot :stuck_out_tongue:
```

---
## \#831 Posted by: darkydawson Posted at: 2018-07-17T09:23:46.014Z Reads: 188

```
@ackmaniac

I can't connect to raptor 2 anymore on Nokia 7 plus(android 8.1) can see device in bt settings but not in app?
```

---
## \#832 Posted by: L3chef Posted at: 2018-07-17T10:52:02.564Z Reads: 187

```
My bluetooth module works only on the slave vesc. What could be the issues why it's not working on my master?
Connected to master it says "no esc connected"
(Focboxes)
```

---
## \#833 Posted by: Ackmaniac Posted at: 2018-07-17T10:53:45.666Z Reads: 186

```
Did you set the same UART Baudrate? And did you choose PPM+UART as control mode.
```

---
## \#834 Posted by: L3chef Posted at: 2018-07-17T10:55:40.332Z Reads: 184

```
Yes I did. But going to double check it now when I have the enclosure off. Una momento
```

---
## \#835 Posted by: L3chef Posted at: 2018-07-17T11:18:21.437Z Reads: 187

```
Lol I had accidently pressed "write motor config" instead of write app config.. All good now
```

---
## \#836 Posted by: L3chef Posted at: 2018-07-25T21:14:39.815Z Reads: 179

```
When I change a mode for dual setup, only master vesc is changed. Bluetooth module connected to master..
What am I doing wrong?
```

---
## \#837 Posted by: Morxy49 Posted at: 2018-07-30T19:09:24.120Z Reads: 180

```
I'm having issues connecting to my skateboard. I have a bluetooth module on my board but i don't think the app is able to find it. There's only a "Unknown device" which i can't connect to.

Am i using the wrong Bluetooth module? This is what i have: https://eskating.eu/product/bluetooth-uart-module-for-electric-skateboards-ios-android-metr-app/
```

---
## \#838 Posted by: Skifree Posted at: 2018-07-30T20:40:16.474Z Reads: 180

```
From the picture, it looks like a clone perhaps? It might not work with Android 8.

This [link](http://blog.yavilevich.com/2016/12/hm-10-or-cc41-a-module-automatic-arduino-ble-module-identification/) gives a pretty good idea of the original and the clone. In the image on eskating.eu there is only one capacitor, I think that the HM-10's without the second are clones. but I'm definitely no expert.
```

---
## \#839 Posted by: Luuke Posted at: 2018-07-31T07:24:37.720Z Reads: 174

```
SInce I want to update my phone to Android 8...
Could you please link a correct module?
Right now I am using a cheap HM10 clone, which is great!
```

---
## \#840 Posted by: rey8801 Posted at: 2018-07-31T07:29:55.880Z Reads: 166

```
How does you module show up on your phone?
Based on that I can tell you of it will work or you need another one or update the firmware
```

---
## \#841 Posted by: Luuke Posted at: 2018-07-31T12:10:33.264Z Reads: 163

```
[quote="rey8801, post:840, topic:20888"]
does you module show up on your phone?
Based on that I can tell you of it will wo
[/quote]
How?? I don't know how to answer this question.
WHat are the possible options?
```

---
## \#842 Posted by: rey8801 Posted at: 2018-07-31T12:14:24.340Z Reads: 158

```
When you open the app before select your board you should see the name of the module. Like Hm10. BLT5 ecc...
```

---
## \#843 Posted by: Quezacotl Posted at: 2018-07-31T13:36:39.612Z Reads: 163

```
Strange. I just updated to Oreo(EMUI8.0) on my Honor 8, and it still connects. No problem at all. The BT module was bought about a year ago. Maybe there is some legacy support afterall.
```

---
## \#844 Posted by: Narnash Posted at: 2018-07-31T13:51:52.378Z Reads: 162

```
That's a known work arround how to get even non offical firmware HM10 modules working when you had a connected HM10 on your old Android version and update than to Oreo.
However it's likely that if you ever have to "forget" your module let's say because you have dropout problems and try the old reconnect fix that you can't find your module again.
```

---
## \#845 Posted by: rey8801 Posted at: 2018-07-31T13:59:13.983Z Reads: 166

```
Some HM10 clones are compatible. I have tried almost all of them and some work and some not. Although I could flash the original HM10 for aware on those ones and make them work as HM10.
```

---
## \#846 Posted by: Quezacotl Posted at: 2018-07-31T14:03:39.575Z Reads: 167

```
Except i wiped the phone completely before installing Oreo :smiley:
```

---
## \#847 Posted by: rey8801 Posted at: 2018-07-31T14:35:05.941Z Reads: 170

```
That's doesn't matter. Is the module that is compatible or not. Anyhow of yours works than better like that. I also use and sell only clones so far. No problem at all, they do their job just fine.
```

---
## \#848 Posted by: Luuke Posted at: 2018-08-02T19:37:39.951Z Reads: 166

```
![41%20-%20Kopie|690x180](upload://nnQQWUouU2y5zmgRP12uFIMOo5v.png)
It looks like that. So will it work with Android 8.0?
```

---
## \#849 Posted by: AutoItKing Posted at: 2018-08-02T20:56:44.906Z Reads: 169

```
@Ackmaniac, it looks like BV has made a change in the firmware that may break your app:

> VESC-Tool: FW 3.40 support, added VESC ID to mc_values.
> BLDC: Added motor controller ID to COMM_GET_VALUES.

Just an FYI for those not using Ack's custom firmware.
```

---
## \#850 Posted by: Titoxd10001 Posted at: 2018-08-02T21:34:27.483Z Reads: 165

```
Would be cool if app would reconnect automatically when signal is regained. Like if i need to step away from the board and I come back with out fail the app is frozen and have to close and search for Bluetooth device again. 

Also not sure if its just my phone but once I connect to a Bluetooth device I get two of those notification boxes. One says speed, battery%.... The other just says "Esc monitor is running." The latter doesn't close when I close the app. So I have to force stop to completely close the app. Anyone have this issue.
```

---
## \#851 Posted by: AutoItKing Posted at: 2018-08-02T22:05:57.960Z Reads: 154

```
Yes, I have the same issue. I have to force stop the app for it to actually close. But you gotta remember this is just one guy working on this app, and I am more than happy with what he has given us. For free.
```

---
## \#852 Posted by: Titoxd10001 Posted at: 2018-08-02T22:26:33.659Z Reads: 151

```
Don't get me wrong I really like this app and I've donated funds to ackmaniac. I like that the app brings a whole new dynamic trying to bring the wh/min down and also the heat by making the mechanical side more efficient. The reason I point out the app issues so hopefully it could be improved even more
```

---
## \#853 Posted by: rey8801 Posted at: 2018-08-02T22:33:21.902Z Reads: 153

```
Yep it should
```

---
## \#854 Posted by: louwii Posted at: 2018-08-03T01:50:58.409Z Reads: 160

```
I have a HM-10 showing up as a BT-05 as well in the app.
It was working fine on my Nexus 5 running Android 7 (Lineage 14).
However, when I updated to Lineage 15 (Android 8), it wasn't showing up anymore in the app.
It's not showing up either on my new phone (Xiaomi Mi Mix 2) running Android 8.

I understand that this is because of the cheap HM-10. But come-on, they work fine on iOS and older Android versions. WTF Google.
```

---
## \#855 Posted by: rey8801 Posted at: 2018-08-03T05:46:25.706Z Reads: 162

```
The problem that they just use different firmware. You can update  the HM10 firmware on your clone module. On the Arduino forum there is a tutorial that is pasted in this thread too. Just search for it. I know it sucks. Anyhow I have bt05 modules that work  depends how old it is. To be sure of future compatibility I advice to update the firmware or buy module with the same breakout board of the HM10 module. You pay them a bit more but you are sure they work. I have plug and play module fully compatible to sell for cheap. You can find it in the flea market thread. AFAIK those are the options available up to know for Android based devices.
```

---
## \#856 Posted by: RyuX Posted at: 2018-08-06T18:02:12.519Z Reads: 164

```
@Ackmaniac
Hey.. is there already a version for Android 8.0 available ? The App can not find my bluetooth module anymore since I changed to Android 8.
I heard that Android Oreo does not have BLE Discovery anymore. I would be very glad if I could use your app again some time soon.. Thanks :slight_smile:
```

---
## \#857 Posted by: AutoItKing Posted at: 2018-08-06T20:04:37.376Z Reads: 158

```
The problem isn't the app, it's how Android handles BLE connections, specifically to knockoff BLE modules. Before 8 not much attention was given to checking for a proper scan response so clone or knockoff BLE modules worked fine. Android 8 fixed this bug.

You can read more about it here: https://blog.yavilevich.com/2018/04/should-you-throw-away-your-cc41-hm-10-clones-now-that-android-8-is-here/ (also posted above by @Pimousse).
```

---
## \#858 Posted by: rey8801 Posted at: 2018-08-06T20:22:49.653Z Reads: 155

```
Is not the app but most likely your bluetooth module. It is probably a clone and not all the clone works. Search in the thread is posted how to flash the ordinal hm10 firmware and it will work again. Otherwise buy a new module :wink:
```

---
## \#859 Posted by: RyuX Posted at: 2018-08-07T03:20:50.246Z Reads: 157

```
Its a original metr.at bluetooth module. No knockoff or clone!!!
```

---
## \#860 Posted by: Pimousse Posted at: 2018-08-07T06:11:12.023Z Reads: 157

```
Metr modules (old ones, not Metr Pro) are based on HM11 clone module.
So same issue.
```

---
## \#861 Posted by: rey8801 Posted at: 2018-08-07T07:38:57.485Z Reads: 156

```
As @Pimoussesaid. You oiad for the nice app but the module was a old clone version
```

---
## \#862 Posted by: Maxid Posted at: 2018-08-07T07:51:37.641Z Reads: 162

```
https://www.electric-skateboard.builders/t/configuration-and-telemetry-for-vesc-ios-android/13483/69?u=maxid
This was in 2016 already! You do have a clone!
```

---
## \#863 Posted by: RyuX Posted at: 2018-08-07T13:41:44.488Z Reads: 158

```
What a ripoff :frowning:
```

---
## \#864 Posted by: gigoy Posted at: 2018-08-13T06:35:12.544Z Reads: 164

```
If I swap batteries from 10s to 12s, is it possible to do that and just create a new mode with different motor/battery max/min and a different battery profile using the app? Or is connecting the VESC to the PC and doing the process again "a-must"?

EDIT: I'm using Ack app by the way
```

---
## \#865 Posted by: Ackmaniac Posted at: 2018-08-13T07:36:16.341Z Reads: 162

```
You can do that by the app. Just simply create another mode. Only thing you have to do additionally is to change the number of cells in the app. That can't be done by switching a mode.
```

---
## \#866 Posted by: L3chef Posted at: 2018-08-14T17:21:47.566Z Reads: 158

```
Can't figure out how to change modes on dual setup. 
Click on the mode I want to change to and only master is affected.
What am I doing wrong?
```

---
## \#867 Posted by: SeanHacker Posted at: 2018-08-14T17:26:02.540Z Reads: 154

```
Afterwards you need to check the box "Connect by can" and also select the mode you want. Then you can uncheck that box and be on your way.
```

---
## \#868 Posted by: L3chef Posted at: 2018-08-14T17:26:42.709Z Reads: 157

```
Perfect! Thanks mate
```

---
## \#869 Posted by: Ackmaniac Posted at: 2018-08-14T17:41:52.190Z Reads: 160

```
Guess you have "send status via CAN" enabled at the master. It only should be enabled at the slave.
```

---
## \#870 Posted by: L3chef Posted at: 2018-08-14T18:27:25.018Z Reads: 159

```
Thanks. I'll check it out
```

---
## \#871 Posted by: Sender Posted at: 2018-08-18T02:28:27.303Z Reads: 164

```
So I have my module set up to my slave and I have "Connect Can to ID 0" checked. (Its on the slave because I am using a firefly remote that steals my Master's UART port.)

To change modes, do I just do it andthe way I have it set up will change it changes for both? 

Or do I need to set the desired mode, then uncheck the box and then select the same mode again to make sure the other VESC had the same settings?  

Damn, that sounds convoluted.

In other words if my BT module is on my slave, how do I get it to affect both VESCS?  Or does it do it automatically?

I have read some conflicting things,  thank you.
```

---
## \#872 Posted by: rey8801 Posted at: 2018-08-18T05:20:39.639Z Reads: 160

```
It does work in the same way as the module on the master. Just selected in the app connect by CAN to 0 and in the VESC tool disable "send status over CAN" at the master level.
```

---
## \#873 Posted by: Sender Posted at: 2018-08-18T11:51:11.439Z Reads: 161

```
Awesome, good to hear. Thank you!
```

---
## \#874 Posted by: Ackmaniac Posted at: 2018-08-18T11:57:06.976Z Reads: 162

```
Perfect answer
```

---
## \#875 Posted by: rey8801 Posted at: 2018-08-18T12:13:30.449Z Reads: 161

```
I learnt from my mistakes :sweat_smile:
```

---
## \#876 Posted by: osbor Posted at: 2018-08-19T04:23:20.079Z Reads: 158

```
Can anyone link to where to buy a 100% real hm10 that is confirmed to work on 8.1?
```

---
## \#877 Posted by: epster Posted at: 2018-08-19T11:55:53.114Z Reads: 160

```
Hey guys so I was trying to setup the app but i encountered an issue. When i select the module everything is fine I allowed all things it asked but when i click the setup mode the app just says it chrashed and restarts. I tried it 3 times restarting the Vesc restarting my phone (s8 with newest android software) but it just keeps chrashing. Did you guys ever encounter an issue like this? Vesc is setup works perfect so does my remote. Oh yeah btw i also changed the setting like they said on the site.

I will try to use another cellphone but i dont have one on me at the moment.
```

---
## \#878 Posted by: Ackmaniac Posted at: 2018-08-19T12:31:51.637Z Reads: 159

```
Maybe uninstall the app and install it again. When the app crashes please send the report so that i can have a look where it crashed.
```

---
## \#879 Posted by: Sebike Posted at: 2018-08-19T12:36:04.463Z Reads: 162

```
That happened to me as well after an update. Phone reboot solved the issue.

Edit. You had already tried phone restart. Sorry, my bad.
```

---
## \#881 Posted by: epster Posted at: 2018-08-19T16:18:25.928Z Reads: 164

```
I send you a chrash report with the details. But I think i am doing something wrong here. What i did to install my bluetooth module was 
1. setup the vesc to preferences 
2. attatch bluetooth module 
3. set the vesc to uart + PPM
4. Set the uart baudrate 9600
5. open the app and connect
but after step 5 it doesnt show any information it just shows a 0 everywhere and it crashes when i click the modes setup button.

Appreciate the quick replies and help guys :pray:
```

---
## \#882 Posted by: rey8801 Posted at: 2018-08-19T16:28:46.846Z Reads: 160

```
Did you give all the permessions to the app? Did you turn on the GPS? After setting modifications in the VESC tool did you press write the app configuration in the VESC tool?
```

---
## \#883 Posted by: epster Posted at: 2018-08-19T17:10:10.335Z Reads: 170

```
yup did every single thing you said. Checked everything again maybe something is set wrong in this screen

.![20180819_191308|374x500](upload://rPi6JGj8whZEkz4RmOSXUUXWh1G.jpg)
```

---
## \#884 Posted by: rey8801 Posted at: 2018-08-19T18:29:05.440Z Reads: 162

```
Which firmware are you using? is it the latest one? I have 3.102 still the latest one I guess
please post a pic of your Bluetooth wiring if possible.
```

---
## \#885 Posted by: L3chef Posted at: 2018-08-19T18:30:39.438Z Reads: 163

```
Gps and bluetooth on?
```

---
## \#886 Posted by: epster Posted at: 2018-08-19T20:45:15.103Z Reads: 161

```
yeah have everything turned on and allowed
```

---
## \#887 Posted by: epster Posted at: 2018-08-19T20:53:18.805Z Reads: 166

```
I am not really sure what you mean with firmware  do you mean the firmware of the module or the vesc. The firmware of the module I have no idea. The firmwares of the vesc are updated i have got 4.12 and 3.102 .
![20180819_225045|666x500](upload://ycfJMx7YMjl7oJLJtPcA6WujTph.jpg)
```

---
## \#888 Posted by: rey8801 Posted at: 2018-08-19T21:06:05.880Z Reads: 163

```
Yes I meant the firmware on the VESC. You have the latest so it should work. Does the app crash only when  you connect the board?
Are TX and RX crossed on you bluetooth module? Meaning TX vesc to RX HM10 and vice versa.
Did you enable send status over CAN on the slave vesc?
```

---
## \#889 Posted by: epster Posted at: 2018-08-19T21:15:11.042Z Reads: 164

```
First off thanks for the reply appreciate it. 
The app only crashes when i connect to the board and select create new setup mode every other part off the app works perfect thats the weird thing. Except that it doesn`t show data when i connect it. I dont know if it should when you load it up for the first time but when i start the app and my vesc is on and connected to my remote it shows nothing no temperatures, no amperage, no voltage nothing just all 0. 
About the TX and RX wires i have no idea what the tx and rx wires are on the HM10 devices i saw the pic on google but my device is heatshrinked and i quote its ``plug and play`` as they said so cant see where they are connected to the HM10.
About the 3rd thing you said i have no slave vesc I have 1 motor and 1 vesc so maybe i made a mistake in my settings there?
```

---
## \#890 Posted by: skatardude10 Posted at: 2018-08-19T22:22:32.266Z Reads: 159

```
I was having issues with GPS not tracking me for the past few days. Realized I turned on power saving a few days ago :man_facepalming:
```

---
## \#891 Posted by: Sender Posted at: 2018-08-19T22:29:23.979Z Reads: 159

```
So I have the BT module hooked up to the slave, "send to id 0" checked, send status over can false on master in Tool,  but I cannot change modes still.  I can get telemetry just fine.  

Just curious, I am not to worried about it.  As soon as my Benchwheel remote comes in, I will swap to that and ditch the Firefly.  This will allow me to hook up to the master and this will all be moot.  But I would like to figure it out...
```

---
## \#892 Posted by: Jc06505n Posted at: 2018-08-19T22:35:15.909Z Reads: 156

```
Aww why ditch the firefly ?
```

---
## \#893 Posted by: Sender Posted at: 2018-08-19T22:44:36.368Z Reads: 158

```
It's cool, but... don't roast me... It feels very DIY.  Like hard for me to trust.  I have had some wheel sticking issues (I have resolved mostly through some sanding) and some weird connectivity issues in places or at times (haven't pin pointed the cause yet).  

And TBH, I never use the remote telemetry.  I either use my BT module (mostly if I want more data) or a quick glance at my battery indicator on my board for approximate battery.  With 10s6p, I don't have to hound on range like the old days.  

I just want a solid connection thumb controlled remote.
```

---
## \#894 Posted by: Jc06505n Posted at: 2018-08-19T23:10:56.307Z Reads: 152

```
Ah I feel you , most likely it’s interference from traffic lights at interssections like the death-maytech remote
```

---
## \#895 Posted by: rey8801 Posted at: 2018-08-20T04:59:25.243Z Reads: 152

```
That's weird. I guess you have select PPM and UART at the master VESC for the Firefly remote and UART at the slave VESC with 9600baud. Then it should work, anyhow you can always use the TCP to connect to the VESC
```

---
## \#896 Posted by: rey8801 Posted at: 2018-08-20T05:03:06.617Z Reads: 156

```
Ah so you bought your HM10 module. I guess the connections are correct then. Try to install the app Serial Bluetooth and connect you bluetooth module to it. I make Bluetooth modules flashed with the original HM10 firmware and I use this app to quickly test which firmware they have and if the BLE connection works. Also read which name appears on the screen for your module.
```

---
## \#897 Posted by: epster Posted at: 2018-08-20T14:40:15.824Z Reads: 163

```
So i installed the app and made some screenshots hope it makes sense to you. Becuase i have no idea what the app can do :smile:. 
  ![Screenshot_20180820-163213_Serial%20Bluetooth%20Terminal|243x500](upload://bavhzosQvxWXDRQL66JuhoAf2Id.jpg)
![Screenshot_20180820-163139_Serial%20Bluetooth%20Terminal|243x500](upload://eJI9I8yF8tYEqw51Pa0HM26CLTE.jpg)

I think I am just an unlucky fellow who`s app doesn`t work. I will try it in the future after there is a new update.
```

---
## \#898 Posted by: Aeroquiv Posted at: 2018-08-24T22:52:03.967Z Reads: 144

```
Didn't find anything via search, but was wondering if it was possible to separate Max W with Max -W? I find I can cruise just fine at very low power, but I find the brakes are extremely weak as a consequence.
```

---
## \#899 Posted by: Ackmaniac Posted at: 2018-08-24T22:57:15.377Z Reads: 144

```
When you adjust max watts via the app then min watts are not affected by that. So you can have strong brakes and gentle acceleration.
```

---
## \#900 Posted by: Aeroquiv Posted at: 2018-08-24T23:13:44.848Z Reads: 146

```
Hmm, going to have to test this out further. Going to have to check some things.
```

---
## \#901 Posted by: visnu777 Posted at: 2018-08-25T06:36:13.222Z Reads: 147

```
For me its the same. I'm running FW 3.40 but using Ackmaniacs fw makes no difference. Maybe its the receiver. Vesc tool for Android works though...
```

---
## \#902 Posted by: AutoItKing Posted at: 2018-08-27T06:19:42.842Z Reads: 146

```
I've been seeing people post about this a lot. There is nothing wrong with your phone or Bluetooth module.
BV made a change in FW 3.40 that breaks the monitor apps. VESC-Tool will work fine since it already has the change.

Options: wait for ack to update his app to 3.40 or more, revert to 3.38, or install ack's firmware.
```

---
## \#903 Posted by: visnu777 Posted at: 2018-08-27T10:33:05.551Z Reads: 143

```
Hmmm, as I said, I already tried Ackmaniacs FW. Reverting to 3.38 needs an older version of VESC Tool to initially configure everything so I can't test it since the linux version 0.94 is not available (at least I didnt find it) I think I wait for 3.4 support :) Thanks anyway.
```

---
## \#904 Posted by: AutoItKing Posted at: 2018-08-27T22:14:36.390Z Reads: 144

```
Ah I see, could be your BLE module, is it a real HM-10? Clones or knockoffs have issues with Android 8.
If that's not it, then I'm out of ideas.
```

---
## \#905 Posted by: osbor Posted at: 2018-08-28T03:00:27.775Z Reads: 155

```
Reporting in with connection problems too.

![Screenshot_20180827-195624|250x500](upload://gLqnzJXhLQ8XYfPS0vMl05PseJ7.png)

![Screenshot_20180827-195525|250x500](upload://uAAFLEK3ODakYUj6gNZnX8X3Ddn.png)

I've actually gone through three different hm10 modules by now. One from BKB, one from Amazon, and one from Psychotiller, none of them work, all of them have the same symptoms with the app; connects then disconnects in an endless loop, doesn't transmit data.

I'm on Android 8.1
```

---
## \#906 Posted by: L3chef Posted at: 2018-08-30T09:44:48.189Z Reads: 131

```
Is there anyway to password protect each board you have?
```

---
## \#907 Posted by: krloz Posted at: 2018-08-30T19:15:27.636Z Reads: 143

```
I could use some help right now.
After a very long time without using my board I turned it on today.  Everything working fine after a check up except the Bluetooth. 
Im certain the app has been updating all this time but the board has been  untouched. 
I get a red blinking led in the Bluetooth module.  I can't remember what the led used to do but that is what im getting.  And I'm 100% sure Bluetooth was working before.
Now I just get the board name in grey in the app Ann's no connection.  
Thanks for any help
```

---
## \#908 Posted by: rey8801 Posted at: 2018-08-30T19:26:29.966Z Reads: 139

```
The Bluetooth light should be still red when connected not blinking. I would guess you update to Android Oreo 8 on your phone. If that is the case you need to flash your module with the HM10 firmware or get a new module.
```

---
## \#909 Posted by: krloz Posted at: 2018-08-30T19:35:32.406Z Reads: 150

```
@rey8801
 I have android 8 on this phone. But I don't understand how this would be a problem if the problem is the module. 
I know my module is original.  I bought it in the recommended seller of the first post.
So if the led shouldn't be blinking, and I have checked the wire connection.  Probably the problem is the module not working any more?
```

---
## \#910 Posted by: rey8801 Posted at: 2018-08-30T19:41:29.683Z Reads: 140

```
The one recommended in the post was a clone one. The original cost more than 15 euro just the module. Anyhow you do not need the original just flash your module, otherwise I have some module left. They are plug and play module all wired for 9 euro with donation to Ackmaniac. Anyhow I would advice to flash it. There are tutorial on the Arduino forum and also in this thread. The reason why it doesn't work is because Android Oreo changed the BLE connection so clone old module won't work. I bet your module showed up as CC2541 or similar. With ordinal firmware it will pop up as HM10. 
Just Google or search i  the forum and you find a lot of people with the same problem.
What you can do to check is take an old android phone not with Oreo and test it. You will see that thee is still possible to use it
```

---
## \#911 Posted by: Jaraya92881 Posted at: 2018-08-30T19:47:36.565Z Reads: 137

```
I'm on a galaxy note 8 and I've had similar issues, it seems to be a crap shoot of when it works. I dont get this issue with my nexus 6p.
```

---
## \#912 Posted by: rey8801 Posted at: 2018-08-30T19:51:21.377Z Reads: 135

```
Sorry forgot to check! From the app I see you have a MLT-BT05. Those clones are decent and I have some that works with Android 8.x and some not. Depends if they have the last firmware. Anyhow I always flash them with the ordinal HM10 firmware and then they all work. I recommend to do the same.
```

---
## \#913 Posted by: epster Posted at: 2018-08-30T20:14:05.957Z Reads: 135

```
I am sorry but you say that i need to flash my firmware on my module does that mean that i need to do this https://www.youtube.com/watch?v=ez3491-v8Og because if i have to start doing that every android update I think I will have to change to metr apps because i am not really interested in this kinda coding and stuff and i really suck at it and i always fuck up something. I also see that he bought another usb device to connect the module too I guess you also need that one right?
```

---
## \#914 Posted by: rey8801 Posted at: 2018-08-30T20:27:22.700Z Reads: 136

```
Yes that the procedure. You find also the tutorial on the Arduino forum page. You only need an Arduino nano or Arduino uno. Plus some wiring. Once you do it, the module will work with Android you don't need to do it every time. If you want I have some module left, already flashed and wired for cheap. I advice to flash it, but in case you have an option :wink:
```

---
## \#915 Posted by: xilw3r Posted at: 2018-08-31T08:58:52.836Z Reads: 138

```
Has anyone tried this with a FlipSky vesc 6 derivative?
Or any vesc 6?

When I open the app and scan, it shows nothing, even if there are a bunch of BT devices visible in the phones bluetooth settings. MLT-BT05 is also seen by the phone, but does not show up in the app. I am on android 7.1

Or is it just beacuse of the shitty BLE module?

Edit, when I turned GPS on BLE showed up immediately. I see the data! awesome
```

---
## \#916 Posted by: rey8801 Posted at: 2018-08-31T09:08:09.304Z Reads: 138

```
I am getting Flipsky vesc6. I can also try it, but I first need to find the time to set them after I receive them
```

---
## \#917 Posted by: rich Posted at: 2018-08-31T11:29:19.627Z Reads: 145

```
Hey guys!

I have some strange problems and no explanation for it, hope someone can help. My BT modules are recognized as HM-soft in the app. On my MTB with V6 and FW 3.38 it worked but since 3 weeks the app crashes when selecting the BT-module (Android 7.1.1 | App V1.111). I thought the BT module is broke but I still can connect with my old mobile  (Android 4.4.2 | App V1.70).

Now it’s getting really weird. Recently I finished another build with V4 and FW 3.38 and the same kind of BT module. It can connect and it works with Android 7.1.1 but the BT module is recognized as the same as my MTB (including name) so when I select my new board the app connects to my “MTB” with all its settings in the app  but it’s a different board. 

I’m very confused :crazy_face:
```

---
## \#918 Posted by: Ackmaniac Posted at: 2018-08-31T11:32:12.832Z Reads: 143

```
Did you flash the bluetooth modules with a new firmware. Because maybe the firmware gives it the same address?
```

---
## \#919 Posted by: Ackmaniac Posted at: 2018-08-31T11:34:26.626Z Reads: 152

```
BTW, i rolled out a new version yesterday which fixes a couple of small bugs and maxbe improves stability or connectivity for Android 8.0 devices. Especially at startup when it sometimes doesn't connect.

It also brings back the possibility to program other power settings for the front axle if you have a 4WD board.
```

---
## \#920 Posted by: rich Posted at: 2018-08-31T11:56:35.839Z Reads: 152

```
Thanks for quick reply! I'm a moron I forgot that I switched from V4 to V6 on my MTB and also changed the module. That's why both BT modules have the same board name but different adresses, all good, sorry.

But my main problem is that I can't connect  to my MTB, the app crashes after selecting the module (without opening the app main screen). It worked before and suddenly no more (did not update anything). No changes with V1.112. Any idea?
```

---
## \#921 Posted by: Ackmaniac Posted at: 2018-08-31T12:00:49.520Z Reads: 152

```
does the phone ask you to send the error report? Please do so if that's the case.
```

---
## \#922 Posted by: rich Posted at: 2018-08-31T12:06:58.612Z Reads: 151

```
There was an option "Feedback" after crashing (the second was "restart app". I just sent it, hope that was what you meant :laughing:
```

---
## \#923 Posted by: Ackmaniac Posted at: 2018-08-31T12:10:12.374Z Reads: 146

```
OK thx. It takes a while for google to provide me the information
```

---
## \#924 Posted by: Minim Posted at: 2018-08-31T23:28:59.612Z Reads: 144

```
Anyone got this working on a Samsung Note9? My iPhone connects to CC41-A Ble module but my android phone won't find it.
```

---
## \#925 Posted by: rey8801 Posted at: 2018-09-01T09:03:22.641Z Reads: 133

```
Read previous post. Your age using a clone module. Your specific one is not recognized by Oreo. Flash the HM10 firmware on it or get another compatible clone module.
```

---
## \#926 Posted by: Minim Posted at: 2018-09-01T20:13:10.696Z Reads: 133

```
Oh thats the same issue? And it has to be loaded through an arduino? I'll have a look at the arduino forum like you suggested and see if I can fix it.
```

---
## \#927 Posted by: rey8801 Posted at: 2018-09-01T20:17:04.347Z Reads: 136

```
Yep you need an arduino nano or uno. Here the link https://forum.arduino.cc/index.php?topic=393655.0
You find a video on YouTube if you search for it (like how to flash HM-10 firmware on...). I do it for the bluetooth module I sell and they work just fine.
```

---
## \#928 Posted by: Minim Posted at: 2018-09-01T20:55:33.817Z Reads: 129

```
It wont do with a CP2102 breakout, usbasp or similar? I don't have a arduino that's not seen magic smoke around atm :S
```

---
## \#929 Posted by: rey8801 Posted at: 2018-09-01T20:59:15.743Z Reads: 134

```
You need to load a script with Arduino IDE, which works on 3 pins on the arduino. If you have the same schematic and you can load the program it might work. I have arduino nano e uno for oter project so I always used them.
```

---
## \#930 Posted by: Minim Posted at: 2018-09-01T21:13:05.674Z Reads: 137

```
Doesn't look good.. The connections was as following but I don't have anything remotly close to that on mine. CP2102 is usb->uart and usbasp is for programming Atmel AVR :S Wonder if one of those fried arduinos could work anyways

Arduino D4 to P18 (Reset)
Arduino D5 to P21 (DD – Debug Data)
Arduino D6 to P22 (DC – Debug Clock)

https://www.fischl.de/usbasp/
```

---
## \#931 Posted by: rey8801 Posted at: 2018-09-01T21:29:11.533Z Reads: 143

```
Yeh I would suggest to get an arduino nano clone. You find them at 2-3$ on Ali. Otherwise buy another module. I have some left wired, plug and play if you do not find the right one. If you can wait then I would say get the arduino and flash it. An arduino is always useful for different projects.
```

---
## \#932 Posted by: Minim Posted at: 2018-09-01T21:42:23.903Z Reads: 146

```
I found a board finally :D It's supposed to be an arduino. Can I flash it with those one? 

http://www.myrcmart.com/micro-minimosd-kv-team-mod-arduino-1g-15x15mm-p-8875.html
```

---
## \#933 Posted by: rey8801 Posted at: 2018-09-01T21:43:46.535Z Reads: 143

```
I guess you will have to change the script before load it. You need several pins that I do not see on your board.
```

---
## \#934 Posted by: Minim Posted at: 2018-09-01T22:05:46.441Z Reads: 141

```
The script loaded at least but the pinout might be a problem. I'm on thin ice but if I remaped "int DD/DC/RESET" in the script to the pins available on my device and then provide the board with supply on vcc/gnd would that do the magic trick?
```

---
## \#935 Posted by: rey8801 Posted at: 2018-09-01T22:08:18.048Z Reads: 142

```
It should work. The second program you need to run it in the terminal windows. It will just tells the arduino to load the firmware as it's programmed so if you change correctly the pins layout in the arduino script it should work. At the end almost all the pins on an arduino can be input or output.
```

---
## \#936 Posted by: Minim Posted at: 2018-09-01T22:22:55.964Z Reads: 143

```
btw. any reason it can't be done like this? 

http://www.martyncurrey.com/hm-10-bluetooth-4ble-modules/#HM-10-update%20firmware
```

---
## \#937 Posted by: rey8801 Posted at: 2018-09-01T23:35:09.539Z Reads: 137

```
This option wasn't published when I started flash mine. Didn't know about it. It should work too
```

---
## \#938 Posted by: Minim Posted at: 2018-09-01T23:47:04.028Z Reads: 144

```
I can't get it working anyways. I tried first with the voltage divider without cheking signal levels at the pins and it didn't work. When I checked voltage at the TX pin it was 3.3V so I removed the voltage divider and it still didn't work out. Also tried with realterm and there's  no response at all when I send those AT commands :( Guess arduino is the way to go. Just have to figure out how the pinout is on the one I got.
```

---
## \#939 Posted by: rey8801 Posted at: 2018-09-02T05:42:57.247Z Reads: 151

```
I guess so. To me to much complications when you know that something works. Get an Arduino nano clone (cheaper than uno clone) some jumper wires and that's it.
```

---
## \#940 Posted by: Sender Posted at: 2018-09-02T18:57:16.161Z Reads: 170

```
Do you guys ever lose telemetry?  I fired up the board this AM and the board came up in red in the app as normal, but it won't really connect I guess? I don't get any telemtry.  I tried to resatart the board and and the app, but same thing.  Shows up, but when I click on it, it doesn't fully connect or something.... anybody know anything to try? Nothing has changed since last night when I was on it
![Screenshot_20180902-135752_ESC%20Monitor|243x500](upload://cq3n8iX9P51Ja2nmRLladPU8umQ.jpg)
```

---
## \#941 Posted by: rich Posted at: 2018-09-02T21:02:53.560Z Reads: 164

```
It's not connected, click "connect" on the top right corner. If it's connected then you can see "disconnect" at this place. But also sometimes I get zero values even when it's connected, but that's seldom.
```

---
## \#942 Posted by: Sender Posted at: 2018-09-02T21:08:03.354Z Reads: 165

```
Yeah, @mmaner helped me get it sorted.  That didn't work.  I had to delete the app twice, then shut down my phone completely. Then I got it going again. Weird.
```

---
## \#943 Posted by: caustin Posted at: 2018-09-02T22:29:00.461Z Reads: 170

```
Haven’t checked in awhile, has anyone gotten the android app to work with Metr Pro ble chip and ack 3.101 FW?  I can get it working with Amy other BLe app on iOS or android but not the ackmaniac android app. Connects but doesn’t display any telemetry no matter what. I had given up and just use Metr app but would like to get this working if anyone else has it work?
```

---
## \#944 Posted by: osbor Posted at: 2018-09-03T04:56:37.292Z Reads: 181

```
Hmmm
Refreshed the settings on my focbox through ackmaniac for the third time, and it started to connect and give telemetry to both the amazon bought hm10 and the psychotiller one no problems

https://www.amazon.com/dp/B0140R8DGQ?ref=yo_pop_ma_swf

https://psychotiller.com/product/mccloeds-blue-tooth-modules

That was...weird.
And my phone is a pixel 2xl with Android 8.1 latest on it
```

---
## \#945 Posted by: Ackmaniac Posted at: 2018-09-03T07:11:33.713Z Reads: 176

```
A couple of people are reporting issues with the latest Android 8.1
Need to google a bit, maybe i find something.
```

---
## \#946 Posted by: osbor Posted at: 2018-09-03T07:28:09.527Z Reads: 173

```
Yes apparently Google added some Bluetooth security stuff in 8.1 that the real deal hm10 is ok with but clones  aren't able to deal with
```

---
## \#947 Posted by: neiru37 Posted at: 2018-09-06T20:01:51.711Z Reads: 163

```
@Ackmaniac do you have plans on open sourcing your app? I want to give it a material design face-lift. It pains me as a ux engineer to see holo themed apps out in the wild.
```

---
## \#948 Posted by: skatardude10 Posted at: 2018-09-06T20:33:14.462Z Reads: 161

```
That would be cool. I don't see the app becoming open sourced, but I can't speak for the dev himself.... But I do want to voice my opinion here, a facelift to modern looking UI *would be sweet* :-) 

Regardless, it works, it's functional, so I have no real complaints.
```

---
## \#949 Posted by: Idea Posted at: 2018-09-07T12:52:38.125Z Reads: 164

```
Hi

From where I can download the older version 1.111
The new version 1.114 does not download data from VESC

My phone is LV V20, Android 7.0
VESC 4.12, firmware 3.38
```

---
## \#950 Posted by: Ackmaniac Posted at: 2018-09-07T12:53:44.129Z Reads: 166

```
What do you mean by "download data"
```

---
## \#951 Posted by: Idea Posted at: 2018-09-07T13:12:16.280Z Reads: 171

```
[quote="Ackmaniac, post:950, topic:20888, full:true"]
What do you mean by “download data”
[/quote]
No data updates: voltages, temperature, etc.
![Screenshot_2018-09-07-15-06-15|281x500](upload://iUFuTPMChPRRhsDAcMwOzccaAex.png)

Maybe it's a problem with my phone, but version 1.111 worked
```

---
## \#952 Posted by: Sender Posted at: 2018-09-07T13:49:32.349Z Reads: 167

```
I don't know if it will help, but mine did the same thing for a while. Connected but no telemetry.  Have you tried completely deleting the app again, restarting your phone, then redownloading the app?  This fixed my issue.
```

---
## \#953 Posted by: Idea Posted at: 2018-09-07T13:53:54.533Z Reads: 175

```
Yes, I did everything you wrote ... :frowning:

I will try to install the latest version on my second phone
```

---
## \#954 Posted by: Idea Posted at: 2018-09-07T13:58:28.215Z Reads: 179

```
Has anyone tried to run VESC Monitor with BT  FlipSky?

https://flipsky.net/collections/accessories/products/core51822-ble4-0-bluetooth-2-4g-wireless-module-nrf51822-onboard-ws82013
```

---
## \#955 Posted by: visnu777 Posted at: 2018-09-07T14:24:13.564Z Reads: 176

```
Yes, i did and it didnt work. Installed ackfw, baud set to 9600, no luck. vesc tool mobile worked.
```

---
## \#957 Posted by: DWU Posted at: 2018-09-09T04:32:49.146Z Reads: 168

```
The App is not working for me also. I tried two galaxy s8 phones, pixel 2, and galaxy s4.  It connects and disconnects. I'm able to label a name for it. when connected, it shows No Data info, same picture as the one displayed five posts above.

@Ackmaniac Any way you can fix this and update the app?
```

---
## \#958 Posted by: Idea Posted at: 2018-09-09T20:40:39.150Z Reads: 167

```
On another phone, the application works perfectly :)
```

---
## \#959 Posted by: Ackmaniac Posted at: 2018-09-09T21:32:30.351Z Reads: 165

```
Try to delete the data of the app. Then delete the app and reinstall it. Maybe reboot the phone in between. No idea where this is coming from.
```

---
## \#960 Posted by: Swix Posted at: 2018-09-15T18:45:53.415Z Reads: 170

```
I got the same problem with the app. Yesterday i had the 3.4 Fw, i could connect to the app but nothing displayed, metr worked fine. Today i updated to your 3.102 Fw. Now the app just connects and disconnects every 2-3 seconds. Now i have the issues with the metr app aswell, displays as connected but everything is 0. Bluetooth device name is Metr-576. I tried TPC connection with both apps and i get this in ESC Tool  "Could not read firmware version. Make sure that selected port really belongs to the ESC.". Andoid version 5.1.1

I tried options above: delete app, restart phone
```

---
## \#961 Posted by: ArnhemAnt Posted at: 2018-09-21T05:53:12.976Z Reads: 173

```
trying to find a reliable app to use so I can monitor my board and also make changes. I thought I finally found it, but after install (samsung galaxy s4) it keeps showing the bluetooth connection window asking me to name it, but every time I try, the screen disappears and another replacement screen pops up. I can get around this by repeatedly hitting "ok'. Managed to start setting up info for battery, etc, but the app just keeps crashing. I have tried to delete, restart then reinstall and the same thing keeps happening. 
Also found that if I try and set up a mode, it says that no ESC is connected.
Frustrated as I have tried to find an app for my iPhone with no luck so I went out and bought an Android just for this reason.
Any help would be gladly appreciated.
```

---
## \#962 Posted by: rey8801 Posted at: 2018-09-23T20:07:39.579Z Reads: 167

```
Fourth rounds of donation. Thanks
@lockeboss 
@jaatis 
@mikedv
:wink:
```

---
## \#963 Posted by: rey8801 Posted at: 2018-10-03T11:02:09.257Z Reads: 161

```
Fifth round of donations…Thanks guys

@BruSkater 
@eb1925
```

---
## \#964 Posted by: eb1925 Posted at: 2018-10-03T15:26:25.415Z Reads: 162

```
Anytime man!
```

---
## \#965 Posted by: Titoxd10001 Posted at: 2018-10-09T06:03:36.898Z Reads: 163

```
App seems to reconnect much better which is nice. Changing settings was nice feature when I let friend borrow board.
Unfortunately the mode didn't seem to want to switch between current mode to current mode with no reverse. Said friend managed to take a spill twice. They managed to be going in reverse instead if braking, so intuitively they press accelerate to brake not know it would launch the board from under them. Not sure if you could make double clicking both ways to switch direction a option. Though if you could take a look at mode switching from with reverse to without that would be great
```

---
## \#966 Posted by: Ackmaniac Posted at: 2018-10-09T06:22:50.383Z Reads: 162

```
Of course you can switch to a mode without reverse.
```

---
## \#967 Posted by: Benjamin899 Posted at: 2018-10-09T08:06:30.978Z Reads: 164

```
Hey ackmaniac could you maybe include distance into the Log.
```

---
## \#968 Posted by: Titoxd10001 Posted at: 2018-10-09T08:26:10.936Z Reads: 166

```
That is what I'm referring to. I made a separate mode settings where everything seem to change like motor max/min, battery max/min , max speed. In that mode I also put current no reverse but that didn't change when I switched to that mode.
```

---
## \#969 Posted by: Ackmaniac Posted at: 2018-10-09T10:28:55.735Z Reads: 166

```
I guess you have a dual motor setup and your Bluetooth module is connected to the salve. In this case you need to enable "Connect by CAN to ID" in the settings of the app and enter the ID of the master. This way when you make changes to the master the slave is updated automatically. Mode changes in general can only be made to the master.
```

---
## \#970 Posted by: Titoxd10001 Posted at: 2018-10-10T03:54:59.101Z Reads: 166

```
The Bluetooth module is connected to the master. Here is screenshots of what I mean. Only the "current no reverse with brake" doesn't change.

![20181009_205000|311x500](upload://9KpVBb6caK9H2dddD7kbaKWCsCG.jpeg) 

![20181009_205107|376x500](upload://xEXug3wNKorPRRM8HKYHCns4MdN.jpeg)
```

---
## \#971 Posted by: Ackmaniac Posted at: 2018-10-10T06:20:10.608Z Reads: 148

```
Oh, then deactivate "Send status via CAN" in the Esc settings of the master.
```

---
## \#972 Posted by: Pmac Posted at: 2018-10-11T05:49:05.718Z Reads: 152

```
any luck?

I am using the bluetooth module from flipsky which is the nrf51.  I'm gonna swap it for the HM-10 now as i have had no luck getting this to work with the ack software and only with the VESC Tool mobile software which doesn't have the features that the ack software has.
```

---
## \#973 Posted by: Jmding Posted at: 2018-10-11T06:11:33.999Z Reads: 151

```
I think it's hopeless. The Flipsky module is nrf based. Ack's app is ble based
```

---
## \#974 Posted by: Vannism Posted at: 2018-10-11T09:06:49.523Z Reads: 162

```
Hey all,
i've a question and hope someone can help me:
i bought the IOS App VESC Monitor and with my Raptor 2 Firmware v2.18 everything works fine.
But i use normally a Samsung Galaxy with ESC Monitor.
Because of the Stuttering problem i have to update Firmware to v2.18.
And since i've this Firmware ESC Monitor don't let me use the profile choose:
Not supported Firmware.
Is there any other Firmware for Raptor 2, which i can use with ESC Monitor?
I tried already the ackmaniac Firmwares, but then my remote doesn't work.
Will ESC Monitor support Firmware v2.18 in the future?
Can someone help me?
thanks in advanced
kind regards
Michael
```

---
## \#975 Posted by: Ackmaniac Posted at: 2018-10-11T23:09:50.869Z Reads: 157

```
Just released a new version 1.115 of the app which hopefully fixes some connection issues people had when the app stopped to connect to the Bluetooth module when it did it before. Please let me know if this version makes a change for those people.
I don't have the issue myself so it is hard for me to figure out the issue. hope this version makes a change.
```

---
## \#976 Posted by: CarlCollins Posted at: 2018-10-11T23:14:02.931Z Reads: 153

```
@Ackmaniac
Nico any possibility of IOS App?
```

---
## \#977 Posted by: Ackmaniac Posted at: 2018-10-11T23:23:17.620Z Reads: 160

```
The app is my hobby and doing it in my free time. I don't have the interest and time to do that in my free time. I also don't like the fees apple charges to be able to provide the app in the app store (100$ each year). And i don't have the hardware (no mac and iphone). So i would need to invest at least 2000$ for the equipment and spent maybe 500 hours in my free time to develop the app. This is money i won't ever get back by donations and time i would spent with a system i don't really like.
And i would feed a money eating machine that i don't like to support.
So long story short, if somebody want's to pay for it then maybe, otherwise i don't think so.
```

---
## \#978 Posted by: CarlCollins Posted at: 2018-10-11T23:24:24.548Z Reads: 163

```
@Ackmaniac
Thank you for the honest answer mate
```

---
## \#979 Posted by: Titoxd10001 Posted at: 2018-10-12T01:20:45.197Z Reads: 164

```
Referring to the mode switching problem I do have "send CAN status" as "False" on the master. 

If you can see in the screenshots I posted some of the settings are changing except for "Cur" to "Cur n R w Br" which is selected in the new mode.

This is on the newest version of the app
```

---
## \#980 Posted by: Jmding Posted at: 2018-10-12T04:24:46.466Z Reads: 165

```
Would it be possible to add the ability to configure the other parameters in-app? Like foc vs BLDC etc?
```

---
## \#981 Posted by: jadatmag Posted at: 2018-10-13T11:45:53.192Z Reads: 170

```
https://www.gofundme.com/

How much money would you need to do it professionally?

Maybe a trusted seller can help set this up.
```

---
## \#982 Posted by: maddy Posted at: 2018-10-14T06:45:30.070Z Reads: 158

```
Is it possible to control the speed of motor via bluetooth? Not just maximum speed, but actual speed.
```

---
## \#983 Posted by: rich Posted at: 2018-10-14T11:23:24.528Z Reads: 165

```
[quote="Ackmaniac, post:975, topic:20888"]
Please let me know if this version makes a change for those people.
[/quote]

Yessssss!
It is showing realtime data again (Android 7) :grin:
Thanks for the new version!
```

---
## \#984 Posted by: Giga Posted at: 2018-10-21T09:41:56.609Z Reads: 163

```
[quote="Ackmaniac, post:253, topic:20888"]
Just released a new version where the motor temperature is visible if temp sensors are installed in the motor.
[/quote]
[quote="Mathias, post:349, topic:20888"]
I’m trying to monitor the battery temperature and figured the easiest way would be to hook it up to the motor temperature slot.
[...]
I could easily find a way to monitor the temperature on my phone while riding!
[/quote]

Hi, 
I got the 105mm Skullboard/DIY Airless Hubs and they got a tempsensor. I can read it out with the AC-Tool via PC and Android Phone like you explained, but like @Mathias said, it doesn't get recorded. Is it possible to have a checkbox somewhere to enable and disable motor temp recording? 
Like you said, 99% of the motors don't have tempsensors, but a NTC is like 50ct and you can place it everywhere, either glue it inside the motors by yourself or just place it onto battery, BMS, Antispark switch, connectors...whatever.
```

---
## \#985 Posted by: chrisongtj Posted at: 2018-10-21T12:58:19.124Z Reads: 163

```
I'm using the VESC tool but this question is also relevant to the Ack app

How do i prevent others from connecting to my deck and changing settings? Is there any security that i can incorporate? Just imagining changing settings during a group ride
```

---
## \#986 Posted by: Jc06505n Posted at: 2018-10-21T14:18:55.539Z Reads: 163

```
That all dependent on the BT module you use , not really the app itself if I’m remembering correctly

http://fab.cba.mit.edu/classes/863.15/doc/tutorials/programming/bluetooth.html

https://stackoverflow.com/questions/49841867/bluetooth-hm-10-pin-to-connect-authentication-security
```

---
## \#987 Posted by: venti2k Posted at: 2018-10-28T12:20:34.339Z Reads: 159

```
Hey,
i am struggling somehow with similar problems. On my old phone (android 6...) i had no problems connecting to the BT module. The App version was 1.73 i guess. After updating to your actual version V1.115 it is connecting, but not reading any data. Same issue with my android 8.xx.
```

---
## \#988 Posted by: isabar Posted at: 2018-10-29T13:05:33.856Z Reads: 160

```
I second this request.
```

---
## \#990 Posted by: Ackmaniac Posted at: 2018-10-30T21:03:13.529Z Reads: 162

```
Answered already in the other thread. Please don't ask the same question multiple times in different threads.
```

---
## \#991 Posted by: secupol Posted at: 2018-11-02T01:59:06.486Z Reads: 167

```
I have developed HM-10 derivative using BGM111 Silabs's BLE module.
It was good working before 5 month ago as you can see below.
https://youtu.be/S6RjwkWSkBs
But now it does not work. After the app is updated.
Perhaps the app does not seem to send CCCD when the PDU size exceeds 20 bytes when connecting to ble. Is this different from before upgrading?
```

---
## \#992 Posted by: scaglionisc Posted at: 2018-11-03T12:09:44.527Z Reads: 159

```
Hello, im new to this tool, i followed every guide and instructions i fount, i managed to get both my foc box updated and set to run in sensored foc mode, managed to bind my alien tech remote the problem im having is getting the blue tooth to work, i did as instructed,UART baud is 9600 bps, the esc tool on my phone detects the hmsoft module and when i connect to it i do not see any data, if i throttle nothing happens in my phone app.
any advice appreciated.
```

---
## \#993 Posted by: Ackmaniac Posted at: 2018-11-04T12:34:16.470Z Reads: 159

```
Rx on the vesc is connected to TX on the module? And you power it by the 5V pin?
```

---
## \#994 Posted by: High-roller Posted at: 2018-11-07T18:38:07.681Z Reads: 157

```
I'm sure this has been answered before but I cannot find it for the life of me, so here goes:
If I have dual focboxes connected via PPM, when I first connect the module to one of them do I have to disconnect the other one before I turn on and start setting it all up?
```

---
## \#995 Posted by: DeathKing Posted at: 2018-11-15T06:54:36.864Z Reads: 156

```
Hi. After I update my vesc 4 to latest 3.4 firmware after connection to Bluetooth module I no see data. What I can do with this? Uart is 9600. Previously works good
```

---
## \#996 Posted by: Ackmaniac Posted at: 2018-11-15T16:58:20.645Z Reads: 154

```
Do you use PPM + UART?
```

---
## \#997 Posted by: DeathKing Posted at: 2018-11-15T23:05:53.305Z Reads: 154

```
Sure. I try 3 vesc. Same situation. Before update work good - after no. :frowning:
```

---
## \#998 Posted by: Ackmaniac Posted at: 2018-11-15T23:09:12.254Z Reads: 154

```
Oh, i just forgot that i didn't add the latest official firmware versions to the app. 
Think the last one that works is 3.38.
```

---
## \#999 Posted by: DeathKing Posted at: 2018-11-16T00:23:15.507Z Reads: 148

```
Can you do this in future? Your app is fantastic!!! I think you have your own firmware? Where I can see difference from official and download it?
```

---
## \#1000 Posted by: Ackmaniac Posted at: 2018-11-17T00:30:38.128Z Reads: 147

```
It's available here
https://www.electric-skateboard.builders/t/extended-ackmaniac-esc-tool-based-on-vesc-tool/35116?u=ackmaniac
```

---
## \#1001 Posted by: Makio13 Posted at: 2018-11-19T19:41:37.418Z Reads: 140

```
i am using vesc6 and the trampa bluetooth module.  the program connects fine to the bluetooth, but i get no readings. Will this module work with your program? am i probably doing something wrong?(i did read the whole thread to double check) Thank you
```

---
## \#1002 Posted by: Ackmaniac Posted at: 2018-11-19T23:29:56.643Z Reads: 144

```
I never tested it but i think the trampa bluetooth modules don't work with my app.
```

---
## \#1003 Posted by: Makio13 Posted at: 2018-11-19T23:45:13.942Z Reads: 146

```
thank you for the reponse! i will look into other modules.
```

---
## \#1004 Posted by: 5ilversurfer Posted at: 2018-11-20T17:06:21.109Z Reads: 147

```
Hi Ackmaniac. First of all - Thank you very much for the efforts and time you spend doing all this Programming and developing ! I am just beginning to read all this stuff and work into the Topic.

The past 5 Years e-skating it was always a hide and seek play with the police so just keep cool, push and hope for the best when they're coming ;-) Here in Germany, as you know, it is a matter of luck if the Policeman had a bad day or if he maybe just don't know the law about Eboards. I am living in Bavaria that makes it not easier...

Evolve offers the Service to send you a Remote which is limited to 6 km/h. I just ordered a Lacroix and now the Question is if it would also work to program a Nano V2 or if it has to be done by changing the VESC Firmware for example using your Tool.

Maybe you could give me a push into the right direction. Unfortunately I am depending on my driver License and it would give me a much better Feeling to have a "Hase Igel Mode" to activate.

Greeting from Nürnberg !
```

---
## \#1005 Posted by: Ackmaniac Posted at: 2018-11-20T20:15:13.433Z Reads: 146

```
By the app you can activate modes which are only active as long as the board is powered. So simply set a police mode as default and activate the ride mode via the app. If they stop you then switch off the board and back on to be in police mode again.
```

---
## \#1006 Posted by: 5ilversurfer Posted at: 2018-11-20T22:24:37.842Z Reads: 144

```
Thanks for the Quick answer. Can I achieve this without changing any other behaviors( in non Police Mode ) of the Board - meaning throttle curve, speed mode 1 & 2 on the remote etc. ?
```

---
## \#1007 Posted by: DeathKing Posted at: 2018-11-21T00:18:29.514Z Reads: 153

```
You planning in future add support of 3.40 and latast firmware support to your app?
```

---
## \#1008 Posted by: Livid Posted at: 2018-11-22T17:45:00.115Z Reads: 152

```
I can't get it to connect, i have an HM-10 module wired correctly, esc set to uart+ppm, 9600 baudrate. running latest firmware on the vesc. every time i connect to "HMSoft" module, it connects but doesn't provide any data, anything i click on it just says "esc not connected"
Any ideas?
```

---
## \#1009 Posted by: skatardude10 Posted at: 2018-11-22T18:37:30.034Z Reads: 151

```
Hey @Ackmaniac, where is the best place to view changelogs? I've been getting spammednwith notifications on the newest version, I was able to just disable notifications from the app in Android.
```

---
## \#1010 Posted by: Ackmaniac Posted at: 2018-11-22T22:36:00.144Z Reads: 144

```
Yes on Android 8 you need to configure the notifications. I was also able to close the app properly so that the annoying message which tells you that the app is still running is gone.
```

---
## \#1011 Posted by: slade Posted at: 2018-11-25T23:18:53.715Z Reads: 145

```
I got the Bluetooth module a few days ago. Super excited for it to come in! Just downloaded the Android app linked, and I was wondering if there's a second app as pictured on the product page to download as well. The one in the product's screenshot reminds me of Birds app and I think it looks pretty sleek
```

---
## \#1012 Posted by: Ackmaniac Posted at: 2018-11-26T12:26:24.341Z Reads: 164

```
I need to refresh the screenshots for the google play store
```

---
## \#1013 Posted by: slade Posted at: 2018-11-27T04:39:00.678Z Reads: 169

```
Do you mean refresh the photos on the product page? The photos on the Play store are pretty much up to date with what the Android app is.
I looked a little further and I found the apple version is much more inline with what the product page's screenshots are, but the app in development on [this thread by bradrisse](https://www.electric-skateboard.builders/t/new-esk8-app-for-ios-and-android/37318) is what is being advertised on the product page. This doesn't seem to be available yet but looks nice and I'm confused why it's on the product page.
```

---
## \#1014 Posted by: Ackmaniac Posted at: 2018-11-27T07:41:31.840Z Reads: 169

```
Badrisse and I have our own individual apps.
```

---
## \#1015 Posted by: slade Posted at: 2018-11-28T02:41:03.912Z Reads: 174

```
The confusion is coming from your product being advertised with his app that is unreleased.
```

---
## \#1016 Posted by: caustin Posted at: 2018-11-28T03:49:49.865Z Reads: 182

```
Sorry not following you. What product page are you referring to, on an App Store or website. Android or iOS. Last I checked ackmaniac was android only app, maybe you are referring to ackmaniac firmware that most if not all of these apps work with to pull data from but certainly to change settings and modes etc. please just link to whatever product page you are referring to so I understand what you mean.

Maybe you mean this:

Xmatic - Electric Skateboard by Thuan Pham
https://itunes.apple.com/us/app/xmatic-electric-skateboard/id1382937037?mt=8

![](blob:https://www.electric-skateboard.builders/5e7dd500-9868-47fd-8108-24e73b29602b)

Sent from my iPhone
```

---
## \#1017 Posted by: slade Posted at: 2018-11-28T04:08:22.426Z Reads: 173

```
[This is the product page I'm referring to.](https://buildkitboards.com/products/vesc-bluetooth-adapter) Specifically I'm talking about the android app.
```

---
## \#1018 Posted by: mmaner Posted at: 2018-11-28T04:22:51.619Z Reads: 170

```
@jlabs is selling an HM-10 Bluetooth adaptor, not an app. He is simply telling you where to get the app for both Android and iOS that works with the adaptor.
```

---
## \#1019 Posted by: Ackmaniac Posted at: 2018-11-28T14:40:37.662Z Reads: 170

```
That's not my product and the app that is shown on the page isn't my app.
```

---
## \#1020 Posted by: Makio13 Posted at: 2018-12-01T05:17:03.497Z Reads: 166

```
Well I got the Bkb module and it is doing the same thing. Bluetooth says connected but no f'd data comes through. Says esc not connected but upper left says connected? I tried switching rx and tx also.
```

---
## \#1021 Posted by: skatardude10 Posted at: 2018-12-01T07:17:07.346Z Reads: 170

```
ESC the BT connected to has uart 9600 baud selected?
```

---
## \#1022 Posted by: Makio13 Posted at: 2018-12-01T07:22:56.566Z Reads: 174

```
Yes. 10 char
```

---
## \#1023 Posted by: SeanHacker Posted at: 2018-12-01T09:38:47.301Z Reads: 176

```
[quote="Makio13, post:1020, topic:20888"]
but no f’d data comes through.
[/quote]

No fucked data? I have no clue what that is. What android version are you running? Android 8 and higher has problems with fake modules because of their firmware.
```

---
## \#1024 Posted by: Ackmaniac Posted at: 2018-12-01T10:12:50.748Z Reads: 169

```
The app doesn't support the latest official firmware version 3.40.
```

---
## \#1025 Posted by: Makio13 Posted at: 2018-12-01T15:02:49.207Z Reads: 166

```
Sorry just a typo.  No data comes through. Just zeros in all sections.
```

---
## \#1026 Posted by: Makio13 Posted at: 2018-12-01T15:09:51.954Z Reads: 165

```
Ok, so the vesc is on 3.4 so it just won't work with the app. Will it eventually, or do I need to revert to an earlier firmware?
```

---
## \#1027 Posted by: skatardude10 Posted at: 2018-12-01T16:41:59.371Z Reads: 166

```
Try Ackmaniac's ESC tool
```

---
## \#1028 Posted by: Makio13 Posted at: 2018-12-01T17:52:08.867Z Reads: 165

```
That is what I am trying to make work.
```

---
## \#1029 Posted by: Jmding Posted at: 2018-12-01T18:06:47.941Z Reads: 166

```
Might as well Side-grade to ackmaniac's firmware, which will make drv codes work with the app as well
```

---
## \#1030 Posted by: jadatmag Posted at: 2018-12-03T13:58:01.487Z Reads: 168

```
So you used the Ackmaniac ESC tool to upload the firmware?
And the android app "ESC monitor" connects and says "Discon"  (means it's connected) in the top right corner and shows all zero's in the interface?
And when you press on for example "mode" in the android app it says "esc not connected"?

A friend of mine has the same problem with his Raptor 2. No solution to be found :stuck_out_tongue:
I'm trying to help my friend resolve this issue.

The 3.4 firmware Ackmaniac is talking about is the latest https://vesc-project.com firmware I think. And not the firmware from his Ackmaniac ESC tool.

I was at a group ride this weekend and heard more people seem to be having the same issue. Noone could help my friend.
```

---
## \#1031 Posted by: Makio13 Posted at: 2018-12-03T19:39:07.198Z Reads: 168

```
Everything is correct but i never uploaded firmware to the vesc.  I only tried to use the adroid ap to see realtime data. I set up the vesc using the vesc tool, which i get functioning perfect with the trampa nrf module.  I bought the bkb module to try to get the ack. android tool to work.  Giving up.  Vesc tool works fine and i guess i don't need the sweet realtime display ackmaniac tool has. Oh well.
```

---
## \#1032 Posted by: jadatmag Posted at: 2018-12-03T20:51:53.344Z Reads: 164

```
So I just solved the issue for my friend.

In the Ackmaniac ESC tool I set the "App to use" to PPM and UART.

If you flash the firmware with that tool and do the same I bet you will have functioning telemetry on your smartphone!

I think this issue can only be solved over USB. As the vesc won't communicate with the bluetooth module you can't change the settings over bluetooth.
```

---
## \#1033 Posted by: Makio13 Posted at: 2018-12-03T21:32:38.203Z Reads: 169

```
I will give that a try!  I did set the mode in the regular vesc tool to ppm+uart using the usb and computer, but will check on the ackmaniac tool as well.   Thanks!
```

---
## \#1034 Posted by: thetechtrader Posted at: 2018-12-10T19:08:14.232Z Reads: 165

```
Anyone know if there is an android watch that will simply connect and read our VESC battery power remaining and show speed using GPS in the watch for current speed?

Looking for someone to walk me through it and possibly hire someone to help make it happen.
```

---
## \#1035 Posted by: adrienfeve Posted at: 2018-12-26T18:11:17.397Z Reads: 154

```
I am getting a lower voltage from the app than the voltage measured at the battery terminal using a voltmeter. Is this normal ? There is a more than 0.5V difference.
```

---
## \#1036 Posted by: Ackmaniac Posted at: 2018-12-26T22:10:52.967Z Reads: 159

```
That is normal. it depends on the tolerance of the resistor that is used for the voltage sensing on you VESC. If you have a 50V battery then 0.5V would be 1 % which is mostly the best type of resistors you get for a reasonable price.
```

---
## \#1037 Posted by: adrienfeve Posted at: 2018-12-27T04:15:11.758Z Reads: 158

```
Ok make sense. Thanks for the info.
```

---
## \#1038 Posted by: Ackmaniac Posted at: 2019-01-03T23:43:38.127Z Reads: 155

```
Just released a new version which supports the official version 3.39 and 3.40 to show the realtime data.
```

---
## \#1039 Posted by: skatardude10 Posted at: 2019-01-04T00:13:52.195Z Reads: 158

```
Nice! I know a few people who will appreciate this update.

At this point, what are the main differences (if any) between using your firmware + app and the official + app?

I'd it the timeout smooth ramping to set braking value? Does the watt limit in your version ramp watts from (say for example) 0W to 1000W linearly (or based on throttle curve) with 0%-100%  throttle input while standard just sets a limit on wattage and nothing else?  That's what I think I can remember the main differences being...
```

---
## \#1040 Posted by: HooliganLabs Posted at: 2019-01-04T17:15:58.028Z Reads: 148

```
Could you share where you got the documentation to handle messaging with the VESC?
```

---
## \#1041 Posted by: brown5tick Posted at: 2019-01-06T20:21:19.809Z Reads: 150

```
Just upgraded to app v1.118 and suddenly instead of the notification updating, it looks like it keeps getting re-sent. The Notification chime keeps chiming until I force-stop the app, switch off my board and then restart the app. I tried disabling 'Fast status notifications' but it doesn't make any difference. Any ideas?
```

---
## \#1042 Posted by: Ackmaniac Posted at: 2019-01-06T21:27:27.759Z Reads: 149

```
When you see the notification then you can change the settings of the notification. This way you can disable the bell sound.
```

---
## \#1043 Posted by: brown5tick Posted at: 2019-01-06T21:34:54.180Z Reads: 151

```
That's true, but it doesn't stop the notifications from continuing to pop-up... effectively stopping me from using anything else at the top of my screen.
```

---
## \#1044 Posted by: Ackmaniac Posted at: 2019-01-07T00:57:38.287Z Reads: 148

```
Thing there is another option in to not bring them to the foreground at the same place where the bell option is.
```

---
## \#1045 Posted by: AlexBE Posted at: 2019-01-07T07:41:35.432Z Reads: 147

```
Anyone managed to get this App working with an Enertion Unity? I have my fingers crossed for compatibility because of the derivation from Vesc.
```

---
## \#1046 Posted by: brown5tick Posted at: 2019-01-07T19:36:25.373Z Reads: 143

```
I appreciate that there are ways of tackling Android's treatment of rapid-fire notifications but I'm curious what the cause and solution might be for these newly introduced rapid-fire notifications. To be clear, this didn't happen (to me, at least) before the app was updated.
```

---
## \#1047 Posted by: Ackmaniac Posted at: 2019-01-07T19:44:17.272Z Reads: 145

```
The old notofications were the notifications of the old android before 8.0. But i saw that notifications don't work at all on the new devices. So i switched to the new version which sadly fire these annoying alerts without adjustment. Need to see if i can get that fixed in the software. Bit once you adjusted it it is fine.
```

---
## \#1048 Posted by: ShutterShock Posted at: 2019-01-07T20:18:46.277Z Reads: 149

```
Have you had any issues with Android 8.0, Samsung Experience 9.0, being able to detect a bluetooth module at all?

I can't seem to get my Galaxy s8 to detect my bluetooth module when it is connected to the vesc.  I have a super old phone that seems to see it just fine, but when I use my actual phone, the module doesn't show up.

It used to work fine for like 300 miles and now idk
```

---
## \#1049 Posted by: Ackmaniac Posted at: 2019-01-07T20:42:39.362Z Reads: 151

```
That is anither issue with Android 8.0 and above. The old BLE clones don't work anymore. There is a fix for that but you need to update the firmware with a arduino.
```

---
## \#1050 Posted by: ShutterShock Posted at: 2019-01-08T04:22:55.375Z Reads: 149

```
Oh really? I have an arduino sitting around.  I guess I could look that up on how to do it!
```

---
## \#1051 Posted by: Ackmaniac Posted at: 2019-01-08T08:15:48.268Z Reads: 150

```
Here you can see how to. Looks more complicated then it is.
https://forum.arduino.cc/index.php?topic=393655.0
```

---
## \#1052 Posted by: ShutterShock Posted at: 2019-01-08T08:20:13.366Z Reads: 150

```
Awesome thanks so much!  I will try that out, doesn't look to hard at all.  Last question, will your app work with the VESC Tool firmware?  I'm not sure what version, I can check if necessary.  Should be the one from whatever vesctool 0.87 had in it.  Haven't updated my vesc firmware at all recently because they are working fine and I have no reason to.
```

---
## \#1053 Posted by: Psmrman90 Posted at: 2019-01-10T01:43:09.296Z Reads: 153

```
 I've been using a canbus and slave/master set up between my focbox and vesc but I'm getting in the mail a second rc reciever so I can pair both vescs with the same remote so no need for master/slave.  BUT I also have a Bluetooth module that can connect to only one vesc, it is great because I can change config on an app, but without the vescs talking via canbus, any change made in the App would only change the config on a the vesc it's connected to.  My question is, is the canbus ONLY good for master/slave setups?  Or can I have both vescs cinnected via canbus, acting independently, yet still able to communicate any config changes through the App ?(since the canbus is connected)
```

---
## \#1054 Posted by: jensens Posted at: 2019-01-16T18:57:32.091Z Reads: 152

```
hello, 
I instaled the modified vesc tool and updated the firmware. I have a real HM-10. The app sees the module and can connect to it. But it says esc is not connected. What did i do wrong?
```

---
## \#1055 Posted by: gaetjen Posted at: 2019-01-18T13:08:27.852Z Reads: 149

```
I have been using your app easily for over a year now. But now it seems that the app doesn't show my boards anymore. I have two boards and none are shown on my phone. I have android 8 and the hm-10 clone you suggested.
```

---
## \#1056 Posted by: Ackmaniac Posted at: 2019-01-18T13:10:19.795Z Reads: 147

```
Did you update your smartphone to Android 8 since then? Because the HM-10 clones don't work with Android 8. You need to update the firmware on the modules to work with it.
```

---
## \#1057 Posted by: gaetjen Posted at: 2019-01-18T13:12:11.609Z Reads: 145

```
That is the case. Is there a new module I could buy, which supports Android 8, because I don't have an arduino?
```

---
## \#1058 Posted by: AlexBE Posted at: 2019-01-21T01:51:43.929Z Reads: 139

```
FYI, tested the app with a Unity, all seems to work. The only thing I noticed is that the motor current value is for only one motor, but I think that is how it is expected to work.

I would love to see motor temperature displayed and logged. Thanks for all your work on this.
```

---
## \#1059 Posted by: Ackmaniac Posted at: 2019-01-22T09:10:28.164Z Reads: 140

```
Just released a new update which for the unity support which summarizes the data of both motors and shows it. So in case you are using a unity you should set 1 motor in the settings to see the correct data.
```

---
## \#1060 Posted by: AlexBE Posted at: 2019-01-23T01:16:30.247Z Reads: 139

```
It works great. Im getting motor currents that make sense now.
```

---
## \#1061 Posted by: Psmrman90 Posted at: 2019-01-27T02:56:50.507Z Reads: 140

```
@Ackmaniac dude, just took my board for my first ride and was pleasantly surprised that the app keeps record of all the data.  You made a seriously great app.  You are a gentleman and a scholar.  

PS on another note, does anyone know how to (If possible) autosave the distance/location/time aspect of the ride?  So each time I go for a ride it saves a map view of where I went?  I know there are some apps for runners and stuff, but i wouldn't be surprised if this app had it too.
```

---
## \#1062 Posted by: skatardude10 Posted at: 2019-01-27T05:44:46.608Z Reads: 136

```
It saves those logs in a folder on your phone automatically and you can use something like VDLA to view the logs in a nice map with stats.
```

---
## \#1063 Posted by: Ronaldinho Posted at: 2019-01-31T03:04:33.451Z Reads: 130

```
great App Bro!!   I just would to see an Evo shape ... is there a way to change that?
```

---
## \#1064 Posted by: Spyro Posted at: 2019-02-01T13:55:23.033Z Reads: 145

```
Hi guys, I recently had some issues with the Ackmaniac android app not showing data / shows data periodically.
So basically I was using adc+uart on my e-bike. I decided to use an arduino to convert the adc input to ppm input so I could change modes on the android app. This was prior to the 3.103 update which allowed mode change on adc. 
I accidentally swapped tx rx for 5v and gnd. Then when I swapped it back to the correct position, the android app stopped showing data. All I did was change to ppm+uart from adc+uart. Everything else was the same. The vesc worked fine, no issues with performance at all. The bluetooth data just didnt show. I changed a bluetooth module and got it to work for 5 minutes. Then it just stopped working again. I took it out for a ride and it worked, I could change modes and everything. Then it just stopped again. 
I thought that I could have damaged my vesc by my mistake of swapping tx rx with 5v and gnd. So I tried to solder jumper wires to pin 28/29 on the microcontroller on the vesc itself after reading about someone having same issues as me (intermittent connections) and having success connecting 28/29 directly to the bluetooth modules, bypassing the traces on the pcb of the vesc. I ended up fucking that up and that was the end of my vesc. 

So I bought another one, and the same issue happened. 
I doubt it's software since it's intermittent, it's not weak signal, I put my phone right next to the module and it still didn't work. I doubt its hardware since I changed to a whole new vesc. 

Whenever I unplug the vesc, the data suddenly shows up on the android app. Like for a split second it sends data before I unplug it completely. This is what shows up during the unplugging process. ![Screenshot_20190201-214201|281x500](upload://9ObaKxOMLAVNqwQAbIXb17uQ9Yx.png) 
I honestly don't know what could be the problem, I reinstalled everything, factory resetting my phone as well, trying with another phone, same issue. 
If anyone could provide some insight into this I would be very thankful.
```

---
## \#1065 Posted by: doust Posted at: 2019-02-01T15:08:34.022Z Reads: 128

```
 hello yours akmaniac app can this connect to a focbox unity? thank you
```

---
## \#1066 Posted by: Ackmaniac Posted at: 2019-02-01T15:09:26.816Z Reads: 128

```
As far as i know only via additional HM-10 BLE module. I don't have a UNITY myself but that's what i heard.
```

---
## \#1067 Posted by: doust Posted at: 2019-02-01T15:32:56.422Z Reads: 126

```
 I just tested and it  not works I do not have the information but jarrive me to connect I must have the app akmaniac in the focbox unity or I can uses the one of enertion? Thank you for the quick reply
```

---
## \#1068 Posted by: Pantata Posted at: 2019-02-09T17:00:48.604Z Reads: 128

```
Hi, I am having problems with the android app. I have the new expensive BT module that works with all the apps. I am using ackmaniac firmware and I am able to connect via the ackmaniac esc tool but no data is displayed and when I click on add modes it will say "esc not connected" It is working all with the METR and PERIMETR app. no problem. Any suggestions?
```

---
## \#1069 Posted by: rich Posted at: 2019-02-09T17:15:39.758Z Reads: 127

```
Did you set the baud rate to 9600? If not then this is the reason.
```

---
## \#1070 Posted by: Pantata Posted at: 2019-02-09T17:17:55.521Z Reads: 130

```
Yeah I had it set to 115200 or something like that, other apps worked but to make sure I have set it to 9600 today and still the same.
```

---
## \#1071 Posted by: rich Posted at: 2019-02-09T17:30:58.560Z Reads: 127

```
 You definitely need the value of 9600, other apps use different baud rates. When it doesn't work with 9600 then you could try it with an older phone/android version as some people have troubles with the latest android fw and HM-10 clones.
```

---
## \#1072 Posted by: Pantata Posted at: 2019-02-09T17:33:11.648Z Reads: 127

```
That's why I bought the one that should have full support and should work with everything. Definitelly with ackmaniac. https://eskating.eu/product/bluetooth-uart-metr-pro-module-for-electric-skateboards-all-apps-os/  I miss the video recording overlay function, ackmaniac has it the best.
```

---
## \#1073 Posted by: Ackmaniac Posted at: 2019-02-09T19:38:10.813Z Reads: 127

```
The baud rate is only for the communication from the vesc to the module. The app doesn't care about the baudrate.
```

---
## \#1074 Posted by: rich Posted at: 2019-02-09T19:56:40.399Z Reads: 127

```
Ah interesting. So you advice to set it to 9600 because of the HM-10 BT module and it can be different for other modules if I understand it right.
```

---
## \#1075 Posted by: Pantata Posted at: 2019-02-09T20:29:35.450Z Reads: 127

```
Any thoughts why it wouldn't show no data, though show the connection and say it's connected? :/
```

---
## \#1076 Posted by: Ackmaniac Posted at: 2019-02-09T21:21:15.369Z Reads: 126

```
No idea. Do you need to add a pin in the other apps?
```

---
## \#1077 Posted by: Pantata Posted at: 2019-02-09T21:23:43.429Z Reads: 125

```
I first pair the device via blutooth where I have to set the pin (written on the back of the module) then I enable my location, give all privileges to the app and then all the apps work, only ackmaniac esc tool acting as described.
```

---
## \#1078 Posted by: Ackmaniac Posted at: 2019-02-09T21:24:15.433Z Reads: 128

```
My app doesn't support to add a pin. There's your problem.
```

---
## \#1079 Posted by: Pantata Posted at: 2019-02-09T21:24:44.641Z Reads: 126

```
Oh ok, nice to know, thank you. Does that mean it will not work or might in the future perhaps?
```

---
## \#1080 Posted by: Pantata Posted at: 2019-02-09T21:26:31.718Z Reads: 133

```
I guess the pin is a nice safety future but obviously... :)
```

---
## \#1081 Posted by: Ackmaniac Posted at: 2019-02-09T21:27:01.654Z Reads: 134

```
Maybe in the future. I guess you have a METR module because you said it is a expensive one. For my app you need the standard ones which are cheap. When i find the time i might have a look at the pin support but can't guarantee that your module will work because i have no details about them.
```

---
## \#1082 Posted by: Pantata Posted at: 2019-02-09T21:28:13.936Z Reads: 135

```
eskating is selling your BT module ackmaniac specific so I thought the support will be in the expensive one they sell as well. Thanks for the info and thank you for you
```

---
## \#1083 Posted by: Pantata Posted at: 2019-02-09T21:29:02.091Z Reads: 134

```
It's just the video overlay I cannot do like you have it on your app. There are other apps but don't show the info as nice as yours does. CHeers, good luck.
```

---
## \#1084 Posted by: Ackmaniac Posted at: 2019-02-09T21:32:00.513Z Reads: 134

```
They only advertise their product with my app. But i was never involved in that. And 64€ for a BLE module, wow. You can get the ones for my app for less than 3 dollars from china.
```

---
## \#1085 Posted by: Pantata Posted at: 2019-02-09T21:35:01.034Z Reads: 137

```
My thought actually was that vast majority of the money goes to the app developers as it should support all the apps etc... So I thought I am giving most of the money to you, Benjamin and the guy that makes METR etc... I guess stupid to think...
```

---
## \#1086 Posted by: Ackmaniac Posted at: 2019-02-09T21:36:42.833Z Reads: 136

```
But the attitude is nice, so thanks anyway.
```

---
## \#1087 Posted by: rey8801 Posted at: 2019-02-11T23:44:45.814Z Reads: 134

```
Hi, I plug the bluetooth module in the unity and set to 9600 the baud rate. I was using the bluetooth before with anothe rvesc, but I do not see live data. There is something more to do compare to previously? Thanks!
```

---
## \#1088 Posted by: AlexBE Posted at: 2019-02-12T01:53:52.990Z Reads: 133

```
Do you have telemetry turned on in the Unity?
```

---
## \#1089 Posted by: SeanHacker Posted at: 2019-02-12T03:27:14.596Z Reads: 137

```
[quote="Pantata, post:1085, topic:20888"]
My thought actually was that vast majority of the money goes to the app developers as it should
[/quote]

If that were only the case. I love the way you think though. It's how it should be.
```

---
## \#1090 Posted by: rey8801 Posted at: 2019-02-12T05:38:25.297Z Reads: 138

```
Well I turned on UART and set baud rate to 9600.is there something more to do?
```

---
## \#1091 Posted by: AlexBE Posted at: 2019-02-12T07:30:57.587Z Reads: 139

```
Are you using the latest version of the phone app? What symptoms are you seeing?
```

---
## \#1092 Posted by: rey8801 Posted at: 2019-02-12T07:38:32.436Z Reads: 144

```
App version V1.121. I see the bluetooth. I can connect to it through the app but I don't get any real data.
```

---
## \#1093 Posted by: rpasichnyk Posted at: 2019-02-12T19:57:59.993Z Reads: 147

```
Money from sold Metr Pro modules goes to me and @hexakopter. Expensive or not, this is of course very individual and everyone will have different opinions.

When we released Metr Pro, it was working with VESC Monitor. You can find a post somewhere and APK / version number that works. Some time later it stopped working. I guess there is some problem somewhere, with so many different modules this app supports it is hard to come up with the code that works for all of them. We are obviously willing to help. We can send a Metr Pro for free. We can also help fund the investigation, maybe something else, I don't know. We beleive there are enough people on this forum that can benefit having both Metr Pro and VESC Monitor working together and we want those people to be happy :v:
```

---
## \#1094 Posted by: rey8801 Posted at: 2019-02-12T20:21:40.214Z Reads: 149

```
That's a great talking. You module and app are really nice and people know it, don't worry :smile: To be honest I only used VESC monitor app so far. It's just now that I can not get it working with the unity but I will figure it out why.
```

---
## \#1095 Posted by: rey8801 Posted at: 2019-02-12T23:49:16.721Z Reads: 151

```
So got the module connected to an unity to work. Or well it works 1 time out of 4 and not sure eit is fast enough to get the real time data as before. For sure there is some conparibility problem.
![vescmonitor|281x500](upload://ivGbwTXAcdSM8eavaVSTPZ9PzRC.png)
Plus most of the time I get the temperature with a red highlighted bar.
```

---
## \#1096 Posted by: skatardude10 Posted at: 2019-02-15T23:46:29.642Z Reads: 142

```
It seems the app detects KV alright, because max speed to 60k ERPM is as expected.

But when setting 1 to 1 gearing, 110mm wheels and 75KV motors, it says I should be reaching 90-110mph, when it's only realistically 30 at full throttle... Does the speed calculation take into account motor KV? Am I missing a setting I need to change to get accurate speed readings?
```

---
## \#1097 Posted by: Ackmaniac Posted at: 2019-02-15T23:52:47.579Z Reads: 143

```
max speed in the mode box only says which speed can be achieved  with the max erpm setting. And when you disable max erpm it will set it automatically to 200000 erpm which results in that high speed.
```

---
## \#1098 Posted by: skatardude10 Posted at: 2019-02-16T00:12:10.627Z Reads: 146

```
![Screenshot_20190215-170902_ESC%20Monitor|243x500](upload://toSAbt0motcRawDK53ejM4aO9w2.jpeg) 

I should only be able to reach 33 mph on my setup according to other calculators.
```

---
## \#1099 Posted by: rey8801 Posted at: 2019-02-16T00:13:57.519Z Reads: 143

```
Are you sure motor magnets and wheels diameter is set correctly?
```

---
## \#1100 Posted by: skatardude10 Posted at: 2019-02-16T00:15:02.705Z Reads: 148

```
Magnets probably not.

I don't want to disassemble to see, maybe I'll just lower the number until the speed makes sense to get it right
```

---
## \#1101 Posted by: Ackmaniac Posted at: 2019-02-16T00:15:40.148Z Reads: 145

```
As i said it is a theoretical software limit which shouldn't be reached. Just ignore it, it doesn't matter.
```

---
## \#1102 Posted by: rey8801 Posted at: 2019-02-16T00:29:15.694Z Reads: 144

```
Well you can ride and adjust the motor magnets to match the GPS speed. Which motors do yuu have?
```

---
## \#1103 Posted by: caustin Posted at: 2019-02-16T00:54:14.509Z Reads: 141

```
Try magnets = 28
```

---
## \#1104 Posted by: skatardude10 Posted at: 2019-02-16T01:00:07.995Z Reads: 144

```
That worked! How did you figure that out?
```

---
## \#1105 Posted by: skatardude10 Posted at: 2019-02-16T01:01:04.291Z Reads: 147

```
Adjusting motor magnets up and down caused the speed to vary up and down wildly... 28 magnets worked, accurate speed now. TB Direct Drives for a little while.
```

---
## \#1106 Posted by: rey8801 Posted at: 2019-02-16T01:10:07.669Z Reads: 149

```
Yeh standard outrunners are 14, hub motors and direct drive are usually 20 or 28. Ah you have the TB direct drive, interesting!
```

---
## \#1107 Posted by: skatardude10 Posted at: 2019-02-16T01:38:40.551Z Reads: 151

```
@Lunasi lent me the set for a week to test ride. So far I'm loving them, I'm sold.
```

---
## \#1108 Posted by: caustin Posted at: 2019-02-16T13:50:00.827Z Reads: 156

```
Your speed was calculated at about twice accurate, and looks like using 14 magnets was likely, the rest is math lol.
```

---
## \#1109 Posted by: Sapphirinia Posted at: 2019-03-01T07:36:38.228Z Reads: 141

```
So what do you actually need to buy/Download to get this working? I have a focbox.
```

---
## \#1111 Posted by: advongunten Posted at: 2019-04-22T16:02:50.994Z Reads: 124

```
@ackmaniac: Is there a way to switch the "Range"-Panel to "remaining Range"? It would be great to change between this to properties by just clicking on the panel :-).
```

---
## \#1112 Posted by: Ackmaniac Posted at: 2019-04-23T07:22:02.068Z Reads: 123

```
Don't know if i understand correctly but it shows already the remaining range. It ic changeing constantly because it is calculated on the left over capacity and the current energy consumption. SO if you go down a hill and brake your average consumption goes down because you charge the battery and by this the range increases.
```

---
## \#1113 Posted by: advongunten Posted at: 2019-04-24T16:30:24.950Z Reads: 122

```
Thanks for your reply, i'm sure i was wrong and i know why, now.
I was irritated as i finished my 10km round and saw a Range of 26km and was at about 60%.
This let me think "ok this should be the total Range Value, because 10km look like the used 30% (just charged to 90%) so i have 60% -> ~16km left equals 90% -> ~26km.
My Setup: 12S6P(LG HG2 3Ah), dual 6374... and with my driving style 36km Range without mental absence :-).
```

---
## \#1114 Posted by: Ackmaniac Posted at: 2019-04-25T23:38:09.104Z Reads: 121

```
No it means with your 60% left in the battery you can get a range of 26 km.
```

---
## \#1115 Posted by: Jarno Posted at: 2019-04-27T12:24:36.780Z Reads: 121

```
What is the latest firmware version of VESC that this app still works with?
```

---
## \#1116 Posted by: Rodeodave Posted at: 2019-04-28T18:38:15.908Z Reads: 127

```
I have a noob question regarding programming drive modes with the ESC Monitor app for the Enertion Nano-X/Raptor 2.

In which mode should I have the Nano-X, r-spec or beginner? Can I still use the physical mode switch on the remote with one stock and one programmed mode?

Is the drive mode programming permanent, or does it only take effect when the app is running?
```

---
## \#1117 Posted by: Marksmoura Posted at: 2019-04-30T10:22:25.289Z Reads: 130

```
My app keeps crashing 1sec after connecting.
From Google play I get the version 1.121 is this correct?

I shared the apk to another cellphone and it still crashes the same way. 

I have ppm+uart enabled and uart settings 9600.

I have all permissions enabled. 
I am using Huawei p20 pro and a one plus x.

My h10 also has a resistor divisor 2k/1k.

After I connect I get the name dialog box and it works if I am quick setting the name and crashes after 1sec.

I am using firmware 2.54 and it connects well with USB.


I can connect using a Bluetooth scanner app:
![blescanner|241x500](upload://AkH6lmb9HmmeX8FfXxOWLCM3DYy.jpeg) ![blescanner|241x500](upload://sdnKhOQi4zcPjpnNUByeKzZBiPm.jpeg)
```

---
## \#1118 Posted by: Marksmoura Posted at: 2019-05-01T15:31:23.124Z Reads: 116

```
Do I need to install the latest firmware 3.xx?
At the moment 2.54 is stable for me and I enjoy the simpleness of the bldc tool.
```

---
## \#1119 Posted by: Ackmaniac Posted at: 2019-05-01T23:34:13.011Z Reads: 114

```
2. 54 runs fine as well. 3.103 has some more features but if our board runs fine then kepp it that way. The app should work with 2.54 as well. No idea why the app crashes for you.
```

---
## \#1120 Posted by: Marksmoura Posted at: 2019-05-02T09:43:40.438Z Reads: 114

```
Update:

Today I turned the board on and tried to connect again with absolutely no changes. And it works now. 

Don't ask me why, I also can't explain.
```

---
## \#1121 Posted by: Eskate444 Posted at: 2019-05-10T03:46:45.099Z Reads: 117

```
Dear Ackmaniac,

I used your vesc monitor on android using firmware 2.80 (on my focboxes Raptor 2)

However when i upgraded to firmware 3.56 via vesc tool

The app does not work anymore with my board,

Is there any way i can get this to work? I really love the app!

Thank you
```

---
## \#1122 Posted by: Eskate444 Posted at: 2019-05-10T03:46:56.604Z Reads: 119

```
Dear Ackmaniac,

I used your vesc monitor on android using firmware 2.80 (on my focboxes Raptor 2)

However when i upgraded to firmware 3.56 via vesc tool

The app does not work anymore with my board,

Is there any way i can get this to work? I really love the app!

Thank you
```

---
## \#1123 Posted by: Marksmoura Posted at: 2019-05-10T03:52:48.966Z Reads: 121

```
Hello ackmaniac,

I would like to debug the PPM input. 
Is it not possible to record the signal/values the VESC is reading?

At the moment I noticed in some rare moments my board for a brief moment keeps accelerating and if we had the history of the signal we could easily debug if the remote has some problems. 

I think this would be a very very useful variable. 
Sometimes people have crashes because the board for example breaks out of nowhere. 
Here we could see if it was just an internal problem or if the remote sent the signal to brake by mistake. 

Thanks and keep the good work
```

---
## \#1124 Posted by: louwii Posted at: 2019-05-14T04:57:05.949Z Reads: 115

```
Hi @Ackmaniac

I'm currently building a tool to look at the logs that your app saves (thanks a lot for the logs BTW!). There's a "Power" column in the csv but I'm not sure what it is, can you tell me?

Thanks!
```

---
## \#1125 Posted by: Ackmaniac Posted at: 2019-05-14T22:00:15.350Z Reads: 123

```
Should be watts.
```

---
## \#1126 Posted by: louwii Posted at: 2019-05-15T00:17:38.118Z Reads: 120

```
Thanks dude
```

---
## \#1127 Posted by: sch_ch1 Posted at: 2019-06-12T14:07:32.877Z Reads: 109

```
I have the problem that the vesc monitor app „refreshes“ the connection every 5 sec’s :roll_eyes:. I open the app, connect to the BT module but it keeps disconnecting and then connecting again every 5 secs.

When using a BLE scanner the connection is stable.:man_shrugging: 

Does anyone know what I can do or try to fix this?
```

---
## \#1128 Posted by: spei Posted at: 2019-06-12T14:23:08.454Z Reads: 105

```
Try turning off battery optimization for the app
```

---
## \#1129 Posted by: sch_ch1 Posted at: 2019-06-12T14:34:26.744Z Reads: 103

```
Thx, haven’t read about that tipp before,  but unfortunatelly it didn’t help.
```

---
## \#1130 Posted by: spei Posted at: 2019-06-12T14:39:37.415Z Reads: 106

```
Have you tried to unpair bt device, clear app data and start from scratch?
```

---
## \#1131 Posted by: sch_ch1 Posted at: 2019-06-12T15:27:32.779Z Reads: 109

```
unpair?!
My phone always says “pairing rejected” when I even try to pair^^ … after googling, I found this.
rey8801:
“Bluetooth Low Energy modules do not require you to connect it directly as a normal Bluetooth module. You only need to connect to it through the app that supports the feature.”

In the app it shows up, but as I said, it always reconnects after 5 sec’s.

Tried to clear app data but still the same problem.
```

---
## \#1132 Posted by: spei Posted at: 2019-06-12T15:45:35.266Z Reads: 106

```
What android version are you running? There was problem with 8+ and bt module needed to be software upgraded throu arduino.
```

---
## \#1133 Posted by: sch_ch1 Posted at: 2019-06-12T16:52:58.365Z Reads: 104

```
I know, I searched around a while already, without success solving my problem. Im using android 5.1.1
```

---
## \#1134 Posted by: spei Posted at: 2019-06-12T17:05:30.470Z Reads: 102

```
I remember having the same problem, but Im not entirely sure how I solved it. What I did was reinstall app few dozen times restarting phone after every uninstall just to be sure and disabling app optimalization,  making sure that all permissions were granted before opening freshly installed app, turning BT on phone on/off, playing with battery optimalization settings and so on. And just like that it started to work. I also flashed new firmware on hm10 module but I had 8+ android.
```

---
## \#1135 Posted by: sch_ch1 Posted at: 2019-06-13T12:02:26.152Z Reads: 105

```
Thanks for your help!
Im trying, but getting frustrated and loosing hope slowly.

I wanted it mostly to monitor my battery, is there any other app I can try or use with only the bluetooth module (without nrf)?
```

---
## \#1136 Posted by: spei Posted at: 2019-06-13T12:27:24.577Z Reads: 106

```
I know only this one, metr, and vesc-tool. But the last two uses nrf.
```

---
## \#1137 Posted by: sch_ch1 Posted at: 2019-06-14T00:00:27.852Z Reads: 106

```
omg, Im so stupid… I checked the wiring so many times before connecting the hm10 to the vesc, that I got it mixed up in my head and thought it was right… I had tx -> tx and rx -> rx, instead of tx -> rx and rx -> tx

now everything works just fine :sweat_smile:
```

---
## \#1138 Posted by: mad_engineer Posted at: 2019-06-22T20:29:07.186Z Reads: 106

```
Did anybody get the app working with the new trampa "wireless BLE bridge to VESC"?

The VESC app works perfectly and in this app, the dongle is shown, too. But when it's connected to the dongle it shows "esc not connected". Any suggestions?
```

---
## \#1139 Posted by: Fixvid Posted at: 2019-07-09T06:18:08.725Z Reads: 105

```
Hi, 
I tried using a hm10 module, cross Tx, Rx connections, supply 5v, set UART and baud rate to 9600bps, but when i start the ESC monitor i can see the hm10 module, connect to it (red led stays on hm10) but no data is streamed and it says 'ESC not connected'. 
I tried dozens of combinations but still no data is streamed to app. Any ideeas? 

My fw is 3.53, does the app work with it ?

[IMG]http://i64.tinypic.com/2hgcx3p.jpg[/IMG]
```

---
## \#1140 Posted by: L3chef Posted at: 2019-07-29T17:07:36.231Z Reads: 90

```
@Ackmaniac ![IMG-20190729-WA0000|281x500](upload://yDoXgnY1q9Gp7dutGSyvq2ookoJ.jpeg)  
Don't see the throttle vs power x/y anymore?
Also what the difference between those 4 modes?
```

---
## \#1141 Posted by: TSJ Posted at: 2019-08-08T19:41:10.889Z Reads: 86

```
I think I have it working, but just for my own information, can someone explain how/where the motor settings are stored?  If I set up BLDC in the vesc tool and then write it to the vesc, they will be stored in the vesc.  If I then set up FOC and write to the vesc, will both BLDC and FOC settings be stored in the vesc?  Or, is the app storing these settings?  Can you set up and switch between a sensored mode and non-sensored mode?
```

---
## \#1142 Posted by: L3chef Posted at: 2019-08-08T20:52:26.399Z Reads: 85

```
All of that is expained i first post. Except your last question. 
I don't think you can, but I'm not 100% sure
```

---
## \#1143 Posted by: ChristianT Posted at: 2019-08-14T07:08:14.681Z Reads: 84

```
@Ackmaniac I just have to give you some huge compliments Achmaniac. Thank you for your app. I haven´t tested it yet as I don´t have my first DIY finished but I love it already.

Somone can just briefly explain me the difference between the vesc-tool, ackmaniac and unity app?

Thanks guys <3
```

---
## \#1144 Posted by: pundahh Posted at: 2019-08-14T07:32:57.949Z Reads: 86

```
VESC-Tool is the app designed by vedder himself. Official firmware so to say.

Ackmaniac is a version of the vesc tool by ackmaniac. Core elements are the same.

Unity is a simpler app also based off vesc tool. Only works with unity as the name suggests
```

---
## \#1145 Posted by: TSJ Posted at: 2019-08-14T14:34:41.517Z Reads: 87

```
I just went for my first commute after getting the app and board working and the app is crashing when I try to connect to the board.  The app starts and it shows the bluetooth connections and when I click on the board, the app crashes.  It looks like the app was updated to 1.123 in the last day or two.  It was working great before this.  Anyone else having issues?  I am on android 9.
```

---
## \#1146 Posted by: Ackmaniac Posted at: 2019-08-14T16:58:09.244Z Reads: 88

```
Will fix it today.
```

---
## \#1147 Posted by: Ackmaniac Posted at: 2019-08-14T17:03:06.580Z Reads: 89

```
Released a new version, please give it a try. Sadly i don't have android 9.
```

---
## \#1148 Posted by: TSJ Posted at: 2019-08-14T19:10:48.158Z Reads: 87

```
It connects now without crashing.  I will give it a test ride on my way home from work and let you know if there are any issues.  Thanks for the quick fix.
```

---
## \#1149 Posted by: thisguyhere Posted at: 2019-08-30T16:15:14.223Z Reads: 79

```
@Ackmaniac

nico, i'd like to request an update to the monitor so it works with Unity.

i know it's a time suck, so i'm ready to collect funds for your time.

if you're up for it, let me know.

thanks!
```

---
## \#1150 Posted by: Ackmaniac Posted at: 2019-08-30T19:34:24.682Z Reads: 79

```
Sure, can have a look if i find the time. Once you have a kid it's hard to find some spare time for hobbies.
```

---
## \#1151 Posted by: thisguyhere Posted at: 2019-08-30T19:52:56.175Z Reads: 80

```
congratulations on being a dad!

i can see how that'd be all consuming.

but there's a bunch of us who'd rather use yours than the other monitors.

anything you can do would be great.

we'll pool some money together too.
```

---
## \#1152 Posted by: pookybear Posted at: 2019-08-30T21:11:28.329Z Reads: 81

```
Unity monitor and fw like the old focbox would be sweet. I'm down to donate as well.

I'm still running your fw on mine and my friend's boards.
```

---
## \#1153 Posted by: Ackmaniac Posted at: 2019-08-31T21:36:12.884Z Reads: 82

```
Just released a new version. Please try if you can see the data with the actual unity firmware.
```

---
## \#1154 Posted by: thisguyhere Posted at: 2019-09-01T07:00:17.843Z Reads: 81

```
Omg no way. 

A bit late in the evening, will try first thing tomorrow. 

Thank you!
```

---
## \#1155 Posted by: deucesdown Posted at: 2019-09-01T17:35:05.169Z Reads: 82

```
It verks! :) Unity 23.44, I'm getting data. Suh-weet! @thisguyhere
```

---
## \#1156 Posted by: thisguyhere Posted at: 2019-09-01T17:43:21.970Z Reads: 80

```
fukin' stoked.

did you use the onboard bluetooth module that comes with unity, or plug a bt module into uart?

just sent @Ackmaniac some funny money for his troubles.

i encourage everyone else to do the same if you're using esc monitor.

nico@asoft-ackermann.de
```

---
## \#1157 Posted by: deucesdown Posted at: 2019-09-01T18:13:28.780Z Reads: 82

```
[quote="thisguyhere, post:1156, topic:20888"]
did you use the onboard bluetooth module that comes with unity, or plug a bt module into uart?
[/quote]

I plugged a BT05 flashed to HM10 into the uart. Didn't think to try other stuff. I usuall have a METR pro plugged into the UART.
```

---
## \#1158 Posted by: caustin Posted at: 2019-09-01T18:26:40.643Z Reads: 81

```
This is excellent, I will have to also try it with stock unity BLE module and reconfirm again that neither the Metr UART or METR unity chip swap interop works here sigh lol
```

---
## \#1159 Posted by: Ackmaniac Posted at: 2019-09-01T19:18:05.887Z Reads: 80

```
Thx a lot for the donation. Much appriciated. Will have a look if I can integrate the unity a bit better. Like seeing each motor individually.
```

---
## \#1160 Posted by: Flasher Posted at: 2019-09-01T19:31:30.955Z Reads: 82

```
@Ackmaniac  hey there. You're the best person to answer this. Is there a way to see a mapping of the rides I do? I would like to go back to previous rides and see on the map where I've been
```

---
## \#1161 Posted by: deucesdown Posted at: 2019-09-01T20:06:51.680Z Reads: 81

```
Tried connecting to on-board BLE, no data. Also tried connecting to METR pro, no data.
```

---
## \#1162 Posted by: thisguyhere Posted at: 2019-09-01T22:12:11.603Z Reads: 83

```
this, afaik, isn't built into esc monitor but you could easily use another app to map your rides.

i use this one

https://play.google.com/store/apps/details?id=com.ilyabogdanovich.geotracker&fbclid=IwAR3-WzkmBle7HMnYrq424LdGPktVdpk8CnUM7FXJfD_rv_DN9wUlXi3np3E

produces something like this

https://forum./t/pictures-and-nothing-else/79/2302
```

---
## \#1163 Posted by: Flasher Posted at: 2019-09-02T02:37:25.670Z Reads: 88

```
I dont know how you got him out of retirement....keep doing it. We need him
```

---
## \#1164 Posted by: Ackmaniac Posted at: 2019-09-02T09:05:43.697Z Reads: 91

```
A very nice tool was @DeathCookies Data Analyser
 ttps://www.electric-skateboard.builders/t/vesc-data-log-analyzer-vdla/16582

Sadly he decided to remove it because of missing donations. Maybe the community can help him out.

Maybe for future i can add a map view of the old data as well. but for sure not as advanced as Deathcookies version.
```

---
## \#1165 Posted by: thisguyhere Posted at: 2019-09-04T17:53:55.102Z Reads: 91

```
confirming it works, just remember to turn on ppm+uart, i think you need to use FOCBOX_TOOL to enable that.
```

---
## \#1166 Posted by: pookybear Posted at: 2019-09-04T20:52:54.499Z Reads: 95

```
Are using the unity's BT module or HM10 peripheral?
```

---
## \#1167 Posted by: thisguyhere Posted at: 2019-09-04T20:54:29.527Z Reads: 96

```
[quote="pookybear, post:1166, topic:20888"]
HM10 peripheral
[/quote]

this one, didn't even try with the onboard BT
```

---
## \#1168 Posted by: Titoxd10001 Posted at: 2019-09-07T20:43:10.892Z Reads: 91

```
Anyone having issues connecting with the app

Edit: App didn't show board name in red, but was still able to connect
```

---
## \#1169 Posted by: Ackmaniac Posted at: 2019-09-09T13:25:38.646Z Reads: 89

```
I experienced the same issue, need to have a look how that can be possible.
```

---
## \#1170 Posted by: Sender Posted at: 2019-09-09T14:19:47.737Z Reads: 86

```
Oh sweet! So now I can run my ack app with the unity?!


I assume it just gives telemetry and you can't change settings?
```

---
## \#1171 Posted by: etvoila Posted at: 2019-09-24T15:28:12.054Z Reads: 78

```
Hi everyone, i have issue with the app, i downgrade my 2 board from vesctool 3,53  (too much connection lost) to ackmaniak 2,54 but the app don't work.

I use the flipsky bt module who worked with vesctool app

-ppm and uart is ok
-baud 9600 too (tried with 115200, nothing better)
-autorisations ok

Bt board is recognized but there is no data information, and "esc not connected" message.

I've tryed to uninstall app and fw 3 times, no more chance.

i have a shitty huawei psmart who have many trouble with bt signals but he worked with my bt flipsky and vesctool fw.

any ideas ?
```

---
## \#1172 Posted by: Ackmaniac Posted at: 2019-09-26T09:53:51.986Z Reads: 75

```
Guess that the onboard blueetooth module isn't a low energy module and my app only works with these.
```

---
## \#1173 Posted by: etvoila Posted at: 2019-09-26T19:08:38.532Z Reads: 71

```
Thx for your answer, so a cheap wish like bt module should work ?
```

---
## \#1174 Posted by: louwii Posted at: 2019-09-30T02:40:34.422Z Reads: 70

```
I might have made a very basic site, that has a basic VESC log analyzer. You can choose to not save the data online, but if you do, the data is stored for a week (so you can share the link to other people).

Poke @Flasher 

https://esk8bible.com/vesc-log-chart
```

---
## \#1175 Posted by: Flasher Posted at: 2019-09-30T03:04:17.709Z Reads: 70

```
![Screenshot_20190929-230200_Chrome|243x500](upload://5Qsegax4LyIDI8NSa5t3sByBJMF.jpeg) 
Works well for most. But I do have some that show rolling at a max of 1-2 km/h 😂
Otherwise, this is perfect
```

---
## \#1176 Posted by: jun1208 Posted at: 2019-09-30T05:22:35.074Z Reads: 67

```
Flipsky's BT module won't work with Ack's app, tried it before :frowning:
```

---
## \#1177 Posted by: malJohann Posted at: 2019-09-30T10:27:48.335Z Reads: 64

```
@Ackmaniac e&ZeroWidthSpace;sk&ZeroWidthSpace;8&period;n&ZeroWidthSpace;ews
```

---
## \#1178 Posted by: etvoila Posted at: 2019-09-30T20:55:35.382Z Reads: 62

```
Yeah, what solition did you find ?
I tried many time wiring with my aliex hm10 and no more result, app is mute, bt is well scan but no data apear
```

---
## \#1179 Posted by: jun1208 Posted at: 2019-09-30T23:36:56.327Z Reads: 66

```
I didn't try to make it work, I know that some hm10 modules work but I didn't borther to try..
```

---
## \#1180 Posted by: M4rcus_63 Posted at: 2019-09-30T23:41:27.825Z Reads: 71

```
I recently got the app on a new Android phone, and in my phone's Bluetooth settings I can see the Bluetooth chip that is connected to the VESC (DSD TECH), But in the VESC monitor app, it is not visible. I tried redownloading the app as well. Suggestions?
```

---
## \#1181 Posted by: M4rcus_63 Posted at: 2019-10-01T01:49:36.726Z Reads: 72

```
Ackmamiac, I am having trouble connecting my phone to the Bluetooth module. My phone sees it in my settings but not on your app. Suggestions?
```

---
## \#1182 Posted by: Flasher Posted at: 2019-10-01T02:30:28.430Z Reads: 75

```
To all using flipsky bluetooth modules. They do not support ack. You need to buy an actual hm10 bluetooth module. Easily bought on amazon and even easier to wire up :slight_smile:
```

---
## \#1183 Posted by: louwii Posted at: 2019-10-02T06:05:53.077Z Reads: 71

```
Glad you like it! For the 1-2km/h speed, I might have an idea of why it's happening. You can eventually send me the file so I can look at it, if you want to.
```

---
## \#1184 Posted by: DanielJohn Posted at: 2019-11-04T11:49:23.755Z Reads: 59

```
Does this app replace the decktop software, or is the software still needed?
```

---
## \#1185 Posted by: Ackmaniac Posted at: 2019-11-06T01:36:29.633Z Reads: 57

```
For the motor detection, hall sensors, app details and so on the desktop software is still needed.
```

---
## \#1186 Posted by: Paulycnotes Posted at: 2019-11-15T17:04:53.526Z Reads: 56

```
Where can I get one for AWD use...May need 2??  Please advise...price and specs...Thanks.
```

---
## \#1187 Posted by: DanielJohn Posted at: 2019-11-21T14:02:17.605Z Reads: 51

```
Is there anyway to record a single ride, or is the app limited to overall board distance?
```

---
## \#1188 Posted by: Timesk8 Posted at: 2020-02-04T18:50:03.041Z Reads: 28

```
Would anyone know if, the Trampa NRF bluetooth dongle works with your Ackmaniac ESC-Monitor? Or do I need to only use the HM-10? I just want to use the app to configure the PPM pulsewidth for my new VX1 remote for the Lacroix Prototipo. Would the android app suffice? Help is much appreciated.
```

---
## \#1189 Posted by: kevingraehl Posted at: 2020-02-14T02:25:00.588Z Reads: 14

```
Same too.  Same issue
```

---
