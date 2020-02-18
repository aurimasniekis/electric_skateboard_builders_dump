# Price friendly 10s bms

### Replies: 57 Views: 3644

## \#1 Posted by: Iam319 Posted at: 2017-05-01T02:10:19.753Z Reads: 425

```
looking for someone to either link me to a great price on a 10s BMS or to sell me two of them.
```

---
## \#2 Posted by: Smorto Posted at: 2017-05-01T02:13:22.145Z Reads: 415

```
http://www.batterysupports.com
```

---
## \#3 Posted by: Iam319 Posted at: 2017-05-01T02:19:08.415Z Reads: 412

```
So I have a 10s2p battery, along with a vesc. Would a 10s 45A bms be safe?
```

---
## \#4 Posted by: Namasaki Posted at: 2017-05-01T03:05:57.475Z Reads: 396

```
These are the best available and they are reasonably priced.
80a continuous discharge, 20a charge, built in E-switch saving you $40-$60 that you would spend on an external E-switch.
http://bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html
```

---
## \#5 Posted by: Iam319 Posted at: 2017-05-01T04:24:28.969Z Reads: 378

```
I don't see a price or a way to purchase?
```

---
## \#6 Posted by: Namasaki Posted at: 2017-05-01T04:42:31.290Z Reads: 356

```
send an email to lucy@bestechpower.com
copy this image to pdf file and attach it.
Tell here you would like to purchase this bms with these specifications.
Note: this bms comes with balance harness and a built in anti-spark E-switch.
Note: these specs are for Lipo application. For Li-ion application you can lower the over discharge detection to 2.8v or leave it at 3v
<img src="/uploads/db1493/original/3X/d/0/d01297cebb990b052debcf541833fb57342cbbba.png" width="355" height="499">

She will email you with an invoice that looks like this:
<img src="/uploads/db1493/original/3X/5/a/5a1ca66cfecfa350d1cc8046d8dc7ad10cb4775b.png" width="568" height="244">
This shipping charge is to USA.
Minimum order Qty is 2.
```

---
## \#7 Posted by: Iam319 Posted at: 2017-05-01T04:59:07.310Z Reads: 322

```
Thanks. I have a 10s 45A bms at the moment, would I be able to use it temporarily until I can get the money together for the new ones? Here's a link to what I'm running. https://www.electric-skateboard.builders/t/parts-and-wiring-setup/22054/4
```

---
## \#8 Posted by: Namasaki Posted at: 2017-05-01T05:04:27.717Z Reads: 323

```
You should be ok, Just set your vesc batter max amps to 45a or less if you are discharging through the bms.
```

---
## \#9 Posted by: Jinra Posted at: 2017-05-01T05:19:15.702Z Reads: 322

```
Mine burned out (my mistake) recently and I ordered the same one as a replacement. Can't be beat in terms of size IMO. I also do **not** discharge through it.

https://www.aliexpress.com/item/Free-Shipping-36V-10ah-battery-BMS-3-7V-18650-li-ion-cell-10S-BMS-PCB-PCM/32283661813.html?spm=2114.13010608.0.0.UBI4Jz
```

---
## \#10 Posted by: Iam319 Posted at: 2017-05-01T07:40:28.375Z Reads: 303

```
What do you mean by discharging through it? In the link I posted there's a diagram of my wiring plans. Will you tell me if I'm discharging through the bms and if so how to fix that?
```

---
## \#11 Posted by: Namasaki Posted at: 2017-05-01T12:31:25.066Z Reads: 285

```
BMS's are designed to manage and protect the battery during charge and discharge cycles. 
This is what is meant by charging through or discharging through the BMS. 
Some people have taken a BMS designed for low current applications and used them in high current applications such as an Eskate. 
To do this they will bypass the bms during the discharge cycle. Doing this will circumvent any protection from the bms during discharge and is a compromised setup.

Your diagram is not bypassing for discharge
```

---
## \#12 Posted by: makevoid Posted at: 2017-05-01T13:00:08.822Z Reads: 278

```
I can recommend [this BMS](http://www.batterysupports.com/36v-37v-42v-10s-60a-10x-36v-lithium-ion-lipolymer-battery-bms-p-267.html)

got three from:

http://www.ebay.co.uk/itm/152385098820?_trksid=p2060353.m1438.l2649&ssPageName=STRK%3AMEBIDX%3AIT

I'm using 2 of them from months and they seem to last / do their job
```

---
## \#13 Posted by: oyta Posted at: 2017-05-01T22:13:34.762Z Reads: 264

```
How should the parameters be set on the BMS @Namasaki mentioned: http://bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html

.. if using LG HG2 in a 10s3p config?

There are several adjustable parameters. If I get an answer from Besttech maybe they'll have a suggestion as well.

<img src="/uploads/db1493/original/3X/0/a/0a5e18cad1d029056a04d4e8a3ad08ef6d164e0b.png" width="690" height="227"> 
Screenshot from http://bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html.
```

---
## \#14 Posted by: Namasaki Posted at: 2017-05-01T23:15:36.360Z Reads: 247

```
I used these specs for Li-ion cells.

<img src="/uploads/db1493/original/3X/4/8/488d6bfb943955e4f77a91f39a17a86700bc806b.png" width="362" height="500">
```

---
## \#15 Posted by: landonkun Posted at: 2017-05-02T00:37:10.807Z Reads: 230

```
Interesting.. my spec sheet showed 0°C for the temperatures. Not that I'd be riding in the crazy cold :stuck_out_tongue:
```

---
## \#16 Posted by: Eboosted Posted at: 2017-05-02T00:55:16.488Z Reads: 219

```
The feature I like the most about the Bestech is the e-switch, you could save US$ 45 as you won't need to buy an antispark switch. 

However, what I also hate is that you need to have the switch on in order to charge the board which makes no sense at all.
```

---
## \#17 Posted by: Namasaki Posted at: 2017-05-02T01:35:32.438Z Reads: 225

```
[quote="Eboosted, post:16, topic:22113"]
However, what I also hate is that you need to have the switch on in order to charge the board which makes no sense at all.
[/quote]
Ya, I can't figure why they designed it that way but then I'm not an electronic engineer either. 
So I just live with it.
```

---
## \#18 Posted by: flywithgriff Posted at: 2017-05-02T03:42:13.622Z Reads: 215

```
Im looking for one as well if you want to split cost on a set.
```

---
## \#19 Posted by: Quent17 Posted at: 2017-05-03T21:31:48.497Z Reads: 203

```
@Namasaki will this BMS configuration work with 10s4p 18650?

If yes I'm also looking for one of these. I'm in Canada.
```

---
## \#20 Posted by: Namasaki Posted at: 2017-05-03T22:13:04.975Z Reads: 203

```
[quote="Quent17, post:19, topic:22113"]
will this BMS configuration work with 10s4p 18650?
[/quote]


Yes it will work with any 10s Lipo or Li-ion configuration.
```

---
## \#21 Posted by: JdogAwesome Posted at: 2017-05-04T00:23:52.236Z Reads: 187

```
Thought I drop in and say that the AliExpress BMS's arent terrible and there relatively cheap. Just make sure that they balance and have a decent charging current. https://www.aliexpress.com/wholesale?SearchText=10S+BMS&opensearch=true
```

---
## \#22 Posted by: Iam319 Posted at: 2017-05-04T05:13:24.797Z Reads: 184

```
I found a 10s bms cheaper on a more reputable website so I figured that was better in all aspects.
```

---
## \#23 Posted by: JdogAwesome Posted at: 2017-05-04T06:18:07.224Z Reads: 185

```
Yeah AliExpress can definitely be sketchy so if you found a better site, by all means purchase it off there. Do you happen to have a link to the BMS?
```

---
## \#24 Posted by: Iam319 Posted at: 2017-05-04T08:35:45.180Z Reads: 177

```
http://www.batterysupports.com/36v-37v-42v-10s-60a-10x-36v-lithium-ion-lipolymer-battery-bms-p-267.html 
$38 bucks before shipping for the 10s
```

---
## \#25 Posted by: Quent17 Posted at: 2017-05-04T14:15:40.108Z Reads: 167

```
Looks good but 74 $ shipping :confused:
```

---
## \#26 Posted by: JdogAwesome Posted at: 2017-05-04T15:53:57.685Z Reads: 162

```
Oh yeah I'm aware of the battery support BMS's but there quite expensive compared to the $15 free shipping ones on AliExpress.
```

---
## \#27 Posted by: WawiKirsinger Posted at: 2017-08-30T05:38:31.255Z Reads: 136

```
[quote="Namasaki, post:6, topic:22113"]
and a built in anti-spark E-switch.
[/quote]



so when you say that is built in..... i can solder a cheap switch from EBay... or i still need to buy a power switch like this https://miamielectricboards.com/shop-1/120amp-12s-power-switch ? i ask because i dont understand the e-wtich

thanks! :slight_smile:
```

---
## \#28 Posted by: willpark16 Posted at: 2017-08-30T05:41:40.386Z Reads: 127

```
U can use a cheap switch but I recvomend the led ones cause they look cool! But I also have the black ones for simplicity and use that one on my own board
```

---
## \#29 Posted by: overint Posted at: 2017-08-30T05:41:58.408Z Reads: 136

```
[quote="Iam319, post:24, topic:22113, full:true"]
http://www.batterysupports.com/36v-37v-42v-10s-60a-10x-36v-lithium-ion-lipolymer-battery-bms-p-267.html 
$38 bucks before shipping for the 10s
[/quote]

You can get them on ebay for a couple of bucks more and free shipping.
```

---
## \#30 Posted by: willpark16 Posted at: 2017-08-30T05:42:36.330Z Reads: 131

```
Those don't have eswitches and aren't exactly as good as the bestech ones when u compare price u will need an eswitch for those
```

---
## \#31 Posted by: Jinra Posted at: 2017-08-30T05:43:36.671Z Reads: 128

```
Where did you get the one you sold to Jay? recycled space cell bms?
```

---
## \#32 Posted by: WawiKirsinger Posted at: 2017-08-30T05:45:13.066Z Reads: 131

```
hey dude thanks fpr the quick answer.... how you do it for power the LED on the switch?.... and can you show or link the black one plz? 

thanks!
```

---
## \#33 Posted by: willpark16 Posted at: 2017-08-30T05:46:53.403Z Reads: 128

```
That's a spacecell bms bypassed per his request I had bestech ones but he asked for it to be exactly like a spacecell and that's about as close as u can get
```

---
## \#34 Posted by: willpark16 Posted at: 2017-08-30T05:47:33.392Z Reads: 125

```
Sure u just solder positive and negative for the black one, depending on the led switch it will vary
```

---
## \#35 Posted by: WawiKirsinger Posted at: 2017-08-30T05:50:39.006Z Reads: 126

```
Sorry for asking again but... what is the "black one" im noob and dont understand to much (also the english is a little dificukt with this word been more technical)
```

---
## \#36 Posted by: scepterr Posted at: 2017-08-30T05:54:55.621Z Reads: 127

```
I'm curious, why do you always have a typo in 1 word per post. It caught my eye and I can't let it go lol
```

---
## \#37 Posted by: willpark16 Posted at: 2017-08-30T05:56:05.660Z Reads: 124

```
HAHAHA my phone is crap my friend
```

---
## \#38 Posted by: willpark16 Posted at: 2017-08-30T05:56:33.082Z Reads: 123

```
Oh that's just the switch I have I can post photos if u want
```

---
## \#39 Posted by: scepterr Posted at: 2017-08-30T05:56:33.647Z Reads: 123

```
Not you @willpark16, I was referring to @WawiKirsinger
```

---
## \#40 Posted by: WawiKirsinger Posted at: 2017-08-30T06:05:33.180Z Reads: 124

```
What is a "typo"?
```

---
## \#41 Posted by: WawiKirsinger Posted at: 2017-08-30T06:06:04.480Z Reads: 120

```
Yeah! Plz post pic! 
Thanks!
```

---
## \#42 Posted by: scepterr Posted at: 2017-08-30T06:06:33.849Z Reads: 114

```
@WawiKirsinger incorrectly spelled word
```

---
## \#43 Posted by: WawiKirsinger Posted at: 2017-08-30T06:09:44.395Z Reads: 118

```
Jajajajajjaa ah ok i understand now xD is because my english is not very good i'm from chile (spanish language)
```

---
## \#44 Posted by: scepterr Posted at: 2017-08-30T06:11:19.136Z Reads: 118

```
Your English is fine,  you have clumsy fingers :stuck_out_tongue_closed_eyes:
```

---
## \#45 Posted by: WawiKirsinger Posted at: 2017-08-30T06:14:26.190Z Reads: 119

```
That too! LOL :joy:
```

---
## \#46 Posted by: willpark16 Posted at: 2017-08-30T06:14:39.735Z Reads: 125

```
<img src="/uploads/db1493/original/3X/1/0/10d9145db4974b13c23e5eb95e1bfcae5a69dc5e.jpg" width="375" height="500">
```

---
## \#47 Posted by: WawiKirsinger Posted at: 2017-08-30T06:18:46.260Z Reads: 124

```
Thanks dude i think i will do the same as you so its more stealth
```

---
## \#48 Posted by: willpark16 Posted at: 2017-08-30T06:25:20.294Z Reads: 122

```
I've got extra if u send me ur adress I'll send u one
```

---
## \#49 Posted by: WawiKirsinger Posted at: 2017-08-30T06:31:30.547Z Reads: 128

```
Im from chile so i think is not going to be very cheap :sweat_smile: Jajajajaja dont worry... thanks anyway but i found this <img src="/uploads/db1493/original/3X/f/d/fd9844c5fa375f557f21397c129b411181ed5cd5.jpg" width="412" height="500">

Very cheap and free shiping
```

---
## \#50 Posted by: willpark16 Posted at: 2017-08-30T06:34:55.613Z Reads: 124

```
Haha that works too
```

---
## \#51 Posted by: Namasaki Posted at: 2017-08-30T11:35:53.739Z Reads: 128

```
Any on/off switch will work to activate the electronic switch that is built into the bms. 
Just connect the 2 white wires coming from the bms 
If you use a light up switch you will have to supply voltage for the light from another source because the bms does  not supply 5v for the light.
If you use one of those light up switches, disregard the instruction that come with it. You will have to figure out with a multimeter how to connect the wires.
```

---
## \#52 Posted by: hornet90 Posted at: 2017-08-30T12:42:34.002Z Reads: 121

```
Brings tears to my eyes how nice people are on this site....
```

---
## \#53 Posted by: Namasaki Posted at: 2017-08-30T13:14:47.736Z Reads: 126

```
I would recommend this switch because they are more robust, they have a very convenient quick connector and they are only 16mm dia. So they're easirer to fit on the edge of your enclosure. 
And they come in a variety of colors. 

https://www.amazon.com/dp/B00YS25ZEM/ref=cm_sw_r_cp_apip_drVhzR6l6dYCe
```

---
## \#54 Posted by: leonsc Posted at: 2017-08-31T07:49:07.396Z Reads: 121

```
I like these cheap and well I think it's cool to start ur board with a key.<img src="/uploads/db1493/original/3X/a/d/ad5f407b6d0d092bddde06f31245d88be020aed4.jpg" width="400" height="400">
```

---
## \#55 Posted by: Tomer Posted at: 2017-08-31T12:12:24.473Z Reads: 106

```
lo. Just get a XT90 key.
```

---
## \#56 Posted by: drone001 Posted at: 2019-07-25T16:23:58.644Z Reads: 27

```
can you use this...does the 12V only mean anything. I'm looking for a replacement switch for my Unity.
```

---
## \#57 Posted by: Namasaki Posted at: 2019-07-28T01:54:05.926Z Reads: 19

```
I really can't advise on a replacement switch for the Unity. 
I'm not at all familiar with that unit.
```

---
