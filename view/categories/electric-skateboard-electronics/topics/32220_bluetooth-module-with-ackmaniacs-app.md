# Bluetooth module with Ackmaniac&rsquo;s app

### Replies: 55 Views: 4585

## \#1 Posted by: Bloop Posted at: 2017-09-04T07:44:56.664Z Reads: 513

```
Hello guys,
I want to use Ackmaniac's android application and I got a HM-10 module from a local dealer and it looks like is just the Clone one..  (not the clone of clone) So i figured it should be ok. But i cannot see it in your application no matter what i tried.

I see the module in bluetooth settings of my phone: is the BT05.

When i open the application i see Device V1.52 and in right part scan / stop but is not finding anything else. Any idea on that ? Do i need to flash another firmware on the BLE module ? or that wont help.

Thank you. (i have Ackmaniac's firmware on my vesc too) Maybe someone have any experience with these clones ?
```

---
## \#2 Posted by: JdogAwesome Posted at: 2017-09-04T07:58:23.891Z Reads: 487

```
I'm using a cheap HM-10 Module as well hooked up to my VESC over the UART port and it's working fine. @Ackmaniac maybe you have some advice for  @Bloop.
```

---
## \#3 Posted by: Bloop Posted at: 2017-09-04T08:00:26.748Z Reads: 479

```
I talked with Ackmaniac and he said to use the one he linked and i will but it will take a few more weeks till i get that. 

Wondering if anyone else had similar problems and maybe have some advices ?
```

---
## \#4 Posted by: ShutterShock Posted at: 2017-09-04T08:24:50.385Z Reads: 461

```
I got this exact one, soldered the wires from my connector to the bluetooth module, and it works great, no problems at all.  I made sure to insulate each connection with heat shrink as well.

https://www.aliexpress.com/item/HM-10-BLE-Bluetooth-4-0-CC2540-CC2541-Serial-Wireless-Module/32516357718.html?spm=a2g0s.9042311.0.0.W5u6hT
```

---
## \#5 Posted by: Maxid Posted at: 2017-09-04T08:31:31.632Z Reads: 443

```
All you can do is:
1) tx and rx need to be crossed
2) 5V should be used instead of 3.3V
3) correct baud rate in the Vesc settings needs to be set (maybe your module has a different default instead of the 9600 - you could check via AT serial commands)
```

---
## \#6 Posted by: Bloop Posted at: 2017-09-04T08:45:02.524Z Reads: 421

```
I connected at 5v also tx rx are crossed and the baud rate is at 9600 but the problem is not the transmission. The problem is that the app dont see the BLE module. And no idea how to solve that.
```

---
## \#7 Posted by: TarzanHBK Posted at: 2017-09-04T09:10:46.504Z Reads: 404

```
Some modules simply just don´t work with the vesc. So get the right one from a place with faster shipping times and change it ;)
You can find a picture of the correct version somewhere in the thread. Check that with the one you want to purchase to get the right one.
```

---
## \#8 Posted by: Bloop Posted at: 2017-09-04T09:17:31.814Z Reads: 392

```
Thats the point it looks right as the one in the thread :)) So it should be the right one :-?? .. no idea now maybe is a bad clone.. idk
```

---
## \#9 Posted by: TarzanHBK Posted at: 2017-09-04T09:48:15.163Z Reads: 379

```
last option is to check the modul with an other vesc, but it´s more likely the wrong clone
```

---
## \#10 Posted by: Sebike Posted at: 2017-09-11T21:16:59.207Z Reads: 358

```
Hijacking this thread since I seem to have a similar issue. I've got the HM-10 module that @Ackmaniac linked to and have it conected to the FOCBOX (3.3V). 

When scanning for it in the app it doesn't show up, however I can see the Bluetooth device in the phone's bluetooth settings under "available devices". 

With a different phone it shows up in the app.. Is there anything I can do to make it work on this phone?
```

---
## \#11 Posted by: Ackmaniac Posted at: 2017-09-11T21:18:00.607Z Reads: 342

```
Connect it to the 5V pin.
```

---
## \#12 Posted by: TarzanHBK Posted at: 2017-09-11T21:26:25.865Z Reads: 335

```
The marking on them is swapped isn´t it? 3,3V <>5V
```

---
## \#13 Posted by: Sebike Posted at: 2017-09-11T22:09:13.984Z Reads: 326

```
I just tried that but with same results. Won't show up in the app.
```

---
## \#14 Posted by: Bloop Posted at: 2017-09-11T22:15:36.402Z Reads: 326

```
not all phones have BLE tho... what phone are you using ? 

i still wait for the module that ackmaniac linked and hope for the best .. also got 2 focboxes.. let the fun beggin hopefully ill be able to make it work
```

---
## \#15 Posted by: Sebike Posted at: 2017-09-11T22:17:22.106Z Reads: 318

```
Sony Xperia Z3. I believe it does support BLE.
```

---
## \#16 Posted by: Bloop Posted at: 2017-09-11T22:23:22.435Z Reads: 311

```
get an app ble checker . not sure how good ia it but it should gove you some info. also i saw on internet that some users had peoblems with ble on xperia z3.
```

---
## \#17 Posted by: Sebike Posted at: 2017-09-11T22:56:19.870Z Reads: 313

```
Thanks. Ble checker said I have ble. I actually got it to kind of work. Removed the app and reinstalled it and then it worked until it lost connection (?) and never found the device.. I erased all data and cache memory in app manager and then it worked again. Hmm.. Don't really know what the problem is and if it's software or hardware related.
```

---
## \#18 Posted by: Bloop Posted at: 2017-09-12T05:24:09.732Z Reads: 306

```
well could you walk me through how you hqve it setup and all? i still dont have it running. You need to set the vesc to uart + ppm or it should see the module just by connecting it to the vesc? any more vesc settings exept baud rate?
```

---
## \#19 Posted by: Sebike Posted at: 2017-09-12T06:54:07.402Z Reads: 309

```
Don't know if vesc was needed to see the device, but I had it setup ppm+uart, baud rate 9600. 

Connected rx-tx tx-rx gnd-gnd vcc-5v. Removed app on my phone and reinstalled it. Restarted the phone and launched the app. If it didn't work try clearing app data and relaunch the app. 

I tried to connect again today and the app doesn't find the device at first. Only when I first erase all app data in android app manager will the app list Bluetooth devices and connect to the HM-10. 

Not the best solution, but the only way I can make it work. Sounds app related, doesn't it @Ackmaniac?
```

---
## \#20 Posted by: TarzanHBK Posted at: 2017-09-12T07:47:39.675Z Reads: 315

```
how about trying to run it on an other phone?
```

---
## \#21 Posted by: Sebike Posted at: 2017-09-12T08:02:58.535Z Reads: 301

```
It works fine on the Samsung galaxy s4 and when all app data are deleted on my Sony it works well as long as I don't disconnect... Using that other phone is no solution for me though, so if there's no other fix I'll have to live with either deleting app data before each ride, or just don't use this app. Too bad as it seems to be such a great app! :cry:
```

---
## \#22 Posted by: Ackmaniac Posted at: 2017-09-12T10:48:24.314Z Reads: 291

```
I guess you don't get a error message when the module isn't available anymore. Do you stop the app with the home button or by going backwards until the app closes?
```

---
## \#23 Posted by: Bloop Posted at: 2017-09-12T18:15:06.102Z Reads: 285

```
Hey i just got the module that Ackmaniac linked and tested. Is working just fine. Thank you very much you are the best.

Now i need to learn how to use it with a dual focbox setup. hopefully it wont be too hard .
```

---
## \#24 Posted by: Sebike Posted at: 2017-09-12T20:10:14.201Z Reads: 273

```
Ok. I believe I found the "bug" :smile: I realized the app doesn't list any Bluetooth devices unless gps is  turned on on the phone. As soon as gps is on, the BT devices show in the app! 😂 Thanks for the troubleshooting though!
```

---
## \#25 Posted by: Sebike Posted at: 2017-09-12T20:32:36.925Z Reads: 256

```
Working app. Donation on its way. @Ackmaniac
```

---
## \#26 Posted by: b264 Posted at: 2017-12-17T04:46:31.652Z Reads: 209

```
Where is the app?
```

---
## \#27 Posted by: b264 Posted at: 2017-12-17T05:06:30.995Z Reads: 202

```
[Found it](https://play.google.com/store/apps/details?id=ackmaniac.vescmonitor)

Also there is [a thread](https://www.electric-skateboard.builders/t/vesc-monitor-android-app/20888) on it
```

---
## \#28 Posted by: Trdolan03 Posted at: 2017-12-20T00:07:11.789Z Reads: 192

```
@Ackmaniac I open the app and connect the bluetooth but it says that the vesc is not connected. Any ideas?
```

---
## \#29 Posted by: Ackmaniac Posted at: 2017-12-20T00:42:55.874Z Reads: 187

```
Did you connect it correct to the vesc? 5V,  rx tx crossed and a baudrate of 9600? And you can also try to restart your smartphone.
```

---
## \#30 Posted by: Trdolan03 Posted at: 2017-12-20T00:45:58.100Z Reads: 173

```
Yes, all the wiring is correct. It seemed to work after I re uploaded your firmware but it has since gone unresponsive to the remote.
```

---
## \#31 Posted by: Ackmaniac Posted at: 2017-12-20T00:48:28.783Z Reads: 165

```
[quote="Trdolan03, post:30, topic:32220"]
but it has since gone unresponsive to the remote.
[/quote]

don't understand that.
```

---
## \#32 Posted by: Trdolan03 Posted at: 2017-12-20T00:49:10.793Z Reads: 162

```
The light doesn't turn blue when I pull the trigger and the motor doesn't spin. It did spin for the FOC detection though.
```

---
## \#33 Posted by: Ackmaniac Posted at: 2017-12-20T00:50:17.992Z Reads: 162

```
go through the remote settings. after the firmware update you have to do the entire setup again.
```

---
## \#34 Posted by: Trdolan03 Posted at: 2017-12-20T00:50:59.406Z Reads: 158

```
Ok, I will try that.
```

---
## \#35 Posted by: Trdolan03 Posted at: 2017-12-20T01:05:55.648Z Reads: 150

```
Should the app to use be ppm or ppm and uart?
```

---
## \#36 Posted by: Trdolan03 Posted at: 2017-12-20T01:29:34.961Z Reads: 150

```
I am back to square one. The remote is now running the motor but no data on the app.
```

---
## \#37 Posted by: Trdolan03 Posted at: 2017-12-20T02:00:08.881Z Reads: 149

```
I got everything working now. :wink:
```

---
## \#38 Posted by: Trdolan03 Posted at: 2017-12-20T07:09:04.959Z Reads: 152

```
@Ackmaniac I took the board for a test run and the app was amazing. I did notice that it never recorder max speed, only the current and GPS based speed.
```

---
## \#39 Posted by: RyuX Posted at: 2018-04-13T15:40:48.315Z Reads: 125

```
Hello.
I would like to use the Ackmaniac App.. I have a original metr.at bluetooth module which is detected by the App but all values will only display zero.
I get no error message when I connect however - but it will not show anything, no real time data etc. everything is only zero.

Can anyone help me out ?
I got the newest Ackmaniac Firmware on my VESC.

Have a good day
```

---
## \#40 Posted by: mmaner Posted at: 2018-04-13T15:43:51.129Z Reads: 132

```
Did you set the UART speed to 9600 baud?
```

---
## \#41 Posted by: RyuX Posted at: 2018-04-13T15:45:45.689Z Reads: 127

```
No because the metr.at bluetooth module instruction said I should keep it at 115200 baud. I will try to set it lower this evening. But a Side Note which is strange - the metr.at App also is not working (not displaying values) however I thought that could be because of the ackmaniac firmware that I run..
```

---
## \#42 Posted by: mmaner Posted at: 2018-04-13T15:46:35.032Z Reads: 124

```
The @Ackmaniac android app requires 9600, I'd start there
```

---
## \#43 Posted by: SeanHacker Posted at: 2018-04-13T15:47:14.684Z Reads: 122

```
If you're running Android O that could be the problem. I haven't gotten either the metr app or ack app running on O yet. I've had to revert to Android N.
```

---
## \#44 Posted by: RyuX Posted at: 2018-04-13T16:01:01.593Z Reads: 119

```
I run Android 5.0
So i should be good ?
```

---
## \#45 Posted by: SeanHacker Posted at: 2018-04-13T16:03:23.625Z Reads: 115

```
Hmmm... I'm not sure what the lowest version is able to be used. Might be 6.0 and up. @Ackmaniac would know.
```

---
## \#46 Posted by: RyuX Posted at: 2018-04-13T16:05:05.221Z Reads: 111

```
Well 5.0 already has BLE compatibility.. so it should.. i guess
```

---
## \#47 Posted by: RyuX Posted at: 2018-04-13T17:20:44.013Z Reads: 111

```
So 9600 baud also is not working :( Just tested it
```

---
## \#48 Posted by: Ackmaniac Posted at: 2018-04-13T17:28:37.818Z Reads: 113

```
Connect it to 5V and RX on Vesc to TX on module and TX on vesc to RX on module. Then you need a mode with uart. For example ppm with uart and a baudrate of 9600.
```

---
## \#49 Posted by: RyuX Posted at: 2018-04-15T14:00:06.366Z Reads: 110

```
Ahh man you are a saint.. I accidently thought that UART is always active.. so PPM + UART Mode fixed it.. even though I run 115200 bauds. Now both your App and the Metr.at app will work.. super happy.
Will i have problems with 115200 bauds though ? It looks like it works ?

Thanks again man
```

---
## \#50 Posted by: RyuX Posted at: 2018-04-15T15:21:44.321Z Reads: 109

```
One thing I wonder is how can I make the selected mode permanent ?
I would like to have a Slow Mode permanently when selected. But when I turn off and on the VESC then it will be back to default ?
Would be great to have it in the VESC permanently..
```

---
## \#51 Posted by: rich Posted at: 2018-04-15T16:43:41.380Z Reads: 108

```
For default use the same settings as you use for your "slow mode" and make an additional "fast mode", problem solved. 

It is normal that the vesc goes in default mode after restart.
```

---
## \#52 Posted by: RyuX Posted at: 2018-04-15T17:14:54.149Z Reads: 107

```
I thought of that too... would be more convenient the other way around for me though
```

---
## \#53 Posted by: Sebike Posted at: 2018-04-15T19:32:22.540Z Reads: 106

```
Isn't it that when you long press a mode it asks if you want this to be written to your vesc as your default mode?
```

---
## \#54 Posted by: Ackmaniac Posted at: 2018-04-15T20:55:34.801Z Reads: 95

```
Exactly.
10 Chars
```

---
## \#55 Posted by: RyuX Posted at: 2018-04-16T16:39:17.044Z Reads: 87

```
Works like a charm.. thanks so much
```

---
