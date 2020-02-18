# Metr Pro UNITY bluetooth module

### Replies: 45 Views: 2119

## \#1 Posted by: rpasichnyk Posted at: 2019-05-30T17:59:33.181Z Reads: 363

```
Fellow master builders!

We are happy to announce **Metr Pro UNITY** edition. It has been in the works since the beginning of this year and is finally ready!

The most important feature is **EASY INSTALL**
https://giphy.com/gifs/eKCrMsVRbow2d2974s

**INSTRUCTIONS:**
1. Lift up UNITY rubber case
2. Remove factory BLE module
3. Insert Metr Pro
4. ???
5. PROFIT!!!

Metr Pro UNITY has a newer nRF52840 chip from Nordic. Otherwise it is the same good and proven Metr Pro module. It works as you would expect, just in a different form factor:

* :alien: Firmware Over-The-Air updates
* :lock: BLE security with Elliptic Curve Cryptography and Man-in-the-Middle protection
* :hammer: BAUD rate and RX/TX autodetection, plug and play
* :shield: Metal shield and 3-LED status indication
* :peace_symbol: Works with many apps (Metr, UNITY, Xmatic)

![metrprounity|690x458,75%](upload://xIGaKsprKsPfstporIVsA6YavLr.jpeg) 

http://metr.at/shop PRICE: €50 (+19% VAT for EU)

We are getting feedback from our beta testers @mackann @StefanMe @janpom and so far only found one software issue that we want to fix before shipping the modules to everyone. This is purely software, the hardware is ready. We expect to ship the modules next week.
```

---
## \#2 Posted by: niuva Posted at: 2019-05-30T19:27:22.338Z Reads: 302

```
As someone who has serious issues with the stock Unity Bluetooth module freezing / crashing due to voltage spikes, the Metr module looks very appealing and I'm close to ordering one. 
You posted a closeup shot of the PCB in the other Metr Pro thread and I noticed you had two ceramic caps between GND and VCC. Is this enough to smooth out the voltage and keep the module from crashing/freezing? Have you taken this into consideration when designing this?

Bit hesitant to place the order, since not sure if the Unity stock Bluetooth module is just trash or if it is an issue with the Unity itself and if buying a Metr module would even fix it. Obviously having access to all the great Metr features is something I'm very much looking forward to. :slight_smile:

https://www.electric-skateboard.builders/t/focbox-unity-official/64944/2592?u=scream
```

---
## \#3 Posted by: hexakopter Posted at: 2019-05-30T20:14:28.603Z Reads: 266

```
We have not experienced any crashes of the module so far. As you mentioned both caps very close to the nRF52840 module should help a lot smoothing out some spikes. We have to wait for some more results form our beta testers, but so far it is looking good. I am waiting for a FOCBOX UNITY myself for some month for more electrical analysis and scope the 3.3V for an example, but not sure if Enertion is holding their shipping dates now. They already delayed the announced date to ship them a few times.

I will keep you updated with results from our beta tester. I know @janpom experienced these crashes with the OEM UNITY BT module also and should have the new Metr Pro UNITY in his hands very soon. Post delayed the shipping of his beta module a bit.
```

---
## \#5 Posted by: McErono Posted at: 2019-05-30T21:14:46.114Z Reads: 240

```
Ordered! I will report about stability asap (hopefully end of next week).
```

---
## \#6 Posted by: niuva Posted at: 2019-05-30T21:26:30.137Z Reads: 234

```
@McErono  Just out of curiosity, have you experienced forementioned bluetooth freezes with the Unity stock BT module?
```

---
## \#7 Posted by: McErono Posted at: 2019-05-30T22:50:52.526Z Reads: 232

```
Yes all the time but since firmware 23.44 it got a lot better.
```

---
## \#8 Posted by: Ixf Posted at: 2019-05-30T22:59:59.413Z Reads: 230

```
purchased.  WOOT
```

---
## \#9 Posted by: Martin Posted at: 2019-05-31T01:53:58.815Z Reads: 223

```
I ordered two module( Metr Pro UNITY bluetooth module and Metr Pro bluetooth module)
I sent additional shipping information by e-mail.
Check please!!!!
```

---
## \#10 Posted by: nuttyjeff Posted at: 2019-05-31T04:38:43.622Z Reads: 212

```
It still has a password like your normal metr modules yeah? I got 2 because the unity lacks this security feature.
```

---
## \#11 Posted by: hexakopter Posted at: 2019-05-31T06:21:26.132Z Reads: 206

```
@Martin Received your payment. Thanks. Also received your shipping information already via PayPal, but thanks for sending it via e-mail again so I can confirm you we have it right.

@nuttyjeff Yes, it still features BLE security with Elliptic Curve Cryptography and Man-in-the-Middle protection, so you have a 6 digit password like on standard Metr Pro modules.
```

---
## \#12 Posted by: nuttyjeff Posted at: 2019-05-31T06:42:29.339Z Reads: 200

```
[quote="hexakopter, post:11, topic:95494"]
you have a 6 digit password like on standard Metr Pro modules.
[/quote]

Cool. Already placed my order. Thanks!
```

---
## \#13 Posted by: Crashtest Posted at: 2019-05-31T21:48:15.876Z Reads: 186

```
I've been eyeing up a Focbox unity but loved my metr pro, i can now upgrade woooo! Good work guys you produce the best module / app. Thank you
```

---
## \#14 Posted by: Moros Posted at: 2019-05-31T22:07:37.202Z Reads: 189

```
Interested in getting one of these for a cleaner look but I've already got a brand new never used Metr Pro bluetooth module.  I upgraded my focboxs to a unity before I got around to installing it so if anyone in the EU is interested in a new Metr Pro bluetooth module, send me a pm.
```

---
## \#15 Posted by: hexakopter Posted at: 2019-06-06T21:27:54.710Z Reads: 179

```
First Metr Pro UNITY modules are completely assembled and each of them tested, so first orders will be shipped tomorrow. You will receive the tracking number via PayPal when your package is send.
![Metr_Pro_UNITY_2|690x458](upload://eqxhtKUpiNzAKxXnZRbPM3NslYo.jpeg) 

To install the module follow the video and steps Roman posted.

[quote="rpasichnyk, post:1, topic:95494"]
![](https://media.giphy.com/media/eKCrMsVRbow2d2974s/giphy.gif)

**INSTRUCTIONS:**

1. Lift up UNITY rubber case
2. Remove factory BLE module
3. Insert Metr Pro
4. ???
5. PROFIT!!!
[/quote]

We recommend turning off the FOCBOX UNITY when you switch the OEM module for the new Metr Pro one. Make sure you plug the 2x3 pin header to the right spot of the internal connector where the old module was sitting before. Turn the UNITY on after confirming its plugged in correctly.

Each Metr Pro UNITY comes with its own pairing pin code like you can see in the following picture.
![Metr_Pro_UNITY_pincode|690x458](upload://1rLR4nnhTGRjXt2BSpUnARTIkoE.jpeg) 
Please note down your pairing code before closing your boards enclosure so you have it ready for first time connecting to the metr app. To connect to the module go to "Settings", hit the scan button and tab on your Metr Pro module thats shown in the list. You are asked to put in the 6 digit code. Its only necessary to put in the code ones, so afterwards your phone will directly connect to the module when opening the app.
Set up your wheel diameter, motor poles etc. under "Settings" -> "Motor" and your battery settings under "Settings" -> "Battery" and you are ready to go. Start records, see realtime data, use modes, change ESC settings and **enjoy your ride**.:slightly_smiling_face:
```

---
## \#16 Posted by: janpom Posted at: 2019-06-06T22:24:12.383Z Reads: 173

```
I was able to test the Metr Unity module today. I did have freezing issues with the stock Unity BT module and Xmatic. In Xmatic, the freezing still happens with the Metr module. However, the Metr module has been working flawlessly with the Metr app. I recorded a 17km test ride. There's no indication of any connection dropouts in the log. Here it is:

https://metr.at/r/eCcR3

The idle sections are where I know I have actually stopped for a short break. You can also tell that the FET temperature went down during the breaks. Clearly not a connection loss.
```

---
## \#17 Posted by: hexakopter Posted at: 2019-06-07T20:42:18.445Z Reads: 168

```
[quote="hexakopter, post:15, topic:95494"]
First Metr Pro UNITY modules are completely assembled and each of them tested, so first orders will be shipped tomorrow.
[/quote]


Quick follow up. All orders [s]placed before 04 June 2019[/s] are shipped now. You should receive the tracking number via PayPal. Use [this website](https://www.deutschepost.de/sendung/simpleQuery.html?locale=en_GB) to track the package.
```

---
## \#18 Posted by: 701Superjet Posted at: 2019-06-07T23:33:39.344Z Reads: 162

```
Ordered! I sent you an email with my shipping address. Paypal was not updated after my recent move. I look forward to tying it out!!!
```

---
## \#19 Posted by: hexakopter Posted at: 2019-06-08T07:07:44.062Z Reads: 156

```
Got your email with new shipping address and updated it.
```

---
## \#20 Posted by: 701Superjet Posted at: 2019-06-08T10:48:17.083Z Reads: 151

```
Thank you!
```

---
## \#21 Posted by: McErono Posted at: 2019-06-14T09:04:38.743Z Reads: 147

```
my module arrived yesterday, will test it over the weekend! :star_struck:
```

---
## \#22 Posted by: rsalmon Posted at: 2019-06-14T17:33:56.672Z Reads: 131

```
My tracking number isn't even updating yet :frowning:
```

---
## \#23 Posted by: hexakopter Posted at: 2019-06-15T19:27:58.940Z Reads: 129

```
I checked your tracking number. It says it was handed over to the International Logistics Center on 08.06.2019. Packages shipped on the same day to the US are already there since a few days. So I guess it should be in Canada very soon. Hope you will receive it in the next days.
```

---
## \#24 Posted by: McErono Posted at: 2019-06-15T21:07:30.270Z Reads: 125

```
Installed it and it is working flawlessly so far. :+1:
```

---
## \#25 Posted by: McErono Posted at: 2019-06-16T19:51:38.822Z Reads: 121

```
Found one issue: I can not connect to the Unity app, it crashes or freezes and wont connect. It finds the module in the BT scan tho.
```

---
## \#26 Posted by: hexakopter Posted at: 2019-06-21T19:20:17.489Z Reads: 114

```
For the people not following both forums. The problem @McErono was talking about is fixed since some days.

https://forum./t/metr-pro-unity-bluetooth-module/1383/35
```

---
## \#27 Posted by: McErono Posted at: 2019-06-21T19:27:13.570Z Reads: 111

```
Yes firmware 4.7 is fine so far for me! :+1:
```

---
## \#28 Posted by: drone001 Posted at: 2019-06-22T15:48:42.476Z Reads: 114

```
I ordered one.....trying to save money but these esk8 parts keep calling me maaan!!! they just keep calling...they never stop calling me maaaan!!!
```

---
## \#29 Posted by: 701Superjet Posted at: 2019-06-28T17:00:19.714Z Reads: 102

```
This thing rocks!! Thank you!
```

---
## \#30 Posted by: Silverline Posted at: 2019-06-28T21:24:46.380Z Reads: 99

```
Any plans for Samsung smartwatch support (Tizen OS ) ??
```

---
## \#31 Posted by: NineLives Posted at: 2019-07-06T18:50:32.520Z Reads: 96

```
Hi,
I need some help please. I have fitted my Metr Pro UNITY and updated the firmware to 4.9. When in real time mode it shows it is connected with the little green circle with a cross in it but it doesn't show any real time data all the values here remain at 0 while revving the motors. The App shows no device connected under expert. The unit itself has a slowly flashing blue light and a rapidly flashing green light. Is there anything I can try to get this working? Thank You.
```

---
## \#32 Posted by: rpasichnyk Posted at: 2019-07-06T19:07:06.387Z Reads: 95

```
Rapidly flashing green light indicates that Metr Pro is unable to connect UART. This is strange. Try to power cycle UNITY
```

---
## \#33 Posted by: NineLives Posted at: 2019-07-06T19:14:12.518Z Reads: 94

```
Hi, Thank you rpasichnyk. I have tried rebooting the Unity many times but always the same rapidly flashing light. Baud rate on the Unity is set to 115200. Metr settigns as bellow
![image|281x500](upload://uNLfQQsc32ixbdXn5FaMHGjtYSe.jpeg)
```

---
## \#34 Posted by: rpasichnyk Posted at: 2019-07-06T19:17:32.575Z Reads: 90

```
If the green light is flashing rapidly, doesn’t matter what settings are. Maybe you plugged it wrong? Do you have factory UNITY module? Does it work?
```

---
## \#35 Posted by: NineLives Posted at: 2019-07-06T19:29:32.235Z Reads: 91

```
Hi Rpasichnyk, I have just swapped back to the Unity module and it works fine App connected straight way and shows input on the HUD when revving the motors. I tried the Metr Pro UNITY again and same rapidly flashing green light.
```

---
## \#36 Posted by: rpasichnyk Posted at: 2019-07-07T06:14:57.318Z Reads: 91

```
Please turn your board off, then run Metr app, power on your board and wait until green light flashes rapidly, go to Settings -> Show Logs and send to support@metr.at

We will have a look at the logs, then we may try another firmware update, if it doesn't help you will have to send the unit back for replacement.
```

---
## \#37 Posted by: NineLives Posted at: 2019-07-07T10:43:02.098Z Reads: 90

```
[quote="rpasichnyk, post:36, topic:95494"]
support@metr.at
[/quote]

Thank you for you continued help I have sent the logs as requested.
```

---
## \#38 Posted by: NineLives Posted at: 2019-07-10T19:33:15.229Z Reads: 86

```
Hi rpasichnyk. Just wondering if you received the logs I sent you and have anything further I can try?
```

---
## \#39 Posted by: rpasichnyk Posted at: 2019-07-12T07:26:24.586Z Reads: 81

```
Yes, please try this firmware. I recommend using USB cable and FOCBOX Tool. The only change I did to this firmware is change baud rate from 250k to 115200. It is not possible to change baud rate for internal BLE module via tool, since it's hardcoded. 

https://www.icloud.com/iclouddrive/0pnwaB-qs0BrIiF6OQYkH00QA#UNITY_23_44_btuart115200

There is a problem with UNITY and 250k baud rate (with all BLE modules) which I will inform about soon.
```

---
## \#40 Posted by: NineLives Posted at: 2019-07-20T21:21:30.631Z Reads: 76

```
Hi rpasichnyk, Sorry for the late reply I have been unwell. I have tried the firmware update with the FOCBOX tool but I am unable to change from the unity.bin file to the one you provided for me to download. Do you know how to do this as I can see how to change this unless you add it as a custom file under the custom file tab tab?
```

---
## \#41 Posted by: NineLives Posted at: 2019-07-20T21:55:08.114Z Reads: 75

```
Hi Rpasichnyk, Further to having to use custom unity firmware to get this working I don't understand why it would just be effecting me could you please explain why only I need this change?
```

---
## \#42 Posted by: Ixf Posted at: 2019-08-14T11:26:36.715Z Reads: 64

```
@rpasichnyk @hexakopter I am also have the same issue @NineLives is having.
I was able to load up the custom firmware.
Right now there are two issues I am encountering

* Metr pro module flashes green and blue quickly.  Iphone app says connected but no data or setting is being sent
* Unity is having trouble configuring through USB with Metr installed on the comm port.  Removing the module resolves this issue

Please advise
```

---
## \#43 Posted by: rpasichnyk Posted at: 2019-08-14T11:39:00.793Z Reads: 62

```
You have Metr Pro UNITY right? This one?

![metrprounity|690x459, 50%](upload://z5fnMcpYhQGQweyEFPnq94R61d2.jpeg)
```

---
## \#44 Posted by: Ixf Posted at: 2019-08-14T14:57:14.866Z Reads: 63

```
Thats correct!
```

---
## \#45 Posted by: rpasichnyk Posted at: 2019-08-15T06:48:58.019Z Reads: 59

```
Was it always blinking rapidly (green LED)? I don’t know how that is possible, maybe you plugged it wrong? Or something is broken. Green blinking means that UART can not be established
```

---
## \#46 Posted by: Ixf Posted at: 2019-08-15T11:30:11.215Z Reads: 58

```
It used to work.

It stopped working after I applied the new custom firmware.

I had to remove the module, apply new firmware, config unity then put the module back since unity doesn't seem to save setting when the module is installed.

Now it isn't working even when i reverted back to the old firmware.
```

---
