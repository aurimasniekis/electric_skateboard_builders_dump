# \[Inactive\] Vesc android/iOS app

### Replies: 59 Views: 10453

## \#1 Posted by: jacobbloy Posted at: 2016-02-15T05:30:49.617Z Reads: 601

```
Hi buy after a lot of project coming to and end, I have low started again on my vesc bldc tool app for iOS and android, where I go stuck was Bluetooth connectivity, but Iv fixed this.
It now onto testing on different devices and then finishing the UI and back end.

Features:
Real time data and screen capture
Programming
Firmware update

Non of this is free and some times I have to buy hardware and contract some one to assist. So if any one has a kind heart you can make a donation on my website while downloading bldc tool for Windows or OSX<img src="/uploads/db1493/original/2X/1/1c9fd37e8c7bdc35da9efbb9913a205934d7d584.png" width="281" height="500"><img src="/uploads/db1493/original/2X/5/5dcfe10bc3f0f36d5d8bbf902a87cfed476dec7e.png" width="281" height="500"><img src="/uploads/db1493/original/2X/3/39d24873943c4b30f56d4d9f79c31a1fc1d61738.png" width="281" height="500"><img src="/uploads/db1493/original/2X/8/8735cb60d9d8e8db87db8951ac0f601f330e17ff.png" width="281" height="500"><img src="/uploads/db1493/original/2X/e/e214287ba79fbc1e0b699862db84a5a5735e941c.png" width="281" height="500">
```

---
## \#2 Posted by: trbt555 Posted at: 2016-02-15T05:57:30.181Z Reads: 499

```
That's simply brilliant !
This is what folks have been waiting for !
How does the BT connection work on the VESC side ?
When will you be far enough with the code to allow us to test ?
```

---
## \#3 Posted by: lox897 Posted at: 2016-02-15T06:52:01.656Z Reads: 491

```
Excellent! Will use this on my next build! Thanks @jacobbloy for the work you have done for the community!
```

---
## \#4 Posted by: jacobbloy Posted at: 2016-02-15T07:24:46.465Z Reads: 474

```
I will select a few to start testing. Bluetooth will work via spi I have it working with a similar setup as the nrf chip that is used for the wii nunchuck.
```

---
## \#5 Posted by: torqueboards Posted at: 2016-02-15T09:28:16.246Z Reads: 448

```
Congrats Jacob!

It's great to have you around in the community.
```

---
## \#6 Posted by: hexakopter Posted at: 2016-02-15T12:47:58.434Z Reads: 429

```
Great work you have done there. Thank you for all your work you have done to bring the VESCs to a wider number of user, with making the programming etc. easier for everyone.

Would you also share the source of the App for us who would compile there own application and maybe also implement some enhancements when they have time for?

Are you using a Wlan-module (like ESP 8266) or a bluetooth module to communicate to the VESC? BT4.0 would be needed for iOS when using bluetooth. (like the HM-10)
```

---
## \#7 Posted by: jacobbloy Posted at: 2016-02-15T13:03:44.444Z Reads: 393

```
Bluetooth 4.0, hm10 is only one of the chips you can use. Iv been using spi not uart at the moment.

And yes the UI for my app as been on GitHub for some time and I will keep it as open as possible
```

---
## \#8 Posted by: hexakopter Posted at: 2016-02-15T14:05:04.640Z Reads: 382

```
Mhh, you are sure using SPI? When I see it correct the HM-10 doesn't have SPI, just TX/RX (Uart). But good to know that it is open source.
When I am right there is the source of Jacob: [https://github.com/jacobbloy/BLDCAPP][1]


  [1]: https://github.com/jacobbloy/BLDCAPP
```

---
## \#9 Posted by: MonsterCoatings Posted at: 2016-02-15T17:51:04.650Z Reads: 380

```
This is really interesting topic that I would like to learn more on so I could use my phone SGN5 to control my board.
Any links that you can post so I can read up more?
Thanks in advance.
```

---
## \#10 Posted by: Blasto Posted at: 2016-02-15T20:03:53.911Z Reads: 373

```
For the ios app, will we require a JB or it will be on the app store?
```

---
## \#11 Posted by: jacobbloy Posted at: 2016-02-15T20:54:10.347Z Reads: 367

```
Your correct, I havnt been using hm10 Iv been using nrf51822 because it is multi protocol.

Yes it will be on the App Store
```

---
## \#12 Posted by: jacobbloy Posted at: 2016-03-13T01:47:22.824Z Reads: 345

```
https://youtu.be/KMicAg91HIc
```

---
## \#13 Posted by: Haimindo Posted at: 2016-04-01T12:33:36.877Z Reads: 331

```
Looking good! Do you have any list of hardware that one should get before you launch your app to the public?
```

---
## \#14 Posted by: jacobbloy Posted at: 2016-04-01T18:50:04.296Z Reads: 336

```
I'm trying to make it support as many ble modules as possible but we will soon see!
```

---
## \#15 Posted by: jacobbloy Posted at: 2016-04-01T22:25:27.584Z Reads: 334

```
Ok I have the BLE side of my iPhone and android app working as smooth as I feel that I can get it.

I need some pple to test and help debug the app with me! I need members who are experienced with updating firmware, and changing settings and that can easily discrible faults.
For iOS users I need your UDID to deploy the app to your phone, I need this via privet msg, if you don't know how to get your UDID with out Google then please don't reply to this.

For android users I can just send you the .apk

You will have to buy a HM-10 preferable genuine module. I have been using  http://www.tinyosshop.com/index.php?route=product/product&product_id=705
And they have lost of distributors you can get them locally.

You will need to plug the module in using default settings via the uart port on the vesc and set your vesc BAUD rate to 9600.
If you do not know how to do this with out asking please don't reply.
```

---
## \#16 Posted by: trbt555 Posted at: 2016-04-02T14:46:42.250Z Reads: 310

```
So this excludes all Nunchuck users I guess ?
I was hoping it would be a usb-bluetooth solution.
```

---
## \#17 Posted by: jacobbloy Posted at: 2016-04-02T15:14:01.411Z Reads: 308

```
if you have a twin vesc set up then you can have both the ble and nunchuk
```

---
## \#18 Posted by: trbt555 Posted at: 2016-04-02T18:04:22.530Z Reads: 306

```
Yeah but can you get data from both ?
```

---
## \#19 Posted by: kaywerks Posted at: 2016-04-03T07:21:22.903Z Reads: 317

```
Can you send me the .apk for Android. I will PM you my email.
```

---
## \#20 Posted by: lowGuido Posted at: 2016-04-04T07:26:34.865Z Reads: 322

```
I'll put my hand up for this. sounds like fun.
```

---
## \#21 Posted by: DeathCookies Posted at: 2016-04-04T07:30:46.006Z Reads: 312

```
I want to help too. I already wrote you a pm ;)
```

---
## \#22 Posted by: jacobbloy Posted at: 2016-04-07T12:40:50.321Z Reads: 325

```
today i added a way of controlling the vesc via the data log page.

its just a basic slider and i might add more functions later, but for know it makes the vesc think that it is getting nunchuk values so we get the benefit of ramping. i was testing it today with @onloop it has a few bugs with the slider but that was all so complicated but is now fixed.<img src="/uploads/db1493/original/2X/a/a6ce5e69e462220675284b89adcfb8d4c6c3f550.png" width="634" height="454"> 

i will hopefully add a video very soon, I'm fixing some bugs that need to be fixed before i share the app with better testers
```

---
## \#23 Posted by: DeathCookies Posted at: 2016-04-07T13:46:22.788Z Reads: 281

```
Like i said, i am actually a Software Developer. Maybe i can help you fixing the bugs?
```

---
## \#24 Posted by: jacobbloy Posted at: 2016-04-07T14:52:25.320Z Reads: 282

```
ok then, i just want to get it finished my self as i have been working on this for over a year now, and asked for help back then and didn't get any, now that i am not very long away from finishing i have had a lot of ppl asking for the source code, i just don't want to loose the time and money i have put into this before i even get to release it.
```

---
## \#25 Posted by: jacobbloy Posted at: 2016-04-07T14:53:25.519Z Reads: 271

```
i also don't want to hurt any one because i have missed some thing.
```

---
## \#26 Posted by: Adam0311 Posted at: 2016-04-07T15:34:16.244Z Reads: 275

```
Super excited to see this come out!
```

---
## \#27 Posted by: longhairedboy Posted at: 2016-04-07T17:28:37.509Z Reads: 280

```
yep, i'm up for this. I PMed my deets as well. Very excited to see data and do configs on my phone, especially while out riding. I'm planning to order the BT board this week if nothing wonderful happens.
```

---
## \#28 Posted by: DeathCookies Posted at: 2016-04-09T12:46:45.510Z Reads: 282

```
[quote="jacobbloy, post:15, topic:1374"]
You will need to plug the module in using default settings via the uart port on the vesc and set your vesc BAUD rate to 9600.
[/quote]

Well,
i will try to find the right ports on the connector myself but it would be good to see the wiring of the hm-10 module and the vesc uart plug.
```

---
## \#29 Posted by: jacobbloy Posted at: 2016-04-09T13:04:34.260Z Reads: 280

```
on the bottom of the vesc if you look next to the pins there will be little labels.

we want to use the RX,TX,VCC,GRD

basically its the same on the module but you swap the RX and TX so RX on the vesc goes to TX on the module, and TX on the vesc goes to RX on the module.

@DeathCookies i have sent you emails with a custom firmware for the version 4.10 vesc to allow write config and the latest .apk

but i have made a lot of ui fixes since i last sent you the .apk and i will send u another one tonight.
```

---
## \#30 Posted by: DeathCookies Posted at: 2016-04-09T13:31:44.406Z Reads: 271

```
Yeah, i already connected it like this way and setted "App Configuration" to use PPM (Receiver) and UART (HM-10). Also the Baudrate to 9600 but the i cannot find the hm-10 module in the app. My apporach: app --> settings --> scan --> it found nothing...

 Also i have a wrong firmware... when i install your firmware the bldc tool says 4.16 but i need 4.15 for my vesc.
```

---
## \#31 Posted by: jacobbloy Posted at: 2016-04-09T13:57:20.960Z Reads: 278

```
why do you need 4.15 for your vesc? 4.16 is the latest firmware version.

also there night be a few things that could be making it not find it, like your bluetooth is turned off in your phone settings.

or you module is set for master instead of slave.

or the SDK that i used for the building of the app

il have a look and can you please have a look
```

---
## \#32 Posted by: jacobbloy Posted at: 2016-04-09T14:18:15.034Z Reads: 278

```
there is an app on the android app store called BLE Scanner, if you download that and just see that you can find the module and if you can the connect and send me a screen shot of what it shows
```

---
## \#33 Posted by: DeathCookies Posted at: 2016-04-09T19:34:19.541Z Reads: 281

```
Now i got it sorted. It is working well. I wrote you a list of bugs i discovered ;)
```

---
## \#34 Posted by: BigAl Posted at: 2016-04-10T17:14:19.099Z Reads: 282

```
Hey Jacob, I sent my UDID and board is on it's way.

Al...
```

---
## \#35 Posted by: onloop Posted at: 2016-04-12T15:01:38.639Z Reads: 296

```
The new VESC PHONE APP got a Big Mention & Demo in my last VLOG. Check it.

https://www.youtube.com/watch?v=9LYkgey1dX0
```

---
## \#36 Posted by: Adam0311 Posted at: 2016-04-12T16:29:51.439Z Reads: 302

```
Looks awesome! Will the released version of this require a similar Bluetooth devise to be plugged into VESC?
```

---
## \#37 Posted by: jacobbloy Posted at: 2016-04-13T18:38:08.528Z Reads: 312

```
https://youtu.be/N98Oqr0WRG0

check out my video guys @onloop you will like this!
```

---
## \#38 Posted by: massy Posted at: 2016-04-16T20:24:36.211Z Reads: 314

```
Any plans on adding Android Wear support? Would be sick to have real time info on the wrist. Willing to help/build it as soon as I get my frickin board actually running as it should.
```

---
## \#39 Posted by: Workaround Posted at: 2016-07-27T13:56:37.657Z Reads: 283

```
I would like the apk file. I'm wondering why you have not uploaded it to github?
```

---
## \#40 Posted by: im-done Posted at: 2016-11-01T18:19:46.228Z Reads: 218

```
So I have the app and a Everton 4.12 vest how do I link the two?
```

---
## \#41 Posted by: mccloed Posted at: 2016-11-01T20:42:55.803Z Reads: 210

```
You need to get a Bluetooth module. I used the HM-10. This thread has the pin outs: http://www.electric-skateboard.builders/t/recording-data-from-vesc-summary-of-tools/7020/13
```

---
## \#42 Posted by: SageTX Posted at: 2016-11-01T21:08:42.904Z Reads: 212

```
Can 1 bt module and the app be used to change settings on dual vesc setup?
```

---
## \#43 Posted by: lox897 Posted at: 2016-12-04T10:07:17.807Z Reads: 186

```
Does this work with clone HM10s? The ones on ebay? @jacobbloy
```

---
## \#44 Posted by: Badrish Posted at: 2017-04-15T23:48:28.930Z Reads: 157

```
I tried using bluetooth to connect to my board but it didn't work. It was connected to my phone but he app couldn't sense it. Any ideas on how to fix it.
```

---
## \#45 Posted by: rpn314 Posted at: 2017-04-20T03:52:42.275Z Reads: 154

```
[quote="Badrish, post:44, topic:1374, full:true"]
I tried using bluetooth to connect to my board but it didn't work. It was connected to my phone but he app couldn't sense it. Any ideas on how to fix it
[/quote]

I've found this app to be quite buggy, so I frankly wouldn't rely on it very much.

But I'll try and help. What's the exact bluetooth module you're using?
```

---
## \#46 Posted by: SeanHacker Posted at: 2017-04-20T04:26:21.824Z Reads: 154

```
https://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286
```

---
## \#47 Posted by: Nordle Posted at: 2017-04-20T07:58:35.934Z Reads: 151

```
You should get in contact with that METR app guy, and make something beautiful together;)
```

---
## \#48 Posted by: Badrish Posted at: 2017-04-21T22:02:41.714Z Reads: 135

```
I have no clue. It was a prebuilt board
```

---
## \#49 Posted by: Marty Posted at: 2017-04-25T10:29:05.751Z Reads: 134

```
Great App - I love the Advanced overview page.
But I got one problem/question:
How the values in the "Settings" page of the App are stored ?
At every relaunch I have to type in my specs (Motor pulley, diameter, Battery Type, etc) new again.
Is there a way to store it ?
Thanks
```

---
## \#50 Posted by: Teilchen Posted at: 2017-06-17T13:01:15.438Z Reads: 116

```
Hey there, I am new on the forum, is this App still available? It seems I cannot PM anyone yet, so I decided to ask here, since I cannot find this app neither in US or Europe AppStore, do we still need to request it from Jacob directly? I have mi UDID ready :)
```

---
## \#51 Posted by: rpn314 Posted at: 2017-06-19T11:48:04.937Z Reads: 115

```
It does look like the app isn't available anymore, but I wouldn't recommend you use it anyways. It was quite buggy. I recommend Android users get @Ackmaniac's app. The links is a few posts above. Right now, there isn't a very good option for iOS users (in my opinion). metr.at and perimetr are both made by a guy on here, but he requires that you buy the bluetooth module from him.
```

---
## \#52 Posted by: Teilchen Posted at: 2017-06-19T12:34:37.323Z Reads: 115

```
Thanks, I have figured out, that metr and perimeter would be the best solution, but I have a bunch of HM10 modules already, and I find it a not-so-nice solution to buy a dedicated module. I would be happier to pay for the app, or only the margin he makes on selling these modules...

Anyways, I have been able to get my hands on an Android device, and have tried all available apps there, but with no success. I can connect to the HM10CONTROL, but it seems there is no communication with the FW. Tried different Bauds, etc.

If I understand it correctly, Arcmaniac's app needs a dedicated firmware, and it looks like I got myself a Maytech VESC, which are believed not to have the bootloader, so FW upgrade is not an option... I will try it later though...
```

---
## \#53 Posted by: Ackmaniac Posted at: 2017-06-19T12:47:13.059Z Reads: 117

```
You still can see the real time data and record videos. But you are not able to change the settings without my firmware mod.
```

---
## \#54 Posted by: Teilchen Posted at: 2017-06-19T12:58:22.267Z Reads: 118

```
Ok, thanks for the info. I was under the impression, that it needed something special, since your app did not find the HM10 device, whereas VESC Control does find it...
I guess I need to double check the HM10 settings... I recall something about Adafruit Uart Friend support? I will read your thread for information.
```

---
## \#55 Posted by: DeathCookies Posted at: 2017-06-19T14:15:17.784Z Reads: 118

```
To See the bt Module u need to turn on the Board and the remote!! Just after that u will See the Module in the App.... Sadly there is no Information about this @Ackmaniac
```

---
## \#56 Posted by: Teilchen Posted at: 2017-06-21T15:08:49.146Z Reads: 109

```
What do you mean by saying the Board and the Remote? I am using ADC input to control the motor, and I was told that ADC and UART has to be active in the BLDC tool...
```

---
## \#57 Posted by: Dredoggz Posted at: 2018-03-09T16:23:17.188Z Reads: 56

```
I need that apk file.
```

---
## \#58 Posted by: Juvaknin Posted at: 2018-04-21T06:06:26.599Z Reads: 45

```
Didnt find it on app store. How its called there?..
```

---
## \#59 Posted by: ivanflo Posted at: 2018-09-03T03:45:38.389Z Reads: 20

```
I too have been looking for this app on the iOS App Store, I guess this app was abandoned
```

---
