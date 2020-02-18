# What BMS will I need with two VESCs?

### Replies: 72 Views: 4067

## \#1 Posted by: Tomer Posted at: 2017-07-07T19:24:29.264Z Reads: 363

```
Hey,

I would like to build a battery pack for my E-Board. 
It will probably be a 10s2p, not sure about it yet. I am going to have x2 Maytech VESCs with a current of 50A each. What kind of BMS will I need, in terms of amps?
And do the dual motors that I am going to use will make a difference as well?

Thanks.
```

---
## \#2 Posted by: Namasaki Posted at: 2017-07-07T19:37:44.188Z Reads: 353

```
We don't know what motors you are using
Or what lithium cells you are gonna use for your battery
```

---
## \#3 Posted by: Tomer Posted at: 2017-07-07T19:43:30.694Z Reads: 351

```
You probably right lol. I am going to use Samsung 18650 30Q, the motors are Maytech 6355 200kv. 
 <img src="/uploads/db1493/original/3X/3/b/3bec5774018d0375d759f9abdad1ca6741548615.jpg" width="690" height="300">
```

---
## \#4 Posted by: Namasaki Posted at: 2017-07-07T20:01:14.714Z Reads: 336

```
200 KV is good for 10s and 30Q are said to be very good cells but I don't think your gonna be happy with a 10s2p. 
You would do much better with 10s4p
The 3510w max power is most likely a misprint 
Normally a 6355 190kv with 80a max will be rated around 2200-2400w
I have not seen 3000w from anything smaller than a 6374
I would suggest a motor that can handle 80a anyway.
```

---
## \#5 Posted by: Tomer Posted at: 2017-07-07T20:47:43.917Z Reads: 322

```
I'll contact Maytech and ask for more details about it. Will update here. 

So what do you think will be the BMS that I'll need to be using? More specific, the amp rate of it?

Thanks.
```

---
## \#6 Posted by: Namasaki Posted at: 2017-07-07T21:41:59.645Z Reads: 316

```
This one: it has a built in anti-spark on/off switch and is rated for discharge 80a continuous and up to 240a peak
Charge 20a
I run dual vescs set at 80a motor and 60a battery each and have no problem at all with this bms.

http://bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html
```

---
## \#7 Posted by: Tomer Posted at: 2017-07-08T00:19:46.790Z Reads: 301

```
Perfect! Much appreciated. 

Sorry for being noob, do I need to contact them in order to get price quote and ordering?
```

---
## \#8 Posted by: Namasaki Posted at: 2017-07-08T00:23:58.642Z Reads: 280

```
All their sales are through email
They accept PayPal
Somebody recently mentioned on another thread that they had an extra for sale.
http://www.electric-skateboard.builders/t/bestech-10s-bms-usa/22803
```

---
## \#9 Posted by: Tomer Posted at: 2017-07-08T00:36:18.024Z Reads: 270

```
Thanks for the reference, however I am not from the US so shipping from there might be more expensive then from the supplier itself.
```

---
## \#10 Posted by: Namasaki Posted at: 2017-07-08T00:41:36.417Z Reads: 266

```
Where you from
```

---
## \#11 Posted by: Tomer Posted at: 2017-07-08T00:41:57.618Z Reads: 266

```
I live in Israel.
```

---
## \#12 Posted by: Namasaki Posted at: 2017-07-08T01:28:18.820Z Reads: 254

```
Bestech has a distributor in Germany
```

---
## \#13 Posted by: Tomer Posted at: 2017-07-08T06:00:01.028Z Reads: 251

```
Cool, is there any way to contact them directly?
```

---
## \#14 Posted by: Namasaki Posted at: 2017-07-08T10:34:44.600Z Reads: 249

```
Email sales dept
```

---
## \#15 Posted by: Alan_Smithee Posted at: 2017-07-08T11:33:23.919Z Reads: 243

```
you could also not use a bms. just put balance leads on your packs and you can balance charge with any $30 hobby charger. You don't need balancing or management for discharging.
```

---
## \#16 Posted by: Achmed20 Posted at: 2017-07-08T18:14:53.337Z Reads: 233

```
why not use a cheapo BMS and use it for charging only?
```

---
## \#17 Posted by: Tomer Posted at: 2017-07-31T09:45:53.962Z Reads: 227

```
Those BMS includes e-switch with them so instead of buying an anti-spark switch for about 50$ I can buy a BMS + e-switch for 40$.
```

---
## \#18 Posted by: Tomer Posted at: 2017-08-08T05:45:29.077Z Reads: 232

```
If my motor is rated as 65A for max current, will it be okay to use the BMS you suggested? In the BMS specs I can see "10S-80A working current". Does it only related for the charging?

Another thing - I saw people here asked from the manufacture to ship their BMS with specific settings for cutoff start and cutoff end. I'm pretty noob when it comes to it so I'll be more then thankful if you can help me decide what settings should I ask from the manufacture to set mine.

Thanks!
```

---
## \#19 Posted by: Namasaki Posted at: 2017-08-08T05:54:33.198Z Reads: 235

```
The bms can handle 80a continuous discharge, up to 240a peak discharge and 20a charge.
I run dual drive. Each vesc is set to 80a motor max and 50a battery max.
That's 160a and 100a total and I have no problem with the vesc or the bms overheating.
And I've got everything inside an almost air tight enclosure. 
NOTE: I'm running Ollin 4.12 Vescs with heatsinks.


Here are the settings I use:
<img src="/uploads/db1493/original/3X/3/d/3d8f4b78ed8e860f4ae4e61ce6389a62fd94f0b7.png" width="392" height="500">
```

---
## \#20 Posted by: Tomer Posted at: 2017-08-08T06:10:59.435Z Reads: 222

```
Thank you for your swift reply, much appreciated.

My setup will include x2 [Maytech VESCs](https://www.aliexpress.com/item/Maytech-VESC-e-board-motor-kit-electric-mountain-board-controller/32754512890.html?ws_ab_test=searchweb0_0,searchweb201602_5_10152_10065_10151_10068_10172_10084_10083_10080_10307_10082_10081_10110_10137_10111_10060_10112_10113_10155_10114_10154_10056_10055_10054_10312_10313_10059_10314_10315_100031_10099_10078_10079_10103_10073_10102_10052_10053_10142_10107_10050_10051,searchweb201603_5,ppcSwitch_5&btsid=d30a0b31-46ab-4e34-97b8-7a8865c9d1d2&algo_expid=c4dbb984-52ed-44bf-a131-ab92da8f29c3-2&algo_pvid=c4dbb984-52ed-44bf-a131-ab92da8f29c3&transAbTest=ae803_2) and dual [Maytech 6355 200kv motors] (https://www.aliexpress.com/item/Maytech-electric-bike-3000w-6355-200KV-mountainboard-motor-with-hall-sensor/32718907347.html?ws_ab_test=searchweb0_0,searchweb201602_5_10152_10065_10151_10068_10172_10084_10083_10080_10307_10082_10081_10110_10137_10111_10060_10112_10113_10155_10114_10154_10056_10055_10054_10312_10313_10059_10314_10315_100031_10099_10078_10079_10103_10073_10102_10052_10053_10142_10107_10050_10051,searchweb201603_5,ppcSwitch_5&btsid=79225337-6e20-440e-876e-476de2863cd2&algo_expid=da355bd6-424d-4b54-a5dd-08d76dd4d6f2-5&algo_pvid=da355bd6-424d-4b54-a5dd-08d76dd4d6f2&transAbTest=ae803_2) (max current of 65A).
Will probably use 30Q Samsung batteries, 10S configuration.

Just to clarify - your settings are as follow:
**(1)  Over charge detection voltage: 42.8V±0.025V.**
**(2) Over charge release voltage: 4.08v±0.05V.**
**(3) Over discharge detection voltage: 3.00V±0.05V.**
**(4) Over discharge release voltage: 3.00V±0.1V**
**(5) Over current detection voltage: 0.1V~0.2V**

Considering all the parts I use for my setup, will you suggest me to apply your settings for my BMS?
```

---
## \#21 Posted by: Namasaki Posted at: 2017-08-08T06:25:52.146Z Reads: 201

```
You can go lower on the "Overdischarge detection voltage with Li-ions. On my Li-ion build, I had them set it at 2.8v
But if you set it at 3.0v then you could easily just ride till the bms shuts off.
I wouldn't worry too much about the Over current detection because the vesc controls battery current.
The default setting is 240a.  
If you get a short, the bms shuts off instantly.
I shorted my system at the charge port once and the bms shut off so fast (microseconds). that the short didn't effect anything except the charge port which was melted by the arc.
```

---
## \#22 Posted by: Tomer Posted at: 2017-08-08T07:34:38.678Z Reads: 198

```
Got you, so I should use all the settings as mentioned above and change **over discharge release voltage** to: **2.8V±0.1V**?
```

---
## \#23 Posted by: cryo Posted at: 2017-08-08T08:59:30.288Z Reads: 190

```
Hey @Namasaki could you explain this a bit more to me, I'm having trouble understanding. If the BMS continuous discharge is 80a, and you run your vesc at 80a motor and 50a battery,  how is the bms not overheating? wouldnt you be continuously drawing 160a which is two times more than the rating?

I just wanted to know for a build im planning based off of your LiPo 10s BMS builds ive seen.  If I were to get a 60a bms from supower and I have two vesc's, shouldn't I limit my vescs to not take more than 30A?
```

---
## \#24 Posted by: cryo Posted at: 2017-08-08T10:45:02.841Z Reads: 184

```
Also @tomer if you're planning to buy the bestech bms I would be down to purchase one with you. If I'm not mistaken those require a minimum order of 2.
```

---
## \#25 Posted by: Namasaki Posted at: 2017-08-08T12:26:32.246Z Reads: 177

```
[quote="Tomer, post:22, topic:27004, full:true"]
Got you, so I should use all the settings as mentioned above and change over discharge release voltage to: 2.8V±0.1V?
[/quote]

Yes if your wanting to get maximum range from your battery. 
If your wanting maximum life out of your battery, then you might just go with 3.0v
```

---
## \#26 Posted by: Tomer Posted at: 2017-08-09T06:51:20.649Z Reads: 167

```
Where are you located?
```

---
## \#27 Posted by: cryo Posted at: 2017-08-09T07:09:59.426Z Reads: 168

```
@Tomer i live in california.
```

---
## \#28 Posted by: Namasaki Posted at: 2017-08-09T07:10:25.061Z Reads: 175

```
[quote="cryo, post:23, topic:27004, full:true"]
Hey @Namasaki could you explain this a bit more to me, I'm having trouble understanding. If the BMS continuous discharge is 80a, and you run your vesc at 80a motor and 50a battery,  how is the bms not overheating? wouldnt you be continuously drawing 160a which is two times more than the rating?

I just wanted to know for a build im planning based off of your LiPo 10s BMS builds ive seen.  If I were to get a 60a bms from supower and I have two vesc's, shouldn't I limit my vescs to not take more than 30A?
[/quote]


Remember that the Bestech bms has overheat protection with a sensor on the FET heatsink.
The Battery max setting on the vesc is just that, The maximum current that the vesc will draw.
Setting the Vesc battery max at 50a doesn't mean your gonna be drawing 50a continuously.
Well maybe if your climbing a very long and very very steep hill at full throttle.
I have tested total amp draw using an inline watt meter riding up a 10% grade with 6s voltage and the total amp draw from both esc's was only 36a. thats only 18a per esc.
I have run my battery max at 60a X 2 vescs and still didn't overheat the vesc or bms.
And, though my vescs and bms both have heatsinks, they are both inside an almost air tight enclosure.


Advantages of the Bestech bms.
built in E-switch
heatsinks on top of FET's
adjustable over current detection up to 240a (meaning it can handle up to 240a)
adjustable over discharge voltage detection up to 3.0v
adjustable over charge voltage detection up to 4.8v
126ma balancing current ( twice as much as Battery Supports)
```

---
## \#29 Posted by: cryo Posted at: 2017-08-09T07:16:26.151Z Reads: 169

```
@Namasaki 
Ah I see. So theoretically if I set max current at 30A for each VESC I wouldn't have to worry about destroying anything, the board would just not be able to push me up the hill, correct?
I just want to have the most idiotproof failsafe system since it'll be my first build and I dont want to fry expensive parts even if it means not using equipment to full potential.
I live in a city with LOTS of VERY steep hills lol.

Edit: are you also bypassing your bms discharge? otherwise you would never get more than 40A on each since your bms is rated at 80A right
```

---
## \#30 Posted by: Tomer Posted at: 2017-08-09T07:21:03.690Z Reads: 156

```
Do I need an anti spark switch or can I just rely on the built in E-switch on the BMS?
```

---
## \#31 Posted by: Namasaki Posted at: 2017-08-09T07:21:13.844Z Reads: 158

```
I am not bypassing for discharge.
I have been running the bestech bms for over a year and have had no issues at all.
the bms has so many fail safes.
it it gets too hot, it shuts off
if you draw too much current (not likely) but if you do it shuts off
if you get a short anywhere in the system it shuts off.
if a battery cell drops to detection voltage it shuts off.

I am currently running my battery max at 50a and no worries.
Remember that you setting the max and the vesc and bms both can handle peaks up to 240a.
```

---
## \#32 Posted by: Namasaki Posted at: 2017-08-09T07:21:59.713Z Reads: 148

```
[quote="Tomer, post:30, topic:27004, full:true"]
Do I need an anti spark switch or can I just rely on the built in E-switch on the BMS?
[/quote]


the built in E-switch eliminates the need for an anti-spark switch or loop key.
```

---
## \#33 Posted by: cryo Posted at: 2017-08-09T07:23:04.176Z Reads: 141

```
ok nice i understand now.

thanks bro ur a fountain of knowledge :relaxed:
```

---
## \#34 Posted by: Namasaki Posted at: 2017-08-09T07:28:46.808Z Reads: 136

```
@cryo @Tomer
One thing you should know is that the Bestech bms has to be turned on while charging. So that means your whole system is on while charging unless you isolate the Vescs with a loop key.
I have been charging mine for over a year without isolating the vescs and it has not caused any issues for me on either of my 2 builds.
```

---
## \#35 Posted by: Tomer Posted at: 2017-08-09T16:56:03.842Z Reads: 139

```
Noted. Thanks for letting us know.
Is there any BMS that doesn't require to be turned ON in order to charge it?
```

---
## \#36 Posted by: Namasaki Posted at: 2017-08-09T17:28:05.566Z Reads: 142

```
Battery Supports because it's always on. With it you'll need an external E-switch or anti-spark loop key to turn the Vescs on
```

---
## \#37 Posted by: Fabar Posted at: 2017-11-04T20:23:16.248Z Reads: 141

```
thanks @Namasaki after reading a lot about it... I decided to get these BMS from bestech.....   maybe you have one spare to sell :) ....  I'm trying to find pictures or something how to connect it to my 5 packs of 2s li-ion batteries...   I'm going to use dual turnigy 6374 motors....
```

---
## \#38 Posted by: Namasaki Posted at: 2017-11-04T21:19:10.824Z Reads: 138

```
Sorry, I don't currently have any spare bms.
```

---
## \#39 Posted by: Tomer Posted at: 2017-12-26T14:00:26.388Z Reads: 133

```
Hey @Namasaki, I just finished to build a 10s4p battery pack with Samsung 30Q cells.
I'm now going to place an order for a BMS. I also bought an anti-spark switch.
I remember you said that if you get Bestech BMS with a built-in ON/OFF switch, you have to turn the board 
ON to get it charged.
When using anti-spark switch and Bestech BMS, do I still need to turn ON the board in order to charge it?
Does it also valid of SuPower BMS?

By the way, earlier in this post you showcased your BMS configurations that you use.
If I build another 10s pack but this time with Samsung 25R cells, do I need to change the configuration?
```

---
## \#40 Posted by: Namasaki Posted at: 2017-12-26T20:21:35.773Z Reads: 131

```
If you use the Bestech with built in e-switch, you have to turn it on to charge. 
If you use the Supower, You’ll need an external switch. 
NOTE: I have found the Bestech built in e-switch to be reliable but external e-switches are commonly unreliable. 
I have been charging both of my builds with them on for a year or longer and it hasn’t been a problem. 
The Vescs are on but just sitting idle.
```

---
## \#41 Posted by: Tomer Posted at: 2017-12-28T14:37:34.581Z Reads: 126

```
Thanks!

Using a BesTech without e-switch will still require me to turn ON the system in order to charge it?

I also contacted SuPower to see if I can buy a BMS from them with custom specifications, they can't do it.
Is it okay to use their BMS as is? 

(I'm asking because I'm still not sure if I'll buy BesTech or SuPower BMS)
```

---
## \#42 Posted by: Namasaki Posted at: 2017-12-28T18:14:33.559Z Reads: 128

```
[quote="Tomer, post:41, topic:27004"]
Using a BesTech without e-switch will still require me to turn ON the system in order to charge it?
[/quote]


I think only the one's with the built-in switch do that.
The switch also doubles as a reset button in case the bms goes into protection mode.
BMS's that don't have an on/off/reset switch require you to disconnect the battery and reconnect to reset them.
```

---
## \#43 Posted by: Namasaki Posted at: 2017-12-28T18:18:45.716Z Reads: 140

```
[quote="Tomer, post:41, topic:27004"]
I also contacted SuPower to see if I can buy a BMS from them with custom specifications, they can't do it.
Is it okay to use their BMS as is?
[/quote]


The problems with supower:
Low over current protection 
Low balance current
Minimum or no heat sinking
```

---
## \#44 Posted by: Namasaki Posted at: 2017-12-29T19:03:06.166Z Reads: 124

```
4 posts were split to a new topic: [Group Buy EU Bestech BMS](/t/group-buy-eu-bestech-bms/42222)
```

---
## \#45 Posted by: trigger4point7 Posted at: 2018-01-15T01:25:37.158Z Reads: 122

```
@Namasaki do you know if that BMS you [linked](http://bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html) still has a builtin anti spark? It doesn't mention that in the description.
```

---
## \#46 Posted by: Namasaki Posted at: 2018-01-15T03:44:34.368Z Reads: 127

```
![37 PM|333x210](upload://wvnpw0jRe5iYiVo5T3Y8yCaBjho.png)

The E-Switch is the anti spark switch
```

---
## \#47 Posted by: trigger4point7 Posted at: 2018-01-17T09:43:19.467Z Reads: 127

```
Oh ha, thank you for clarifying!!
```

---
## \#48 Posted by: Namasaki Posted at: 2018-01-17T12:56:44.520Z Reads: 130

```
It also serves as a reset switch for the bms when if it does a protection shut down
```

---
## \#49 Posted by: hornet90 Posted at: 2018-01-17T13:39:31.184Z Reads: 127

```
I also use a bestech bms having it on when it's charging is ok...it's a bit strange but it works ...
```

---
## \#50 Posted by: Namasaki Posted at: 2018-01-17T22:50:04.925Z Reads: 125

```
[quote="hornet90, post:49, topic:27004"]
I also use a bestech bms having it on when it’s charging is ok
[/quote]


It's not only ok, it is absolutely necessary.
```

---
## \#51 Posted by: Tomer Posted at: 2018-01-18T11:17:33.452Z Reads: 116

```


Hey @Namasaki, I'm about to [group buy](http://www.electric-skateboard.builders/t/eu-bestech-bms-group-buy-i-know-there-have-been-many-lately-lol/43963) with @koralle the [HCX-D131](http://www.bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D131.html) BMS (the one with no e-switch).
Would really appreciate if you could re-check these settings and let me know if they can be used for 30Q 
and 25R Samsung batteries.

[quote="Tomer, post:20, topic:27004, full:true"]

Just to clarify - your settings are as follow:
**(1)  Over charge detection voltage: 42.8V±0.025V.**
**(2) Over charge release voltage: 4.08v±0.05V.**
**(3) Over discharge detection voltage: 2.80V±0.05V.**
**(4) Over discharge release voltage: 3.00V±0.1V**
**(5) Over current detection voltage: 0.1V~0.2V**
[/quote]

Thanks!
```

---
## \#52 Posted by: Tobi Posted at: 2018-01-18T20:00:24.178Z Reads: 105

```
No its not ... my bms is charging the battery even when the switch is set to be off. same bms by 10s4p samsung 30q
```

---
## \#53 Posted by: Tomer Posted at: 2018-01-18T22:09:12.168Z Reads: 100

```
:scream::face_with_raised_eyebrow:
```

---
## \#54 Posted by: Namasaki Posted at: 2018-01-18T23:51:02.830Z Reads: 102

```
According to Bestech the switch needs to be on.
If you try to charge with the switch off, you might damage the bms or your charger.

![37 PM|357x500](upload://AtFScVyEtCIxwgU0NdafsPSHMsV.png)
```

---
## \#55 Posted by: Namasaki Posted at: 2018-01-19T00:00:52.574Z Reads: 100

```
[quote="Tomer, post:51, topic:27004"]
Just to clarify - your settings are as follow:

(1)  Over charge detection voltage: 42.8V±0.025V.

(2) Over charge release voltage: 4.08v±0.05V.

(3) Over discharge detection voltage: 2.80V±0.05V.

(4) Over discharge release voltage: 3.00V±0.1V

(5) Over current detection voltage: 0.1V~0.2V

Thanks!
[/quote]

I used these settings on for my 10s Li-ion battery.

![44 PM|354x500](upload://1PcN0q486xr6CvQ3IruoS59B8BP.png)
```

---
## \#56 Posted by: trigger4point7 Posted at: 2018-01-23T07:34:04.536Z Reads: 89

```
Does anyone have any tips for actually getting a hold of Bestech? Two emails so far to their sales department.
```

---
## \#57 Posted by: koralle Posted at: 2018-01-23T09:17:22.555Z Reads: 88

```
They are a bit weird. A week ago I had a 4-email-conversation with them within 20min. Now they are not answering me either. Maybe its a holiday over there or something...
```

---
## \#58 Posted by: trigger4point7 Posted at: 2018-01-23T15:08:45.748Z Reads: 86

```
You know, I looked up Supower on eBay because the shipping on their site was rediculous. I found their official eBay store and they had listed that they where on vacation. The English was a little off but it seemed like they would be out till the end of February! That definitely delays my build if supower and bestech are doing the same thing. I think Chinese New Year is on the 15th of February, so maybe it's that.
```

---
## \#59 Posted by: koralle Posted at: 2018-01-23T15:12:49.273Z Reads: 85

```
Since when do chinese factories have any holidays at all? What about all the foxconn scandals then? This would really screw up my nice BMS groupbuy :thinking:
```

---
## \#60 Posted by: longhairedboy Posted at: 2018-01-23T15:14:13.184Z Reads: 84

```
[quote="Namasaki, post:28, topic:27004"]
Setting the Vesc battery max at 50a doesn't mean your gonna be drawing 50a continuously.
Well maybe if your climbing a very long and very very steep hill at full throttle.
I have tested total amp draw using an inline watt meter riding up a 10% grade with 6s voltage and the total amp draw from both esc's was only 36a. thats only 18a per esc.
I have run my battery max at 60a X 2 vescs and still didn't overheat the vesc or bms.
[/quote]


all of this is truth. I run 60amp BMSs in all my boards and they never trip the BMS over current protections, even with ridiculous settings.
```

---
## \#61 Posted by: trigger4point7 Posted at: 2018-01-23T15:20:39.132Z Reads: 81

```
 Right there with you dude! Here is what I read. ![Screenshot_20180123-071905|281x500](upload://2injVsX8wgF54GTQv7RqOxZHYqD.png)
```

---
## \#62 Posted by: koralle Posted at: 2018-01-23T15:24:45.995Z Reads: 77

```
fml 10char
```

---
## \#63 Posted by: ron Posted at: 2018-03-12T11:31:01.444Z Reads: 75

```
So you are using a dual Setup with one BMS? Which BMS are you using and did you only connect the two VESCs in Parallel to the BMS power output?
```

---
## \#64 Posted by: longhairedboy Posted at: 2018-03-12T14:45:28.487Z Reads: 81

```
You only need one BMS per battery pack. You don't need a BMS for each VESC. 

The Battery Management System is designed to manage the battery. The only thing it has anything to do with the vesc is the power it is feeding it. You can not only power two ESCs off of the same BMS, which is part of the battery pack entity and not a seperate compartmentalized entity, but four. Or six. Or eight. 

there is no circumstance in which you would need more than one BMS in a battery pack. 

I have run 4WD builds capable of taking a 200 pound rider up to nearly 40mph while carrying an additional 30 pounds of gear in a pack. I did that on a 60 amp Battery Supports 12S BMS. I use those BMSs in all of my builds and will do so until i can finish properly evaluating these new open source ones i got from this forum.
```

---
## \#65 Posted by: ron Posted at: 2018-03-12T15:20:59.679Z Reads: 82

```
Thank you very much for your explanation. My thoughts were, that a 80A Continous Discharge BMS (Like the ones from BesTech) in a Dual Setup would be "on the edge" .

Thanks again for your help! :)
```

---
## \#66 Posted by: pjotr47 Posted at: 2018-05-09T14:41:50.366Z Reads: 66

```
[quote="Namasaki, post:19, topic:27004"]
Here are the settings I use:

HCX-D223V1 specs:Lipo.png599x764 157 KB
[/quote]
Are those the best bms settings I can use?
```

---
## \#67 Posted by: Namasaki Posted at: 2018-05-09T15:13:27.513Z Reads: 62

```
Can’t say if they are the “best”
They are just what I use.
```

---
## \#68 Posted by: pjotr47 Posted at: 2018-05-09T16:25:59.867Z Reads: 59

```
I think that i go order some BMS's with that specs. It is difficult to decide sometimes
```

---
## \#69 Posted by: Wraith Posted at: 2018-07-13T02:54:18.474Z Reads: 45

```
Hi! Newbie builder here and I’m curious as to your recommended bestech BMS for a 10s5p or 10s6p running the samsung 30Qs? I went throughthw thread and while I still don’t understand everything it definitely helped in planning out my first build. I’d prefer something that’s reliable and has the on/off switch. Is there a concern when using the bestech BMSs when the board is powered on while charging as I’ve read here as well?

Thanks to @longhairedboy for explaining the 1 BMS for a single pack part as well! I was unsure about that until I cane across this post.
```

---
## \#70 Posted by: Namasaki Posted at: 2018-07-13T06:41:24.288Z Reads: 41

```
I’ve never had a problem charging with the board on. 
I think that as long as the Vescs are not turning the motors, they are not really working. 
My Vescs are all 2-3 yrs old and still no issues.
```

---
## \#71 Posted by: Wraith Posted at: 2018-07-13T07:11:08.644Z Reads: 38

```
What vescs are you running?
```

---
## \#72 Posted by: Namasaki Posted at: 2018-07-13T11:32:15.482Z Reads: 38

```
Ollin 4.2 with heat sinks
```

---
