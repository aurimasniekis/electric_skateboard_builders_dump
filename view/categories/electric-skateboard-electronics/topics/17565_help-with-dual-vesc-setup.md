# Help with dual vesc setup

### Replies: 50 Views: 4006

## \#1 Posted by: WARMAN Posted at: 2017-02-11T18:26:05.533Z Reads: 428

```
So got the board built currently connected to bldc tool can only get one motor to spin,both vesc's have power motor dection works on both motors.
My settings are set for master as follows 
Controller Id 0
PPM and UART 
Send status over can disabled "not ticked"
Mutiple esc over can enabled "ticked
settings for slave is setup as follows
Controller id 1
PPM and UART 
Send status over can enabled "ticked" 
Mutiple esc over can disabled "not ticked" 
If I tick can fwd and select id 1 "slave" and go to realtime data and activate sampling I get a still graph "not moving" is this normal? 
It begins to move if I connect back to master! 
Any suggestions
```

---
## \#2 Posted by: Sander Posted at: 2017-02-11T20:06:58.816Z Reads: 404

```
Im not an expert but I think that the master should be id 0, so the :
[quote="WARMAN, post:1, topic:17565"]
Send status over can disabled "not ticked"
[/quote]
Should be ticked.

And the id 1 not ticked.
And can I see how you have connected it?
```

---
## \#3 Posted by: WARMAN Posted at: 2017-02-11T23:35:24.814Z Reads: 390

```
Yeah the master is set to id 0 and I thought that send status over can was supposed to be ticked on the slave to receive signal and Mutiple esc over can ticked on the master to send signal.
Anyway tried to switch with the send status over can enabled on master and not the slave no luck! 
Also tried switching the Mutiple esc over can from master to slave no luck! 
What did you want to see the conections of?
```

---
## \#4 Posted by: Sander Posted at: 2017-02-11T23:42:29.760Z Reads: 371

```
[quote="WARMAN, post:3, topic:17565"]
What did you want to see the conections of?
[/quote]

The wiring of the VESC with Dual setup, the two wires that goes on the CAN bus.
Have the Multiple ESC on and send over can too on the id 0
```

---
## \#5 Posted by: WARMAN Posted at: 2017-02-12T00:00:08.664Z Reads: 359

```
<img src="/uploads/db1493/original/3X/2/3/231ee969ee04091b6eedda8d67754c8dc813c0d4.jpg" width="690" height="388">
```

---
## \#6 Posted by: WARMAN Posted at: 2017-02-12T00:05:40.368Z Reads: 348

```
[quote="Sander, post:4, topic:17565"]
Have the Multiple ESC on and send over can too on the id 0
[/quote]

Done that id 0 that's the master now have them both on what about the slave id 1
```

---
## \#7 Posted by: Sander Posted at: 2017-02-12T00:09:18.440Z Reads: 342

```
[quote="WARMAN, post:6, topic:17565"]
Done that id 0 that's the master now have them both on what about the slave id 1
[/quote]

Let me check my dual setup brb
```

---
## \#8 Posted by: Sander Posted at: 2017-02-12T00:14:42.838Z Reads: 338

```
What is your rate(hz) on _Send Status Over Can_?
```

---
## \#9 Posted by: WARMAN Posted at: 2017-02-12T00:16:25.866Z Reads: 333

```
500
10 characters
```

---
## \#10 Posted by: Sander Posted at: 2017-02-12T00:18:07.800Z Reads: 325

```
On the ID 1 I have the same thing as the ID 0 but I havent Send Status checked on id 1 nor in PPM in control mode disabled
```

---
## \#11 Posted by: Ackmaniac Posted at: 2017-02-12T00:22:56.804Z Reads: 321

```
The problem is that you have selected PPM and UART and the slave VESC. Set it to None at the Slave.PPM should only be active at the Master.
```

---
## \#12 Posted by: WARMAN Posted at: 2017-02-12T00:24:45.212Z Reads: 309

```
So Mutiple esc over can ticked on both master and slave and send status over can only ticked on master that's what I now have setup no luck
```

---
## \#13 Posted by: Sander Posted at: 2017-02-12T00:26:17.141Z Reads: 301

```
[quote="WARMAN, post:12, topic:17565, full:true"]
So Mutiple esc over can ticked on both master and slave and send status over can only ticked on master that's what I now have setup no luck
[/quote]

Like @Ackmaniac said, on the Slave set the App to No app
```

---
## \#14 Posted by: WARMAN Posted at: 2017-02-12T00:29:45.521Z Reads: 279

```
Now have that done still nothing 
Does your graph move on realtime data when you test canbus connection via can fwd and selecting id  of slave vesc
```

---
## \#15 Posted by: WARMAN Posted at: 2017-02-12T00:31:51.669Z Reads: 278

```
I read in a thread from @onloop that ppm should be activated on both anyway it's just on the master at the minute still no joy
```

---
## \#16 Posted by: Ackmaniac Posted at: 2017-02-12T00:35:03.213Z Reads: 271

```
You have to select "No app".
Then write the configuration.
Then reboot the Vesc. (Press the reboot button or switch off the power and switch it back on)
Without a reboot the Application switch doesn't work.
```

---
## \#17 Posted by: Ackmaniac Posted at: 2017-02-12T00:36:12.003Z Reads: 271

```
And if it is still not working then please post screenshots of the General and PPM Tab of the Master and Slave.
```

---
## \#18 Posted by: WARMAN Posted at: 2017-02-12T00:38:03.860Z Reads: 267

```
Yeah I did that selected no app on slave write configuration turned off and on still nothing will take some pictures
```

---
## \#19 Posted by: WARMAN Posted at: 2017-02-12T00:44:01.882Z Reads: 273

```
These first two pictures are master settings for app general and ppm 
<img src="/uploads/db1493/original/3X/0/4/04ed99bf84a9487a4224edefc9fa4833f882e0c9.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/a/2/a23d1958f08a5387a2d29c6175907135d2f3b23a.jpg" width="690" height="388">
```

---
## \#20 Posted by: WARMAN Posted at: 2017-02-12T00:46:26.889Z Reads: 261

```
Same again but for slave 
<img src="/uploads/db1493/original/3X/c/a/ca6d64a19db8da02623fbdd1de01c99afe7e8739.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/7/6/767c7bb5d8558cb33a24b55816a631c1fc71e436.jpg" width="690" height="388">
```

---
## \#21 Posted by: Ackmaniac Posted at: 2017-02-12T00:50:58.112Z Reads: 244

```
There we go. Disable "Send sttaus over CAN" at the Master and enable it at the slave. Don't forget the reboot for both. Have fun
```

---
## \#22 Posted by: WARMAN Posted at: 2017-02-12T00:59:15.121Z Reads: 243

```
Yeah that's what I did have it set as originally 
I now have it so send status over can is on slave and not master like you said..reboot still only one spins up? 
It's got to be a setting as motor detection works!
```

---
## \#23 Posted by: Ackmaniac Posted at: 2017-02-12T01:09:48.735Z Reads: 242

```
Go to the Terminal Tab on the Master and type in can_devs
What does it show?

Seems that your CAN cable doesn't have a solid connection or the VESCs have a issue with the CAN ports.
```

---
## \#24 Posted by: WARMAN Posted at: 2017-02-12T01:16:28.009Z Reads: 238

```
<img src="/uploads/db1493/original/3X/2/a/2ad372a82a4adc106f1cf51fc8892ac959533363.jpg" width="690" height="388">
```

---
## \#25 Posted by: Ackmaniac Posted at: 2017-02-12T01:19:12.259Z Reads: 223

```
If you have "Send status over CAN" enabked at the Slave and don't see anything with this command then they can't communicate with each other. Check the CAN wire with a multimeter. And where did you get the VESC from.
```

---
## \#26 Posted by: WARMAN Posted at: 2017-02-12T01:23:46.736Z Reads: 219

```
Vesc is from diy.com
It must be the canbus conections I'll check now
```

---
## \#27 Posted by: WARMAN Posted at: 2017-02-12T01:31:51.482Z Reads: 213

```
Disconnected the canbus from the slave and tested that end with a multimeter nothing! will try wire it again tomo it's 1:30 am here,even though my board lights up like a Christmas tree it's freezing will have to wait till tomorrow thanks for your help @Ackmaniac
```

---
## \#28 Posted by: WARMAN Posted at: 2017-02-12T01:32:50.720Z Reads: 214

```
And @Sander cheers Bro
```

---
## \#29 Posted by: Ackmaniac Posted at: 2017-02-12T01:33:51.898Z Reads: 214

```
I mean test with the multimeter the connection from one side to the other. The mode when the multimeter makes a beep when a electrical connection exists.
```

---
## \#30 Posted by: WARMAN Posted at: 2017-02-12T01:46:05.457Z Reads: 215

```
Yeah there's power between them must be the jst
```

---
## \#31 Posted by: Eboosted Posted at: 2017-02-12T04:35:29.353Z Reads: 213

```
Are you trying to spin both with the arrow keys on the keyboard? 

If you do that you will always spin only one motor, I'd also suggest to flash the ackmaniac firmware if you don't have any other recommended solution to test
```

---
## \#32 Posted by: halifax21 Posted at: 2017-02-12T06:47:24.900Z Reads: 215

```
Try this:

On the **Master VESC** - the one with the remote receiver on it

1. Plug in the cable, press connect then press "Read Configuration"

1. Select "App Configuration" then "General" on the left, set the Controller ID value to 10

1. If you are using "PPM", select "Multiple ESC's over Can" & set the Control Mode to "Duty Cycle no reverse" then press "Write Configuration"

1. Ensure that all the other control modes "ADC & Nunchuck" are disabled then press "Write Configuration"

1. Test your controller, only the master motor should spin.


**Now for the Slave VESC**

1. Plug in the cable, press connect then press "Read Configuration"

1. Select "App Configuration" then "General" on the left, set the Controller ID value to 2

1. On the General tab, set APP to use to **No app**, then press "Write Configuration" then press reboot

1. On the PPM tab, set the Control Mode to "Duty Cycle no reverse" & select "Multiple ESC's over Can", then press "Write Configuration"

1. Ensure that all the other control modes "ADC & Nunchuck" are disabled then press "Write Configuration"

1. Test your controller, both motors should be spinning

One major difference is I'm on "Duty Cycle no reverse" where you are using "Current no reverse with brake" give that a change
```

---
## \#33 Posted by: WARMAN Posted at: 2017-02-12T15:12:29.412Z Reads: 196

```
So i changed the jst lead still nothing @halifax21 thanks man did all the above changed controller ids to 2 and 10 if I change to duty cycle my motor acts weird pull the throttle and nothing then few seconds later full throttle! where as current with no reverse works responsive but have hardly any brake.
Still can't get it to spin dual after reboot iv run out of ideas!
```

---
## \#34 Posted by: Ackmaniac Posted at: 2017-02-12T15:38:18.861Z Reads: 197

```
Seems that something is wrong with your VESCs.
Last thing that comes to my mind is that you might have different Firmware versions but you use the same Version of BLDC-tool for it so it also should be fine. Last chance is to upgrade to version 2.18 from the official source or to my firmware and try it with that, But i don't think that it will help.
I think on one of your VESC's the CAN pins don't work.
```

---
## \#35 Posted by: WARMAN Posted at: 2017-02-12T15:43:22.665Z Reads: 200

```
Both vesc are running firmware version 2.18 luckly I have 5 more vesc's at my work unit that i bought from diy.com will pop down there now and grab another if that works then must be the vesc if not I'll go over the settings again with a fine tooth comb!
```

---
## \#36 Posted by: WARMAN Posted at: 2017-02-12T16:36:04.540Z Reads: 194

```
@Ackmaniac you were right it's the vesc's replaced both now have dual wheel drive but the slave spins the motor the wrong way?
```

---
## \#37 Posted by: Ackmaniac Posted at: 2017-02-12T16:37:40.268Z Reads: 190

```
Just switch any 2 of the 3 phase wires. Then the motor will spin the other way.
```

---
## \#38 Posted by: WARMAN Posted at: 2017-02-12T16:43:06.490Z Reads: 187

```
Thanks for the help @Ackmaniac @halifax21 got there in the end! 
Not sure where I stand with returning the vesc's to diy.com hopefully I'm covered as they work on there own just not the canbus!
```

---
## \#39 Posted by: psychotiller Posted at: 2017-02-14T17:12:39.373Z Reads: 182

```
Why not just use a receiver splitter wire? The canbus is just a complication.
```

---
## \#40 Posted by: WARMAN Posted at: 2017-02-14T17:38:20.860Z Reads: 183

```
Yeah I'm starting to realise that I have multiple vescs that the canbus doesn't work on but luckly  now have two that communicate im just gona put the others in single wheel drive boards.
```

---
## \#41 Posted by: psychotiller Posted at: 2017-02-14T17:47:55.609Z Reads: 172

```
The master/slave scenario is so 80's haha
```

---
## \#42 Posted by: Ackmaniac Posted at: 2017-02-14T18:40:52.751Z Reads: 172

```
Well it's good for traction control and advanced cruise control or to update multiple vescs with a now drive mode via smartphone app.
```

---
## \#43 Posted by: MustardTiger Posted at: 2017-12-22T20:12:03.563Z Reads: 116

```
I’m upgrading to dual motors and I plan on going the splitter route. Do you have to use any reduced vesc setting values or do I just copy the values I have on my original vesc?
```

---
## \#44 Posted by: Colson003 Posted at: 2017-12-22T20:14:25.853Z Reads: 116

```
Simplest thing to do is half your battery max and min
```

---
## \#45 Posted by: MustardTiger Posted at: 2017-12-22T20:33:21.340Z Reads: 111

```
Thanks for the advice. Will this reduce my performance?
```

---
## \#46 Posted by: Colson003 Posted at: 2017-12-22T20:38:17.161Z Reads: 111

```
No. You'll have dual motors. 
Use the search function for a better explanation
```

---
## \#47 Posted by: psychotiller Posted at: 2017-12-22T21:18:34.207Z Reads: 109

```
The guys are right! Not sure what you have your motor amps at, but most likely you can up those values too.
```

---
## \#48 Posted by: MustardTiger Posted at: 2017-12-23T19:49:33.402Z Reads: 99

```
Motor max 90
Motor min 50
Batt max 35(was 70 with single motor)
Batt min -12

63/74
12s lipo
```

---
## \#49 Posted by: Colson003 Posted at: 2017-12-24T00:11:19.286Z Reads: 91

```
What was your battery min before?
Motor min is -50 right?
```

---
## \#50 Posted by: MustardTiger Posted at: 2017-12-24T04:03:11.399Z Reads: 86

```
Yeah -50 motor min batt min was -14 with single motor
```

---
