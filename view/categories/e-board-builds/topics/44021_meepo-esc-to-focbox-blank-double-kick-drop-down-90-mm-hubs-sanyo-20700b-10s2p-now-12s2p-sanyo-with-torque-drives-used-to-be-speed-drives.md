# Meepo esc to FOCBOX &#124; blank double kick drop down &#124; 90 mm hubs &#124; Sanyo 20700b 10s2p &#124; NOW 12s2p sanyo with torque drives (used to be speed drives)

### Replies: 71 Views: 5620

## \#1 Posted by: sayekim Posted at: 2018-01-18T14:26:03.780Z Reads: 554

```
I am going to replace the esc from the Meepo with FOCBOX. 

Can you please check if I am missing any parts to complete my build?
I think I got it right.

I live in the Netherlands so I have linked most parts to the eskating.eu online store.
Any suggestions to other stores are also welcomed.

This is my first build. Looking to go FOC (still have to read the other builds who have done this).

Parts list:

* Meepo Sanyo (pre V1):
https://meepoboard.com/
Will only use the hub motors (90mm x 55mm, 250 watts, 75kv I believe) with trucks, enclosures, front trucks with wheels, battery indicator, Sanyo battery (20700B 10s2p), battery cable (xt60)

* 2x FOCBOX (bought from [KOMODO](https://www.electric-skateboard.builders/u/KOMODO)):
https://eskating.eu/product/electric-skateboard-speed-controller-focbox-based-upon-the-vesc-2x/

* Nano X (bought from [KOMODO](https://www.electric-skateboard.builders/u/KOMODO)):
https://eskating.eu/product/nano-x-remote/

* waterproof cover for switch:
https://eskating.eu/product/waterproof-cover-for-on-off-bms-switch-20mm/

* gasket for enclosure:
https://eskating.eu/product/soft-black-gasket-for-enclosures-perimeters-1m-tailored/

* Bluetooth UART module for electric skateboards (IOs/Android Metr App Ackmaniac):
https://eskating.eu/product/bluetooth-uart-module-for-electric-skateboards-ios-android-metr-app-ackmaniac/

* can bus:
https://eskating.eu/product/can-bus-connector-for-electric-skateboard-speed-controllers/

* Anti spark power switch Made in Italy (40 to 100 amp fuses) will take the 40 amp fuse I guess?:
https://eskating.eu/product/anti-spark-power-switch/

* blank deck 42 inch drop down double kick with grip tape:
http://www.skateshred.com/index.php/wholesale-blank-longboard-decks/40-x-10-drop-through-blank-deck-205.html

* servo cable for connecting remote receiver:
eskating.eu doesn't sell this, what? 

After testing it I will probably try a 10s4p setup with the original Meepo stock battery (pre V1 10s2p)

For this all I will need is a new enclosure (don't know which yet) and the following part:

* 12 awg adapter:
https://eskating.eu/product/12-awg-parallel-adapters/
```

---
## \#2 Posted by: sayekim Posted at: 2018-02-20T15:07:14.452Z Reads: 463

```
I got it up and working but the bms is the limiting factor now.
The battery I am using right now is the sanyo 20700B (meepo sanyo 10s2P).

For the vesc batt settings on achmaniac vesc tool (firmware 3.1) is ok to set the batt max to 40 per vesc you think? Also wonder if I can go even higher than that.
```

---
## \#3 Posted by: rey8801 Posted at: 2018-02-28T11:20:33.518Z Reads: 447

```
Hi! since I am also going to use almost the same hubs, could you share how you connected the hubs with VESC/ focbox? With picture is probably easier:grin: Did you also connect the sensor cables? Thx a lot
```

---
## \#4 Posted by: sayekim Posted at: 2018-02-28T12:11:24.389Z Reads: 456

```
Yeah sure. I also use a can bus connection and blue tooth module. 

Unable to connect the sensor cable due to different size connector. I plan to buy the adapter plug from here:

products/vesc-sensor-wires

I believe they are the right ones. 

![image|374x500](upload://ga2d7brk11o8Y3AH9giFJOzMp4q.jpeg)
```

---
## \#5 Posted by: rey8801 Posted at: 2018-02-28T12:19:00.047Z Reads: 428

```
For the sensor cable you can also buy just the jst ph 6 pins female end and solder it instead of the 5 pins present. One pin is missing because the motor doesn't have the temperature sensor. Although I do not know the order of the cable on the Focbox and the motor. I know that yuo need to knoe just the ground (usually black) and the 5V (usually red) the other ones can be randomly placed. Otherwise you can also solder the cable directly on the focbox 6 pin male end.
Concering the bigger cables do you know what do they refer? I mean their role on the focbox becaue I have a different vesc. Thx a lot


Anyhow the sensor cable you wanna buy is not correct for this motor. if you want an adapter has to be a jst 1.5mm 5 pins for the motor side. But I would say that is better to replace directly the cable to jst ph 6 pins for the focbox.
```

---
## \#6 Posted by: sayekim Posted at: 2018-02-28T12:29:01.131Z Reads: 413

```
The 3 fase wires to motor?

No, someone told me it didn't matter. Just switch them around until it works.

As you can see I have the master which is the bottom one in my case in the order blue, yellow, green.
I had to to switch green and yellow on the slave to get the same direction. 

I don't think it was necessary though for I think you could also reverse the direction in the vesc tool which is what I am using with ackmaniac firmware 3.1.
```

---
## \#7 Posted by: rey8801 Posted at: 2018-02-28T12:30:45.346Z Reads: 395

```
Ah ok cool. I thought they have a order, but easier like that. Thx
```

---
## \#8 Posted by: sayekim Posted at: 2018-03-01T12:40:30.506Z Reads: 425

```
I read through all the posts and I was still confused a bit about the focbox installation. So here is my quick guide since I too was looking for one but could not find any and was very weary when I first tried it but managed anyway from the following links. Happy riding everyone.

https://www.electric-skateboard.builders/t/extended-ackmaniac-esc-tool-based-on-vesc-tool/35116

https://www.electric-skateboard.builders/t/new-version-2-1-ios-eskate-vesc-app-for-standard-and-ackmaniac-fw/32340

https://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286/13

https://www.electric-skateboard.builders/t/new-improved-focbox-official-thread/11102/335


What I did in the end for the ackmaniac tool and firmware was install the ackmaniac bldc tool first from the following link.

[ACKMANIAC-ESC Tool Link](https://www.dropbox.com/sh/t7dl90owz5ccbyl/AAANyC-yQCMeveA7errNRnYqa?dl=0)

upload firmware 2.54 in the tool from this link.

[VESC_Ackmaniac_Mod_2_54.bin](https://www.dropbox.com/sh/t7dl90owz5ccbyl/AAAXbKTS_VKlJMA3Gx_b0Zh9a/BLDC-TOOl%20and%20Firmware/VESC_Ackmaniac_Mod_2_54.bin?dl=0)

Since I am going dual I have the focbox's connected via the canbus.
The receiver for the remote is connected to the master focbox.
The Bluetooth UART module is also connected to the master focbox
The antispark is connected to both focbox's via the parallel, and then connected to the battery. 
Be aware that when you connect the power to only one focbox and the focbox is connected via canbus to the other focbox it wil/might blow up the non powered focbox. 

After this I connected the master focbox to the computer, started up the bldc ackmaniac tool which now has the firmware available of 2.54, and uploaded this firmware to the focbox.
Repeated the same for the slave focbox.

![image|690x198](upload://lVgb1kqarEYcv9s3kDSc40Iv8Ax.png)

Master focbox settings:
-App Configuration

I then went back to the master focbox and after I connected it to the bldc ackmaniac tool I made sure to id it as 0 for master, and since I am using the bluetooth module and nano x remote I also selected the PPM and UART option.
For slave you need to set controller ID to 1 and check Send status over CAN as well.

![image|690x351](upload://oohlT7YtIYttT3Hb4frQfuYl39h.png)

Then for the PPM page I went for Current no reverse with brake, and selected the Multiple ESCs over CAN option. For slave you do not set this option of Multiple ESCs over CAN option. Use the auto wizard for the remote calibration.

![image|690x478](upload://6o5q9DC1KRPa9iAZJCX47hqS2X.png)

For the bluetooth module connection you need to  enter the baud rate for value 115200 or 9600. It depends on which app you use. I don't know which was for which.

-Motor Configuration

I set the motor type to FOC, and played around with settings but I consider this safe so far. Haven't done any long range testing yet (It is too cold to enjoy it to the max). Use the same setting for the slave here.

![image|690x423](upload://cAtn9UGyfT3VWI1RY7ZDXbDMOCn.png)

On the FOC page go through the steps 1-5, repeat for the slave.

![image|525x500](upload://eeSSrhS0jgwlkE0QT2jRQin1qzs.png)

Hope this helps someone. I am currently running the vesc tool which is from ackmaniac which you can find from the same link at the top. This tool already includes the firmware 3.1 so once you have firmware 2.54 on your vesc's you can download this tool and upload the firmware to your vesc.

If anyone wants to see those settings let me know and I will add it. If anything isn't clear, message me and I will try to help.
```

---
## \#9 Posted by: Jumpman Posted at: 2018-03-01T13:09:20.616Z Reads: 315

```
Nice guide.  As you mentioned, you can upgrade to 3.1 firmware straight from the Esc Tool.  I don’t think you need to load the 2.54 firmware, unless I’m missing something?
```

---
## \#10 Posted by: sayekim Posted at: 2018-03-01T13:56:30.314Z Reads: 318

```
Thanks.

Yeah that may be true. I am not sure. This is what I did. If any one can confirm this for sure I'll edit it.

I read those posts many times over and it just wasn't clear to me. So I took what I thought was the safest to do since I also read so many posts about people with faulty/broken vescs.
```

---
## \#11 Posted by: rey8801 Posted at: 2018-03-01T14:22:39.944Z Reads: 297

```
Nice guide...I will ask yuo something for sure in the future qhen I will have to do the same! :grin:
```

---
## \#12 Posted by: stormboard1 Posted at: 2018-03-01T16:55:15.192Z Reads: 285

```
what would i do different for single focbox with nano x remote and planning use bluetooth module in the future but not now..iv got as far as uploading the 2.54 firmware to the focbox just now
```

---
## \#13 Posted by: sayekim Posted at: 2018-03-01T20:12:10.229Z Reads: 278

```
Do you wish to run it in foc?

You can keep it the same except for unchecking the box for multiple esc and traction control. Other than that you still have to figure out your current limits which depend on your motor and battery.
```

---
## \#14 Posted by: stormboard1 Posted at: 2018-03-01T21:15:56.329Z Reads: 264

```
ya hoping run foc on the focbox since its a sensored 6374 motor with 36/14 gearing and a 10s4p 30q battery and a nano x and bluetooth module soon
```

---
## \#15 Posted by: rey8801 Posted at: 2018-03-03T17:34:46.672Z Reads: 278

```
Hi! I would have some questions. I read all the thread but something is still not clear to me. I need to configure two VESCs 4.12 via Canbus. The VESCs have the ackmaniac's firmware and I will use the customize ESC tool he programed.  My questions are mainly about the initial steps:
1- Do I need to set up both vescs separately and only later connect them through the Canbus cable? Or can I already connect them together, then power on both of them and first connect the master to pc configure it (specificy ID0, send status over Can, multi esc over Can ecc...). Once the master + receiver is tuned, connect the slave VESC to pc ID1, send status over can and no multi esc over Can. Which one is correct?
2- Concerning the remote configuration, the receiver has to be connect to the master VESC, but how do I configure the remote on the slave VESC? Is it possible do it through the Canbus connection?
3- Do I need to reboot the VESC between the passages? 
4- Ackmaniac's firmware is based on watt instead of current. Where does it apply the max watt at the motor or VESC (battery) current? I mean usually we calculate the watt as 60A battery discharge x 10s x 3.7V = 2200W so 1100W for motor available. What current does the program take into account? The battery or the motor? Because the current at the motor level can be higher then the one provide by the VESC.

Sorry for the long questions :sweat_smile:
```

---
## \#16 Posted by: sayekim Posted at: 2018-03-03T18:03:37.207Z Reads: 264

```
The canbus is really only there for the vescs to communicate with each other to receive signal from remote and Bluetooth input. Maybe more but can’t think of it. 

1. Both ways work. Either way you will have to connect each vesc separately to the computer to configure them. 
2. You can connect the receiver to either vesc. The one that it is connected to is the one where you need to calibrate the remote. 
3. Don’t know. I connect the vesc then simply read settings first when I have them set up already, then make changes and write them. Then disconnect. 
4. It is max watt of the motor.
```

---
## \#17 Posted by: rey8801 Posted at: 2018-03-03T18:28:47.555Z Reads: 263

```
Thx for the fast reply. So
So I can power on both of the vesc and then just switch the usb cable to connect them to the pc, first the master then the slave. All passages briefly:
1- Connect both th vesc to the battery (can I use my own 10s battery right?) + motors.
2- usb cable to master vesc -->  ID0, send status over Can, multi esc over Can, motor max, battery max ecc... Select ppm + uart (if you have bluetooth) and configure the remote.
3- motor detection and adjust values.
4- Apply all the setting and move to the slave vesc.
5- Connect the canbus cable and connect the slave vesc to pc --> D1, send status over can and no multi esc over Can. Select PPM (do I need to select uart as well if I have bluetooth or only at the master side is needed?). At this point do I need to do the remote configuration or the master send the remote setting to the slave?
6- Motor detection and adjust values. Now both of the motors should spin. right?
7- Apply all the setting and enjoy!

Thanks for the help!
```

---
## \#18 Posted by: sayekim Posted at: 2018-03-04T12:01:25.218Z Reads: 266

```
You can configure the slave first or the master. It doesn’t matter. 

1. Yes connect the vescs to the battery with motors attached if you want configure the motors too. 
I do use an anti spark with power button for safety of the vescs. 

2. This is correct except for the send status over can which should only be enabled on the slave. 

3. Yes. 

4,5.  Yes do the slave and only check send status over can. Ppm uart checked on both to get data if using Bluetooth module. 
Remote calibration is done only on the vesc where the receiver is attached to. 

6. Yes. 

7. Happy riding
```

---
## \#19 Posted by: rey8801 Posted at: 2018-03-04T12:21:41.368Z Reads: 258

```
Perfect, I finally see the light a that e ed of the tunnel! Thx you very much! Now I need only need the motor :grin: ...
```

---
## \#20 Posted by: rey8801 Posted at: 2018-03-09T08:52:33.700Z Reads: 269

```
Hi! I thought it could interested you.

https://www.electric-skateboard.builders/t/eu-group-buy-cheap-hub-motor-set-90-mm-new-price-collecting-orders-4-10-taken/42647/166?u=rey8801

Ciao ciao
```

---
## \#21 Posted by: DeathByBacon Posted at: 2018-05-05T05:42:53.103Z Reads: 241

```
What do you call the connectors on the meepo's motors phase wires? Did you have to change them to connect to the focbox?

https://cdn.shopify.com/s/files/1/2096/3333/products/7_1800x1800.jpg?v=1520569102
```

---
## \#22 Posted by: rey8801 Posted at: 2018-05-05T05:45:13.283Z Reads: 218

```
Those are bullet connectors. No Focbox use the same size. I can't be sure but anyhow Focbox comes with 3.5mm connector. Check for your motor, but should be the same.
```

---
## \#23 Posted by: DeathByBacon Posted at: 2018-05-05T06:46:12.710Z Reads: 209

```
How different is the riding experience with using the focboxes instead of the old esc?
```

---
## \#24 Posted by: rey8801 Posted at: 2018-05-05T06:54:32.663Z Reads: 209

```
If with old esc you mean the one in meepo or other Chinese boards. I had a Koowheel before switch to Vesc. The difference is that you can program it. So speed, torque and brakes are better. You will feel immediately that acceleration and brakes are way smoother. It really does a lot.
```

---
## \#25 Posted by: sayekim Posted at: 2018-05-05T09:53:02.411Z Reads: 216

```
Yeah bullet connectors. They are 4mm on the motors and 3.5 on the focboxes. 

You will need to solder some new ones on to connect them or make an adapter from 3.5 male to 4mm female. 

Personally I would cut the bullets off of the focboxes and solder new ones on to fit whichever motor you are going to use. 
The soldering on them sucks. On one wire it broke already on mine.
```

---
## \#26 Posted by: sayekim Posted at: 2018-05-05T10:06:35.924Z Reads: 213

```
Way better. 

With the focboxes you set up your power needs as you please along the brake and throttle curve. 

Power is also instant if you like. I have it set so that I get full power from the get go up until the top speed. 

I recommend you do it and build your own battery too.
```

---
## \#27 Posted by: sayekim Posted at: 2018-07-02T00:15:42.272Z Reads: 208

```
I have just built a fresh 12s2p Sanyo 20700b battery for these meepo motors. 

No load speed from metr:
![image|281x499](upload://8il0u9otcmtSXPbL4nHudIJ11fU.jpg)

No load speed from eSk8matics:
![image|281x499](upload://vByYBpzboh44Y3KVVfveBc8HU9v.jpg)
```

---
## \#28 Posted by: onepunchboard Posted at: 2018-07-02T00:25:40.762Z Reads: 181

```
I'm more interested in amp consumption on load. but it gives u decent speed tho!
```

---
## \#29 Posted by: rey8801 Posted at: 2018-07-02T06:53:30.622Z Reads: 188

```
Nice! I was wondering about these motors with a 12s. I think some one eksw tried in the past but I am curious to know how they perform.
```

---
## \#30 Posted by: sayekim Posted at: 2018-07-02T16:50:06.424Z Reads: 192

```
Well I went for a short test ride and it is scary knowing that I am not fully recovered. Falling again on the same shoulder would not be good. 

Here are the metr data:

12s2p
https://metr.at/r/VqWxW

10s2p
https://metr.at/r/TgviX
```

---
## \#31 Posted by: Holyman92 Posted at: 2018-07-02T17:01:33.445Z Reads: 178

```
be safe man, we dont need to lose another rider, and nice conversion. It's funny how most people think you have to stick to stock hardware with pre-fabs... its like a sports car... u think the factory gives u ALL the bells and whistles lol.... u always gotta go after market for more fun
```

---
## \#32 Posted by: rey8801 Posted at: 2018-07-02T17:11:45.747Z Reads: 172

```
Nice. I will need to update to 12s I guess :grin:
```

---
## \#34 Posted by: sayekim Posted at: 2018-07-04T18:33:31.622Z Reads: 170

```
Hill climb was already pretty powerful with the 10s2p. Never actually measured the angle but I should have some footage of me going up a very steep part of a golf course. 

I’ll see if I can find it and upload it to my youtube channel.
```

---
## \#35 Posted by: rey8801 Posted at: 2018-07-04T18:57:45.320Z Reads: 171

```
Do you notice heavy voltage sag with 12s2p? ...from the metro data I see the voltage dropping of 5V during acceleration and high speed. Maybe a 3p would solve it.
```

---
## \#36 Posted by: sayekim Posted at: 2018-07-04T20:37:10.941Z Reads: 168

```
Yes I notice it in the data. Not sure if more p would solve it but I will find out when I finish building a 12s6p. It wouldn’t be a good direct comparison though for I will use 30q cells for it instead of 20700b cells.
```

---
## \#37 Posted by: rey8801 Posted at: 2018-07-04T20:54:50.423Z Reads: 169

```
The p should definitely help since it increases the discharge current available so you will be able to drain more current from the battery without sagging hard.
```

---
## \#38 Posted by: sayekim Posted at: 2018-07-06T18:57:40.459Z Reads: 175

```
Here is the uphill footage. 

https://youtu.be/TS92hZ-XYuU
```

---
## \#39 Posted by: sayekim Posted at: 2018-08-01T22:50:03.291Z Reads: 168

```
My current 12s2p battery I built. 

![image|500x500](upload://mMbJZ2JqlaikwZnF0v1sAMTNACN.jpeg)

![image|375x500](upload://lqhZ2RlyQF50hyzJffljwZQW6mI.jpeg)

![image|500x500](upload://bzy83gIU1yWwVkHvzWxyeVsA7k4.jpeg)

![image|500x500](upload://mKu20UvmOjj6pPLkqeKuOtjynPK.jpeg)

![image|500x500](upload://qxuTK98z8LgTV6P10RfsWxgzFe1.jpeg)
```

---
## \#40 Posted by: rey8801 Posted at: 2018-08-01T22:53:42.757Z Reads: 165

```
Nice Sanyo battery pack. I am using the same BMS. I had to remove the discharge connections to avoid braking failure when the battery is almost full charged.
```

---
## \#41 Posted by: sayekim Posted at: 2018-08-01T22:58:13.164Z Reads: 161

```
It is bypassed for discharged. Braking fail only happens when the battery maximum input voltage is reached.
```

---
## \#42 Posted by: sayekim Posted at: 2018-08-01T23:02:09.622Z Reads: 163

```
Carvon torque drives now. 
I love them but still only one ride day done. 

![image|375x500](upload://hRYa9WQAXN9eU3Pv0rgHhVaNFTT.jpeg)

![image|666x500](upload://ygze28pwuE8ALFoSZMO9WGZ7QmP.jpeg)
```

---
## \#43 Posted by: goldrabe Posted at: 2018-08-01T23:37:10.634Z Reads: 164

```
Nice upgrade!
How is the ride comfort compared to the Meepo hubs? What is your top speed with the torque drives and 12S? I've been also tempted by those, but 500$ for Koowheel hubs is a tad too steep for my wallet.
```

---
## \#44 Posted by: sayekim Posted at: 2018-08-01T23:41:46.666Z Reads: 162

```
A lot better but it is a little hard to compare since I’m riding them on 97mm vs the 90mm meepo. 

Need to ride more to give a better verdict. Top speed was 55kph. 

https://metr.at/r/tGCTi
```

---
## \#45 Posted by: sayekim Posted at: 2018-08-01T23:50:17.589Z Reads: 161

```
Initially I thought the same about modded koowheel hubs and the price which is why I went with the speed drives first but they are definitely worth it. 

It does make me wonder how the koowheel hubs would compare to torque drives on 12s with focboxes. 

If anyone would want hub motors that go fast, I’d try koowheel 96mm hub motors paired with focboxes and a 12s battery. My guess is they would be pretty sweet and the only advantage with torque drives then would be free choice of wheels within limits of course.
```

---
## \#46 Posted by: rey8801 Posted at: 2018-08-01T23:58:43.691Z Reads: 144

```
Yeh I read they have the problem with the heat dissipation and they get hot fast
```

---
## \#47 Posted by: goldrabe Posted at: 2018-08-02T00:05:30.980Z Reads: 152

```
How is the initial torque when accelerating and on hill climbs with the speed drives compared to the torque drives?
```

---
## \#48 Posted by: sayekim Posted at: 2018-08-02T00:12:26.193Z Reads: 149

```
I am having serious problems with the speed drives. Check my other posts in the carvon threads. 

Torque is not much with speed drives until you get going at speed but then they die of heat. 
Torque drives are heat safe and I still have to ride more to see if I can get them as torquey as the meepo hubs. The meepo hubs could throw me off. 
I’m riding the torque drives with a lot lower amps because of my bad experience with heat and speed drives. 

Settings now:
45
-45
25
-15

The torque drives can go up hill easily but I’ll for sure test more soon to give a better opinion since I have only ridden them for one eskate event day.
```

---
## \#49 Posted by: gmurad Posted at: 2018-08-02T00:20:47.502Z Reads: 143

```
Shouldn't your battery max be set to around 16 since you have a 2p setup and 2 VESCs and this Sanyo cell can only do Max Continuous of 16 Amps?
```

---
## \#50 Posted by: sayekim Posted at: 2018-08-02T00:23:22.097Z Reads: 143

```
Yeah but I don’t. The motors don’t pull 25 amps continuous which is why I set them higher.
```

---
## \#51 Posted by: rey8801 Posted at: 2018-08-02T03:14:49.658Z Reads: 149

```
I also have the Meepo hubs form diyeboard and indeed the torque is nice. Although I got used of the top speed so now I am going to try the 130Kv torqueboard hubs. I just got them 2 days ago and I am going to try them once I will back from holiday. I hope the torque is still ok with the 130Kv.I saw nice video and the speed should be plenty. If the 130Kv are too weak then I will try the 75Kv version and see if they have higher top speed of the Meepo ones. I am organizing a group buy so no problem in getting both of the version.
```

---
## \#52 Posted by: sayekim Posted at: 2018-08-02T06:53:44.792Z Reads: 140

```
If I’m right they won’t take off as well as the 75kv from my understanding of kv with hub motors and direct drive hubs. 
If you are going 12s you’ll be happy to use them with the diyeboard hubs.
```

---
## \#53 Posted by: rey8801 Posted at: 2018-08-02T11:34:31.450Z Reads: 139

```
Yeh I know but I do not have enough space for a 12s battery without making a new enclosure ecc.. I will try with a 10s and see it.
```

---
## \#54 Posted by: sayekim Posted at: 2018-08-02T22:12:02.006Z Reads: 144

```
https://metr.at/r/ALnnm

Went for a ride. Went uphill on the same slope as from my other youtube. They could not handle it from a full stop but from a bit speed they managed. 

Difference is that meepo hubs only have the weight of the motor plus the thin pu layer around it. Torque drives have this plus an entire wheel of weight to move. 
For this sole reason the hubmotors kill it in torque compared to these direct drives. 

I think the torque boards 65kv direct drives or perhaps 60kv will definitely compensate for this extra weight and then might be just as torquey as the meepo hubs. @torqueboards
```

---
## \#55 Posted by: rey8801 Posted at: 2018-08-02T23:24:06.287Z Reads: 125

```
Could you calculate the real Kv? With the ackmaniac app you can do it and my meepo hubs are actually 65Kv instead of 75Kv.
```

---
## \#56 Posted by: sayekim Posted at: 2018-08-25T14:37:53.320Z Reads: 127

```
Ackmaniac android app?

Or you mean his vesc tool for 3.102  firmware right?

I haven’t gotten round to this yet. I’m running vesc tool .94 now for 3.38 firmware. 

I will however try acks later though.
```

---
## \#57 Posted by: rey8801 Posted at: 2018-08-25T16:19:41.613Z Reads: 120

```
I think for the Kv you only need the app. Not need the actual firmware on the VESC. The app you can find it in the Google Play store. Although you have a metr connected. Is it not possible to check the motor Kv? Anyhow I asked to othera and indeed the hubs are actually a bit less than 75Kv, as in most of the motors.
```

---
## \#58 Posted by: sayekim Posted at: 2018-08-25T16:50:06.550Z Reads: 120

```
I don’t have an android device. I forgot to mention that. 

Yes I get that I don’t need the firmware, I just mentioned that to refer which vesc tool release.
```

---
## \#59 Posted by: rey8801 Posted at: 2018-08-25T16:51:06.849Z Reads: 116

```
No problem at all. Thank you for the help
```

---
## \#60 Posted by: gmurad Posted at: 2018-08-28T11:34:53.940Z Reads: 125

```
I just finished a DIY build using 10s2p Sanyo 20700b and I set my battery max to 20Amps for each of the 2 x Focbox. I'm experiencing some heavy voltage drops when accelerating and drawing 40amps from the pack (https://metr.at/r/DOZ6l)

I see the a similar behavior on your graphs as well, you seem to have set 25A for each Focbox. I'm considering lowering it to 16 Amps but wanted to ask you how is your aggressive setting going after a month.

Thanks.
```

---
## \#61 Posted by: sayekim Posted at: 2018-08-28T12:55:17.763Z Reads: 132

```
Nice 12s even better but if I would do it again I would go at least 3p due to sag. 

The sag seems to be pretty normal for 2p setups. 
I have been riding them very hard and they are fairing well. 
Time will tell though. 
Latest ride a lot more confident to ride faster and range is decreasing a lot due to this. 

Normal riding 25km range:
https://metr.at/r/Evreb

Agressive fast riding 17km range:
https://metr.at/r/x2ron
```

---
## \#62 Posted by: gmurad Posted at: 2018-08-28T16:08:12.327Z Reads: 118

```
Nice, I did my first commute today on the new DIY, I lowered the max amps on each vesc to 16A to try and this was the full ride:

https://metr.at/r/dZQWa

Still getting some heavy voltage sag but looks like I will get 20+ kms which at my 225lbs weight I think is positive.

Do you see anything concerning in my data?
```

---
## \#63 Posted by: sayekim Posted at: 2018-08-28T18:49:23.629Z Reads: 104

```
What is your setup? Motors, motor settings, esc?
```

---
## \#64 Posted by: gmurad Posted at: 2018-08-28T20:07:58.985Z Reads: 106

```
Dual 6354, Focboxes, 10s2p Sanyo 20700b. This ride had the following settings:

Batt Max 16A
Batt Min -12A
Motor Max 80A
Motor Min -35A


Cutoff starts at 31V ends at 28V.

Before I tried 20A batt max instead of 16A and it was very nice but a bit worried about pulling 40A from this battery.
```

---
## \#65 Posted by: sayekim Posted at: 2018-08-28T21:58:39.658Z Reads: 105

```
Yeah if it worries you don’t do it. I’m doing it for science pulling 50amps. The thing is those ratings are continuous ratings. 
The sanyo 20700b cell is rated for 15amp continuous current. 
I only pull 50 when taking off and that lasts a second or so. When riding 50kph, depending on wind conditions I only pull 10amps per focbox. 

Since I have the metr pro the batt and motor values are added up for dual.
```

---
## \#66 Posted by: gmurad Posted at: 2018-08-29T00:09:38.224Z Reads: 104

```
What I noticed from my ride logs is that whenever I touch the throttle it draws max amp, it's either 0 or full amps.

I was able to make my way back home form work just now and the battery was still at 35V! Almost 22km. Not bad considering I'm 225lbs. The sag wasn't so bad I was able to go up the long hill at end of my commute still going at 20~25km/h.
```

---
## \#67 Posted by: goldrabe Posted at: 2018-08-29T00:16:17.059Z Reads: 103

```
Which BMS are you using? Is that the pack offered by several chinese vendors?
```

---
## \#68 Posted by: gmurad Posted at: 2018-08-29T02:13:02.190Z Reads: 102

```
Yes, got the meepo 10s2p Sanyo 20700b pack when it was on sale recently.

build thread: https://www.electric-skateboard.builders/t/murad-i-vanguard-42-flex-2-caliber-ii-50-10-dual-6355-190kv-marcmt88-mounts-10s2p-sanyo-20700b-2-x-focbox-90mm-abec-11/62355/18
```

---
## \#69 Posted by: Skyart15 Posted at: 2019-05-08T03:53:03.259Z Reads: 46

```
Does anyone know if meepo hubs will run sensorless?
```

---
## \#70 Posted by: ryansinatra Posted at: 2019-05-08T03:59:56.215Z Reads: 45

```
Yes, meepo hubs will run sensorless
```

---
## \#71 Posted by: Skyart15 Posted at: 2019-05-08T04:00:23.497Z Reads: 46

```
Oh sweet! Thanks!
```

---
## \#72 Posted by: City-Blade-101 Posted at: 2019-05-08T20:54:43.912Z Reads: 40

```
Nice with that lunchbox underneath, so you have always veggies and peeled off fruits at hand:joy::joy::joy::joy:
just kidding
```

---
