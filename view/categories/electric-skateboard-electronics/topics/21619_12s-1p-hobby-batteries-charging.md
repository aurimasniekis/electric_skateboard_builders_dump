# 12s 1p hobby batteries charging?

### Replies: 36 Views: 2483

## \#1 Posted by: SyrusB Posted at: 2017-04-23T15:40:38.126Z Reads: 155

```
<img src="/uploads/db1493/original/3X/0/a/0a7df01ac6cef9b7a00bbb58b057524ae2333ba9.PNG" width="666" height="500">
Ok so I am wanting to upgrade and add another 4s 5000mah but, this time I want to make it where I can just plug and go instead of taking the batteries out of the case is there any easier way to do this. I was thinking of a bms but I am not sure which one to get and how to set it up.
```

---
## \#2 Posted by: Smorto Posted at: 2017-04-24T01:18:13.235Z Reads: 128

```
Do you have to take your batteries out in your current setup? It looks to me that you could just add another battery in the same way you have now any you will be good to go. Just as a thought your charging setup looks almost exactly the same as mine lol which is cool.
```

---
## \#3 Posted by: ieatflys Posted at: 2017-04-24T01:48:34.050Z Reads: 127

```
from what im seeing your wanting to leave it all plugged in and charge all of the batteries individually like you would with one charger one at a time??  if this is true it would be a bad idea because while you charge one the voltage will leak into the other batteries unless you unplug them... my suggestion is go on ebay and google 12s lipo bms and purchase one from china   i just ordered mine and it will be here in a week or two (im in the middle of an overhaul) then to charge you just plug a power supply with the correct voltage into the bms and it will do the rest for you...

a mean well bms made for 48 volts will have a pot on it you can turn it up to 50.4 and safely se it to charge with. this is what i am doing currently however it will be my first attempt with a bms so fingers crossed.
```

---
## \#4 Posted by: Namasaki Posted at: 2017-04-24T03:06:40.678Z Reads: 113

```
[quote="SyrusB, post:1, topic:21619"]
Ok so I am wanting to upgrade and add another 4s 5000mah
[/quote]

Adding a 12s bms would be the best way to charge all your batteries together.
However, it is possible to charge them separately using a hobby charger without disconnecting them.
But you would still have to charge them one at a time.
@ieatflys Voltage will leak across a parallel connection but not a series connection.
You can't isolate cells in a parallel connection but you can in a series connection.

I can't tell for sure if your wiring is correct because it is unclear with all the yellow blocks.
If you could edit your diagram and remove the connectors so we can see exactly how you are connecting the wires.
Also you would do better to omit so many connectors and hard wire the main battery wires like I did in my build with 5 Lipos in series.
I am using a bms but you could just tap into the main wires for isolated charging.
<img src="/uploads/db1493/original/3X/f/6/f616750027452cdbcef6fabd852909a41c985f47.png" width="649" height="500">
```

---
## \#5 Posted by: Hummie Posted at: 2017-04-24T03:36:36.810Z Reads: 103

```
We're on a very similar topic one thread below.  Here's an option:

https://www.amazon.com/GENSSI-Regulated-Switching-Power-Supply/dp/B005CLBZRO

https://hobbyking.com/en_us/turnigy-dlux-lipo-battery-cell-display-and-balancer-2s-6s.html?___store=en_us
```

---
## \#6 Posted by: SyrusB Posted at: 2017-04-24T10:19:18.343Z Reads: 93

```
Yes I do have to take my batteries out of my current setup.
```

---
## \#7 Posted by: SyrusB Posted at: 2017-04-24T10:21:43.170Z Reads: 93

```
Is there any digrams that I could use to show me how to setup a BMS because I would like to do this to my second build also if this is true also how do u check the voltage. I am fairly new to this and @cmatson help with my first build.
```

---
## \#8 Posted by: lowGuido Posted at: 2017-04-24T11:43:42.885Z Reads: 85

```
https://www.electric-skateboard.builders/t/skate-a-tron-4000-superleggera-carbon-deck-12s-dual-hub-motor-vesc/1531/58
Have a look at my diagram here. I use two B6 chargers to charge 12S
```

---
## \#9 Posted by: Smorto Posted at: 2017-04-24T12:50:02.841Z Reads: 77

```
Why? Do you have pictures of your setup? I have pretty much the same wiring diagram and I don't have to take my batteries out... I am a bit confused :slight_smile:.
```

---
## \#10 Posted by: SyrusB Posted at: 2017-04-24T14:18:56.147Z Reads: 72

```
I Am actually at school right now but basically it is two 4s batteries then I have a plug to connect them in series then they connect to the vesc.
```

---
## \#11 Posted by: SyrusB Posted at: 2017-04-24T14:26:44.572Z Reads: 72

```
Do u balance charge your batteries by plugging in the balance Cords any where.
```

---
## \#12 Posted by: SyrusB Posted at: 2017-04-24T15:18:36.448Z Reads: 74

```
Ok so this battery has a voltage of 14.8 that time 3 one for each battery so it is 44.4 volts. So basically it will look like this <img src="/uploads/db1493/original/3X/8/9/8992826a15701c9dc5541c376dbf1b0e3634b6c5.PNG" width="375" height="500">
Then where do I have the charge port and the plug to go to the vesc and then the power switch.
```

---
## \#13 Posted by: Namasaki Posted at: 2017-04-24T15:30:56.595Z Reads: 70

```
<img src="/uploads/db1493/original/3X/e/3/e3cd1238e5c7f8e6caac64ba45f30b48ac97cfee.JPG" width="375" height="500">

<img src="/uploads/db1493/original/3X/c/0/c0e903853f08234f1aa1223c308c11d1d189be44.PNG" width="664" height="500">
```

---
## \#14 Posted by: SyrusB Posted at: 2017-04-24T16:08:26.889Z Reads: 63

```
Sweet that is very helpful.
```

---
## \#15 Posted by: jmasta Posted at: 2017-04-24T18:34:52.658Z Reads: 66

```
[quote="SyrusB, post:12, topic:21619, full:true"]
So basically it will look like this<img src="/uploads/db1493/original/3X/8/9/8992826a15701c9dc5541c376dbf1b0e3634b6c5.PNG" width="375" height="500">

[/quote]

Your wiring schematic is incorrect

Positive line never goes into this BMS. It only switches the negative line 

P- to ESC/Charge negative
B- to Battery negative 
N- is not used
```

---
## \#16 Posted by: SyrusB Posted at: 2017-04-24T18:46:35.390Z Reads: 60

```
Ok so more like this but I am still missing the charge port and power switch.
<img src="/uploads/db1493/original/3X/b/a/ba50098d4b5405d763023809ac0c9a0185e90f20.PNG" width="375" height="500">
```

---
## \#17 Posted by: mmaner Posted at: 2017-04-24T21:34:03.134Z Reads: 52

```
That BMS doesn't come with a power switch.  You will need to use an XT90-S or a VEdder switch.  You should have a port on the BMS labeled C-, that is the negative for the charge port, the positive for the charge port should be spliced into the battery pack positive.
```

---
## \#18 Posted by: SyrusB Posted at: 2017-04-24T21:35:10.115Z Reads: 53

```
What company do u usually buy your bms from or recomend.
```

---
## \#19 Posted by: mmaner Posted at: 2017-04-24T21:36:05.538Z Reads: 54

```
I've SuPower and BesTech, I prefer the BesTech but both are OK.
```

---
## \#20 Posted by: SyrusB Posted at: 2017-04-24T21:36:58.561Z Reads: 53

```
Ok I will go check them out now.
```

---
## \#21 Posted by: SyrusB Posted at: 2017-04-24T21:44:26.645Z Reads: 53

```
If I were to buy this one could I also splice into the negative like the positive.http://www.ebay.com/itm/44V-48V-50-4V-12S-60A-Lithium-ion-Li-ion-LiPo-Li-Polymer-Battery-BMS-PCB-System-/221644780045?hash=item339b0ef20d:g:aXsAAOxy06hSEdYj
```

---
## \#22 Posted by: mmaner Posted at: 2017-04-24T22:03:20.457Z Reads: 48

```
look here...
http://www.batterysupports.com/44v-48v-504v-12s-60a-12x-36v-lithium-ion-lipolymer-battery-bms-p-270.html

The image as shown on the website above explains how its connected.
B- goes to the battery pack NEG
P- goes to the VESC/ESC and the charge port NEG
<img src="/uploads/db1493/original/3X/4/1/415bee31d47ad671bd4cd6c411dc158e66c8fe58.jpg" width="690" height="384">
```

---
## \#23 Posted by: SyrusB Posted at: 2017-04-24T23:57:20.130Z Reads: 45

```
After a lot of reading and all of advice from everyone that helped me I think that I figured it out (probably wrong)
<img src="/uploads/db1493/original/3X/f/4/f4c388aa6bf15b633a58f9f5b292da4d34d010e0.PNG" width="375" height="500">
And know all I have to do is get a charger that is compatible 12s 44.4v
```

---
## \#24 Posted by: jmasta Posted at: 2017-04-25T00:04:44.765Z Reads: 44

```
Looking good. I'd recommend wiring the charge port before the XT90s loop key, so that the ESC is off while charging 

I have an extra 12S 2A charger I can sell you if you are interested. PM me
```

---
## \#25 Posted by: Smorto Posted at: 2017-04-25T00:04:59.946Z Reads: 42

```
If you do end up competing this please please take some pictures of your setup so I can basically copy it! :slight_smile:. This thread has helped me understand BMS's quite a bit as well. Just out of curiosity, is this setup by passing the BMS for discharging and using it for charging only or not? I am still confused on that lol.
```

---
## \#26 Posted by: SyrusB Posted at: 2017-04-25T00:06:48.238Z Reads: 42

```
Truly I am just as confused as you i don't know but I bet someone on here will knwk and yes I will post this.
```

---
## \#27 Posted by: Smorto Posted at: 2017-04-25T00:07:18.348Z Reads: 42

```
Awesome! Looking forward to it and good luck!
```

---
## \#28 Posted by: SyrusB Posted at: 2017-04-25T00:08:20.022Z Reads: 43

```
Yea I am interested but doesn't it matter the voltage output I have 3x 14.8v so 44.4v.
```

---
## \#29 Posted by: SyrusB Posted at: 2017-04-25T00:09:02.036Z Reads: 43

```
Thanks I will also be doing this on my second board with a 8s battery.
```

---
## \#30 Posted by: SyrusB Posted at: 2017-04-25T00:10:24.842Z Reads: 43

```
<img src="/uploads/db1493/original/3X/2/e/2e3c64ef528f2bebb6bc87f297469bccb5f1ae16.PNG" width="375" height="500">
Like this.
```

---
## \#31 Posted by: SyrusB Posted at: 2017-04-25T00:20:04.849Z Reads: 39

```
How many amps do I need to have on my bms for example I will doing a 2x 4s 5000mah would 45a work or do I need 60a.
```

---
## \#32 Posted by: SyrusB Posted at: 2017-04-25T00:27:23.337Z Reads: 40

```
Never mind
```

---
## \#33 Posted by: jmasta Posted at: 2017-04-25T00:40:22.193Z Reads: 41

```
44.4V (3.7V x 12) is nominal voltage. For 12S you need a 50.4V charger (4.2V x 12) 

I am using this same exact BMS and have an extra 50.4V 2A charger
```

---
## \#34 Posted by: SyrusB Posted at: 2017-04-25T01:13:29.558Z Reads: 40

```
yeah how much?
```

---
## \#35 Posted by: SyrusB Posted at: 2017-04-25T01:21:08.877Z Reads: 39

```
what voltage meter did u use also what plug is it for the charger.
```

---
## \#36 Posted by: SyrusB Posted at: 2017-04-25T10:48:36.691Z Reads: 38

```
Also you know that I have a battery with 44.4 as in hobby grade batteries not lion just making sure you new that.
```

---
