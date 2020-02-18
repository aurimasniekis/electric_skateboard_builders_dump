# First build - Mono 6374, VESC, 10S3P, BMS, 90mm Flywheel

### Replies: 26 Views: 2702

## \#1 Posted by: Luuke Posted at: 2017-11-03T19:03:23.168Z Reads: 351

```
Hi everyone,

I am planing to build my fiste ESK8. This will be my setup:

Maytech 6374 170KV sealed and Hall sensors
http://www.maytech.cn/en/mto6374-170-ha/10339.html

VESC 4.10
https://hobbyking.com/de_de/turnigy-sk8-esc-for-electric-skateboard-conversion.html

12S3P DIY INR18650 25R Samsung
What will be the expected range? May i switch to 12S4P

12S BMS Bestech with antispark switch
Maximal continuous discharging current 80A
http://www.bestechpower.com/444v12spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html

maytech Remote with cruise control
http://www.maytech.cn/en/mtskr1512-2-4ghz-hand-remote-controller/10774.html

Meanwell Powersupply 48V 3A
Boost it to 50V

Drivetrain 15T 36T 285mm 15mm
https://hobbyking.com/de_de/gear-set-with-belt.html

Motor Mount Cover
https://hobbyking.com/de_de/motor-mount-cover-with-bearing.html

Motor Mount
https://hobbyking.com/de_de/motor-mount-5.html?wrh_pdp=7

MT60 for motor phase contacts

3mm PVC Thermoplast for enclosure

I will reuse some Longboard-stuff I allready own:
ABEC 11 Flywheel 90mm
Bear Polar 180mm trucks with spacer  OR gullwing sidewinder
One of my decks
Ceramic bearings


I hope that sounds like a good setup?!
I am unsure about the capacity at the moment...
Do you have some further hints for me, which I have to take care?
```

---
## \#2 Posted by: Lawndart Posted at: 2017-11-03T19:45:39.678Z Reads: 296

```
I'd get a better motor mount. I don't trust the universal fit style of mount. There are alot of people on here that make mounts. Hit them up and get a decent mount. You should think about a 10s4p to use with your vesc or upgrade to a focbox.
```

---
## \#3 Posted by: Luuke Posted at: 2017-11-03T19:55:42.191Z Reads: 289

```
I wanna give that motor mount a try. Can change to some other or DIY later.
WHY shoukd I change to 10S? And why 4P instead of 3P?
Why would upgrade to focbox make a difference? Ok, they use diffrent FETs, but still very close layout to VESC 4.xx, right? So they also use 2 Shunts for current measure? VESC 6 uses 3 shunts.
Do they measure lowside or inline the phases?
```

---
## \#4 Posted by: Crossfire Posted at: 2017-11-03T20:01:27.754Z Reads: 271

```
More batts in parallel, less voltage sag. Go for 30Q instead of 25R. 
10S4P with VESC and 190kV motor with 15/36 drive on Caliber II's is a gold standard (proven setup) in esk8 atm.
```

---
## \#5 Posted by: Lawndart Posted at: 2017-11-03T20:32:31.653Z Reads: 250

```
VESC don't handle 12s battery packs  very well. Well they can but you got to be careful  with your gearing and your settings or your blow it. Upgrading  to focbox would be much safer, and a little more forgiving. Or go with a 10s4p.
```

---
## \#6 Posted by: Luuke Posted at: 2017-11-03T20:41:41.241Z Reads: 253

```
Is there any 190KV sealed Motor to buy??

25R have 20A each. 3P means 60A!
30Q just have 15A. That means only 45A @ 3P. Why do you prefere the 30Q then?

Change gearing later is not the issue.

I have those trucks mounted on my boards atm. So I want to try one of those.

But can handle Voltage: 8V to 60V (Up to 14S LiPo Voltage), right? So 12S shouldn't be an issue.
WHY is focbox much safer and forgiving?
I prefere sealed and sensored motor. But since it has 170KV i really want to go for 12S.
```

---
## \#7 Posted by: Rinzler Posted at: 2017-11-03T20:50:41.292Z Reads: 247

```
@Luuke The cell ratings are often false. In this case the samsung 30q cells perform better than 25rs because they have a lower internal resistance, less voltage sag. When picking cells is it smart to look at discharge graphs found on google, there is a vape guy that does all the independent testing. You dont want to run electronics at their max, leave some slack. I would recommend running at 10s if you want lessen you chances of future issues. Focbox is an improvement over the  4.12 vesc, they solved some issues and made it more stable and powerful. It is still a Vesc which means it is not bulletproof.
```

---
## \#8 Posted by: pat.speed Posted at: 2017-11-03T21:04:07.850Z Reads: 237

```
Have a look on alien power systems they might have a sealed 190kv motor. I also would recommend going to 10s just to be safe
```

---
## \#9 Posted by: Luuke Posted at: 2017-11-04T13:48:09.779Z Reads: 229

```
30Q seems to be really cool!
20% more capacity for 30% higher costs.
http://www.taschenlampen-forum.de/media/samsung-inr18650-30q-vs-inr18650-25r.13802/full

Couldn't find any other 6374 sealed motor arround 190 or 200KV.
So may I change gearset and use 170KV @ 10S.

What range could be possible with 10S3P INR18650-30Q?
```

---
## \#10 Posted by: Moros Posted at: 2017-11-04T14:04:38.117Z Reads: 240

```
[quote="Luuke, post:6, topic:37257"]
Is there any 190KV sealed Motor to buy??
[/quote]

I'm pretty sure [eskating.eu](https://eskating.eu/product/eskating-pro-motors-6374-190kv-waterproof-sealed-and-sensored/) sells that exact motor from maytech just in 190KV.  They also have a 6355 190KV one too.

Otherwise the only other ones I know of are 95% sealed from [street-wing.com](https://street-wing.com/product/6374-190-kv-motor/).  
[Alien power systems](http://alienpowersystem.com/?s=HEV&post_type=product) have a selection of similar motors.

I've only been looking at EU suppliers because that is where I am, so don't know what you can get in US or AUS.
```

---
## \#11 Posted by: Luuke Posted at: 2017-11-19T10:48:54.828Z Reads: 224

```
I desided to change my setup a little.

I will go for 10S3P, but stay with the 170KV. If I need higher speed I can change gearing.
For now I will go with 15/36 ratio, thanks to @fliess!
<img src="/uploads/db1493/original/3X/d/4/d49981805dc0d990df8dbf8a587200a700bf54c7.jpg" width="666" height="500"> 

Just installed my 90mm 83A Flywheels with fresh lubed Amphetamine Ceramics Gold bearings.
On long term I will try to use my 80mm DTC Concept wheels. I really like those wheels with great urethan component the aluminum core.

This is the Maytech 6374 motor I will use.
It is sealed and sensored. I missed to take a photo of the keyway.
<img src="/uploads/db1493/original/3X/4/b/4b6def5d22fe39fceffad83675f042b5f3736e33.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/e/4/e4cde53c8c33d1f94cfd8a01a1afa421b0b84c18.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/7/4/745b70c0b13391829499847e5c12a199091b5681.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/8/7/87fd5d611391b9fe93a7be44d894e82862d29c8d.jpg" width="666" height="500">
And this is the remote:
<img src="/uploads/db1493/original/3X/d/c/dcd0f263f28c8decfcd5f527d1c2c3099fe8c756.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/f/9/f9b32b8177482538570efde5ad0c2311ef8ac4d7.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/d/0/d0cf55cad868f7e06480f53007c2a66cf66d1b70.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/1/9/19a622a3614432ca7c5c79164a2cc85b5d155af3.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/e/d/ed3d8995399b417b7f9e469d2ed1b361627d7876.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/6/0/60c6f90466a5bdb934e7a7cb04929576bede6070.jpg" width="374" height="499"><img src="/uploads/db1493/original/3X/5/9/59400f195acf8edc067aadc11dcd08ea25e6b4b9.jpg" width="666" height="500">
```

---
## \#12 Posted by: fliess Posted at: 2017-11-19T11:27:19.469Z Reads: 202

```
@Luuke, good progress! Looking forward to finally ride together :smiley:
```

---
## \#13 Posted by: Luuke Posted at: 2018-01-06T12:47:53.824Z Reads: 278

```
my built is going really slow. Didn't expact that....
Could manage a proper motormount for my Kodiak trucks. So i will go with some caliber II for now :confused:
And I am still waiting for my focbox.

But hear is my first printed part for my 3P battery pack:
<img src="/uploads/db1493/original/3X/5/b/5b0ed8cbfc536f4b0932134febd4d1e1fc0d8e7b.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/8/8/8817f01ee959471d2d5519d64dcd8733fa14ffca.jpg" width="666" height="500">

It provides single cell level fusing and supports to route the wires for the BMS.
Further i will connect the bus bars with copper mesh wire.
I hope the PLA can withstand the heat?! But I didn't expact more than 50°C here, right?

This is a first test of a anti spark switch:
<img src="/uploads/db1493/original/3X/1/4/140b948eaba3804f2457eb244c032848a4182d30.jpg" width="281" height="500">
```

---
## \#14 Posted by: Luuke Posted at: 2018-03-04T10:48:38.628Z Reads: 261

```
It's time for a little update on my build :slight_smile: 

PCB of the Focbox is protectet via 70 Super. To not decrease the heat transfer rate of the FETs they are covered with tape for that process.
I also covered the PCB of my remote and receiver.
 ![0|375x500](upload://eSPSWNkSDqdycOSJz64hw9P11nf.jpg)

This is my single fuse 10S3P battery pack.
the core is very flexible. With a lot of heatshrink it isn't that flexible anymore. But it is unlikely to damage the pack by flexing it.
The positve pole has some nickel on it to solder the the fuse on. And it is protected against short circuits to the housing (negative pole) 
![1|690x388](upload://wjy63o1aR0yCKWIaeFvKydrHzvC.jpg)
![3|690x224](upload://7eaWfTziGxbp6Dn1zLMyHwTvMgR.jpg)
![2|690x388](upload://nINsKIujgBbxuXTZU0DoxKkJbO4.jpg)
![29|374x499](upload://7pNJfxWloEhq5EjBgLeB00Fkka3.jpg)
![26|374x499](upload://qNY6GwUdXzbVwbVlu3sexHH9kQk.jpg)
![4|690x240](upload://4zi8bMrqQjnIKFK7u2WgqOQXX0j.jpg)
![5|690x388](upload://bB12JRGGr4Kqop0U5lRzk6nImfV.jpg)

Cell individual charger made by 10 pcs 5V ACDC Converter and 10 pcs TP4056
![7|690x388](upload://2shGfst9DxHqbGFycPW9msACn9W.jpg)
![8|352x500](upload://h5WWmsCdDltJ43zF4ePqLPviPiZ.jpg)

Hobbyking parts: motor mount, pulleys, belt
The Wheelpully is 20mm wide. So I had to cut it down to 15mm.
![6|690x388](upload://9zmxo7yNUrG33pReLaOHQU1SLUq.jpg)

I have to modify my Tesseract Cantellated to fit 1/2" riser, 90mm Flywheels and 44° Caliber trucks.
Right now I still have wheelsbites.
Or is there any other option? Maybe other bushings?
![9|281x500](upload://otovqpjGEZIa6OENDCgvYYVFT33.jpg)![10|281x500](upload://smbHqymO4L16yiiIfFheRTRXzZS.jpg)
```

---
## \#15 Posted by: Der6FingerJo Posted at: 2018-03-06T12:40:38.639Z Reads: 228

```
Man i didn't expect someone to actually build such a frankenstein charger, i love it! :smiley:

The rest looks great too, i really like the cell level fusing. Do you think one could get away without using nickel bits on the cells and just soldering the wire directly to them?
```

---
## \#16 Posted by: Luuke Posted at: 2018-05-13T17:29:48.874Z Reads: 188

```
[quote="Der6FingerJo, post:15, topic:37257"]Man i didn’t expect someone to actually build such a frankenstein charger, i love it! :smiley:[/quote]
yeah, it really looks strange. But it is doing it's job pretty good :)[/quote]

[quote="Der6FingerJo, post:15, topic:37257"]The rest looks great too, i really like the cell level fusing. Do you think one could get away without using nickel bits on the cells and just soldering the wire directly to them?[/quote]
Sure, you can solder direct to the positive pole.
But i wanted to stress the cells as less as possible. And doing it with this extra nickle you are adding some more clearance between the positive pole and the edge of the housing, which is negative pole respectively your 3D-print case.
```

---
## \#17 Posted by: petter Posted at: 2018-05-28T14:36:52.324Z Reads: 155

```
what gauge is your cell fuse? It looks pretty beefy, according to [this](https://www.powerstream.com/wire-fusing-currents.htm) for example, it might take a pretty high current to actually burn off.. the biggest problem being that if something goes wonky with a cell, you still might not have the amps/voltage difference to actually get up to that current and burn it off. Nice setup though, even if fuse wires is a tricky business.
```

---
## \#18 Posted by: briman05 Posted at: 2018-05-28T16:25:08.566Z Reads: 148

```
I would do sidewinders because the polar bears are tkp
```

---
## \#19 Posted by: Luuke Posted at: 2018-05-29T08:01:33.683Z Reads: 137

```
It is 19 AWG copper. That means 70A fusing current.
20 oder 21 AWG may would be better to use, you are right.

But I think in case of misuse 70A per cell could be easily provided for short terms. Then the fuse wire should blow off.
```

---
## \#20 Posted by: Luuke Posted at: 2018-05-29T08:02:44.745Z Reads: 135

```
At the end I went for caliber II :frowning:
wasn't able to create a well aligned mount for my bear kodiaks....
But with the right bushing setup they are not that bad :)
```

---
## \#21 Posted by: deucesdown Posted at: 2018-12-08T17:08:14.033Z Reads: 90

```
[quote="Luuke, post:14, topic:37257"]
10 pcs 5V ACDC Converter
[/quote]

@Luuke nice stuff! Those ACDC converters have transformers on them? Isolated outputs? Nice!
```

---
## \#22 Posted by: Luuke Posted at: 2019-01-05T10:43:27.897Z Reads: 74

```
Transformers? sure! They convert the AC Voltage of 110V - 240V  to 5V DC!
What do you mean by isolated Outputs? Which connection should be isolated?
```

---
## \#23 Posted by: deucesdown Posted at: 2019-01-05T15:15:03.743Z Reads: 73

```
Hey thanks for answering. I saw you post in another thread confirming. What I meant was, do those ac dc 5v converters isolate the ground?

Hey next question, do the acdc (oi oi oi!) converters get hot?

Thanks for making the franken charger and posting man. I have parts on the way for a 2 amp version -- I think I'll end up with the TP5000 modules with the heat sink on the back, about $1.65 per piece.
```

---
## \#24 Posted by: Luuke Posted at: 2019-01-05T18:28:06.810Z Reads: 66

```
The converters may get a little warm, but definitely  not hot.
2A version sounds great! Let me know when you are done with it! And think about choosing a 2A 5V ACDC converter ;)
```

---
## \#25 Posted by: deucesdown Posted at: 2019-01-05T18:43:46.269Z Reads: 75

```
Yeah here's my list.

https://www.electric-skateboard.builders/t/cheap-diy-12s-balance-charger-idea/76695/52?u=deucesdown

Bought the 3a tp4056 but I think that was a mistake. Bought some tp5000 2a after watching this video.

https://youtu.be/u4CQ62PsLiI

The buck converters, hard to find super cheap ones that are more than 10w.
```

---
## \#26 Posted by: Benjamin899 Posted at: 2019-01-08T21:45:26.144Z Reads: 59

```
great find, i was about to buy those too.
```

---
