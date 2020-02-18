# DIY Trampa build / Trampa MTB / 12s1p (4 x 3s) / Dual 170kv / Dual FocBox /

### Replies: 41 Views: 823

## \#1 Posted by: Corevena Posted at: 2018-09-12T04:32:25.189Z Reads: 202

```
Hey all!

After a tone of research and study, I think I've got everything i need for a mtb build. 
A couple of things im concerned about is:
- Do i need higher than 80a for my bms? / Change the bms config from buildkits?
- Would the batteries be fine for over 20km? (Hilly inner city riding Melbourne)
- Do i need to change the vesc settings like in the tab for this setup?
If anyone has any recommendations for alt parts that would work better would be greatly appreciated :smiley:  

Build: (Excel doc)
https://docs.google.com/spreadsheets/d/1Cr9wY56VrvvGmJ0NvRqy2t7HWt7iCgy6BqOLUjkcQE8/edit?usp=sharing

Thank you all for your help so much info and especially @Namasaki 
(Started from not knowing much :stuck_out_tongue: )
```

---
## \#2 Posted by: telnoi Posted at: 2018-09-12T04:40:08.242Z Reads: 191

```
Go 6384 and save yourself some cash. 6380 fills a niche and is therefore expensive. 

You are wiring in series to get 12s, which means you still only have 5000mah which is not nearly enough for 20km.  You need at least double that/most likely even more. I needed 15Ah, but I am heavy and tend to ride full throttle allot.
```

---
## \#3 Posted by: Wraith Posted at: 2018-09-12T04:42:23.927Z Reads: 184

```
Aren't the 6380s by Torqueboards actually 6384 in stator size with a smaller can making it measure to 6380?
```

---
## \#4 Posted by: Corevena Posted at: 2018-09-12T04:44:11.036Z Reads: 178

```
Oh ok thanks :) So would something like this be better?
https://alienpowersystem.com/shop/brushless-motors/aps-6384s-sensored-outrunner-brushless-motor-130kv-4000w/
```

---
## \#5 Posted by: telnoi Posted at: 2018-09-12T04:44:20.657Z Reads: 166

```
Yes...but the price is different. They made a custom motor to fit their trucks, but with trampa you can even fit 8xxx motors. No need for an expensive custom motor size.
```

---
## \#6 Posted by: telnoi Posted at: 2018-09-12T04:45:25.943Z Reads: 160

```
Something like that. Your only determining factor might be how deep your pockets are and how long you are willing to wait. APS takes up to 4 weeks.
```

---
## \#7 Posted by: Corevena Posted at: 2018-09-12T04:47:32.423Z Reads: 156

```
Oh damn, im not really sure where to look for sensored motors if you have any thoughts? im in Australia for site reference.
```

---
## \#8 Posted by: telnoi Posted at: 2018-09-12T04:48:14.946Z Reads: 161

```
[quote="Corevena, post:1, topic:67780"]
Do i need to change the vesc settings like in the tab for this setup?
[/quote]

Every diy project with a vesc requires a complete setup from beginning till the end. Don't forget your remote failsafe either, it could save your life or that of others around you.
```

---
## \#9 Posted by: Andy87 Posted at: 2018-09-12T04:49:47.071Z Reads: 158

```
[quote="telnoi, post:6, topic:67780"]
APS takes up to 4 weeks.
[/quote]
😂😂😂
Only if the motors on stock...
Waiting already 10 weeks for my 6374 and 6384 motors from aps.
They wrote 6weeks if they on back order.
Hopefully they will ship today, than another two weeks for delivery and we made it to 3month and the end of the summer...
```

---
## \#10 Posted by: telnoi Posted at: 2018-09-12T04:50:36.421Z Reads: 150

```
Yeah, I'm going by what they told me via email. Looks like real life experience is even worse :laughing:
```

---
## \#11 Posted by: Wraith Posted at: 2018-09-12T04:51:25.423Z Reads: 144

```
yeah you're right didn't realize it was going to be a full Trampa deck and trucks. definitely go bigger then without the same constraints as the Tb218 trucks for motor sizes
```

---
## \#12 Posted by: telnoi Posted at: 2018-09-12T04:53:37.431Z Reads: 140

```
Dual 6374 is fine by the way. I haul 120kg Uphill off road at 35 km/h. The sk8 from hobbyking is most likely a good match. Personally running SK3 unsensored and it's holding up over 3000 km now.
```

---
## \#13 Posted by: Andy87 Posted at: 2018-09-12T04:54:01.184Z Reads: 129

```
If I understood right, this week they get the new batch of all motors which have been on backorder. So theoretically now is the best time to order 😅
Just hope they made this time a quality check...
Looks like with the last batch of 6384 motors they had some issues 😬
```

---
## \#14 Posted by: telnoi Posted at: 2018-09-12T04:55:05.354Z Reads: 128

```
Yah, I'm a bigger fan of the hobbyking motors despite of their smaller sizes.
```

---
## \#15 Posted by: Corevena Posted at: 2018-09-12T04:56:27.838Z Reads: 129

```
Is this something you configure in the VESC?
```

---
## \#16 Posted by: Andy87 Posted at: 2018-09-12T04:56:49.024Z Reads: 133

```
Keep in mind that the aps 63xx motors have a 10mm shaft, most other like sk3/8, torqueboard etc. usually only 8mm.
Important to know when you choose your pulley!
```

---
## \#17 Posted by: Andy87 Posted at: 2018-09-12T04:59:29.750Z Reads: 134

```
Already a bit sad that I didn’t order 4 sk3 motors... guess the 6374 is one of the most reliable motors on the market...unfortunately only unsensored
```

---
## \#18 Posted by: telnoi Posted at: 2018-09-12T04:59:59.271Z Reads: 138

```
No short answer. Simple failsafe is programmed with just the receiver and the remote. You press a button on the receiver and hold the throttle neutral or with a slight brake to save that value. It will then use that value when the remote looses the connection. 

Ackmaniac's vesc firmware also has software level failsafe stages that can be programmed via his vesc tool graphical user interface. Visit the dedicated thread for ackmaniac's firmware for more info on this, he describes the steps involved.
```

---
## \#19 Posted by: Corevena Posted at: 2018-09-12T05:03:40.127Z Reads: 139

```
I'll check it out thanks for the info!
```

---
## \#20 Posted by: Corevena Posted at: 2018-09-12T05:04:41.115Z Reads: 142

```
I was looking into the sk3 motors but sensorless sounds sketch with alot of stop start in the city?
```

---
## \#21 Posted by: Corevena Posted at: 2018-09-12T05:06:10.479Z Reads: 115

```
Sorry but do you mean go bigger than 6384 motors or battery?
```

---
## \#22 Posted by: Wraith Posted at: 2018-09-12T05:08:08.338Z Reads: 113

```
yeah bigger motors as the Trampa trucks are all considerably wider than standard longboard trucks. as for the battery yeah you can scale way up as well. probably better to top mount as this is an mtb build
```

---
## \#23 Posted by: telnoi Posted at: 2018-09-12T05:08:19.661Z Reads: 115

```
Sk8 is the sensored alternative. Supposedly it has almost the same internals as the SK3.

Would not go unsensored in the city.
```

---
## \#24 Posted by: Andy87 Posted at: 2018-09-12T05:11:25.138Z Reads: 114

```
You can always buy a sensor kit and install it by your own. 
Think even hobbyking has one listed.
```

---
## \#25 Posted by: Corevena Posted at: 2018-09-12T05:18:31.162Z Reads: 112

```
Im not too sure on adding a sensor to motors, any thoughts other than HK sk8's? for a mtb with 6.5" slicks
@Wraith @telnoi
```

---
## \#26 Posted by: Wraith Posted at: 2018-09-12T05:22:21.858Z Reads: 120

```
Don't think you'd really need to run sensor-ed as you won't be starting on an even surface mostly. APS is what I usually see on atb builds and my first build isn't full atb so I can't give a good recommendation on other motor options for that use. Ideally sealed and then go big to handle the heat is my 2 cents
```

---
## \#27 Posted by: Corevena Posted at: 2018-09-12T05:24:27.828Z Reads: 123

```
Thanks, i'll have a bit more of a look into sensorless mtb build and if i dont like it i guess i could put sensors on them.
```

---
## \#28 Posted by: Andy87 Posted at: 2018-09-12T05:24:41.421Z Reads: 131

```
https://www.unikboards.com/en/boutique/moteur-skateboard-electrique-6374/

https://eskating.eu/product/eskating-pro-motors-6374-190kv-waterproof-sealed-and-sensored/

For example and they both sealed, but EU so don’t know about shipping
```

---
## \#29 Posted by: Wraith Posted at: 2018-09-12T05:28:30.797Z Reads: 111

```
Unik parts are well made so they should serve you well. I recall seeing even a sub 170kv motor for massive torque to get you over steeper terrain
```

---
## \#30 Posted by: Andy87 Posted at: 2018-09-12T05:36:39.287Z Reads: 114

```
I think both similar just with different kV.
I have the eskating.eu motors and they work flawlessly till now. Manly I used them for flat roads. For off-road or hill climps I would go below 170kV to have a better torque
```

---
## \#31 Posted by: Corevena Posted at: 2018-09-12T05:39:13.771Z Reads: 113

```
Thanks, i have heard of Unik but never looked at their stuff that motor looks good. For 170 sensored is hard to find
```

---
## \#32 Posted by: Wraith Posted at: 2018-09-12T05:46:59.800Z Reads: 108

```
I think it would be good to factor in gearing as well. Not sure of the sweet spot for gearing and kv for atbs though but generally 170kv and below is the idea I think
```

---
## \#33 Posted by: Corevena Posted at: 2018-09-12T05:48:24.412Z Reads: 115

```
Yeah in that case the 150kv @Andy87 mentioned might work best
https://www.unikboards.com/en/boutique/moteur-skateboard-electrique-6374/
```

---
## \#34 Posted by: Andy87 Posted at: 2018-09-12T06:26:57.581Z Reads: 115

```
Definitely a good choice.
And @okp is here in the forum too and owner of unik boards ;)
That´s always good!

I just had some time to look through your part list.
Trampa board is nice, the motor mounts not really.
The end cap for the motor pulley will only fit if your motor shaft long enough. For mine it didn´t..
Get some motor mounts from unik boards or @Idea makes very nice ones too.
From both you can also get your pulleys too, and I think it´s even a bit more cheep.  (by the way, how you come to 400 dollar just for the motor mounts?)
Get a push to start switch from @Martinsp
http://electricskateboard.repair/index.php?id_product=44&controller=product
Will save you another 20-25 dollar
your focbox you can get from unik also...save you the shipping
about lipos we where speaking before. you will not get your 20km range with a 5ah battery, so you need to step up on this point.
in my opinion, if you have a BMS from Bestech, you don´t need a 130 dollar charger. There are a lot of good 12S chargers for about 50 dollars to find or from unik for 69 Euro.
get 10AWG instead of 12AWG. For a MTB with batteries in the middle it will reduce voltage spikes which could fry your focbox. The bigger the better. I use even 8AWG.
Don't forget to buy some JST adapters for your motor sensor wires.
The ones on the motor are 1,5mm on the focbox are 2mm.
and get some 5.5mm bullet connectors...focbox has only 3.5, your motor 5.5
```

---
## \#35 Posted by: Andy87 Posted at: 2018-09-12T06:58:35.412Z Reads: 100

```
aaand, get a Bluetooth modul...always good to track your rides. 
Will help you also to adjust the focbox settings later or find faults
```

---
## \#36 Posted by: ElectricCoast Posted at: 2018-09-12T09:07:55.535Z Reads: 96

```
That is correct.
```

---
## \#37 Posted by: mynamesmatt Posted at: 2018-09-12T12:40:35.433Z Reads: 92

```
hope so! i asked online and was told that they'd only be getting them in the last week of September :(
```

---
## \#38 Posted by: Andy87 Posted at: 2018-09-12T12:43:51.620Z Reads: 92

```
😬😬😬
Hope not so late... but we will see...
```

---
## \#39 Posted by: mynamesmatt Posted at: 2018-09-12T12:51:09.978Z Reads: 99

```
sick.... @hobbyking_ian 
![Screenshot_20180912-224708_Chrome|243x500](upload://3PlTc0HtfFCyoUxYoIgBaCCYBdL.jpg)
```

---
## \#40 Posted by: Corevena Posted at: 2018-09-13T06:21:41.644Z Reads: 91

```
Awesome info! just having some trouble finding the adapters you mentioned, Is this a thing i have to make or can but them from somewhere?
Also is this what you meant for a bt module? 
https://buildkitboards.com/products/vesc-bluetooth-adapter
```

---
## \#41 Posted by: Andy87 Posted at: 2018-09-13T07:08:48.623Z Reads: 89

```
for the sensor wires you need this adapter
https://eskating.eu/product/sensors-adapter-jst-2-0mm-6-pins/

or just cut the 1,5mm jst and solder a 2mm jst 6pin plug to the old wires. (if you do, don´t mix the black and the red wire ;) )

The Bluetooth module you linked would work.
but you also can get one for cheap, like this 
http://s.aliexpress.com/mIviqeUn
This works for IOS and Android, but it is a clone, so in case you run Oreo I think you need than to update the firmware on the module. If you have IOS you fine with it. Works on mine perfectly.

Another note on Bluetooth modules.
They work usually with all esk8 apps instead of the Metr app.
If you wanna use this app you need to purchase a special module.
```

---
