# I Found Out How Evolve hit 70 km/h!

### Replies: 27 Views: 5168

## \#1 Posted by: VikasG Posted at: 2017-04-01T03:20:49.566Z Reads: 784

```
So I kept on pressing Evolve over and over and they finally caved in and gave me details. Basically, instead of changing the motors, Evolve adjusted their ESC to give massive power delivery and produce a ridiculous amount of low-end torque. 
https://www.youtube.com/watch?v=AidKstPWrrk
You can also see in the video above that the gear on the motor looks nothing like the stock one. From my calculations, the motor gear is either 28T or 30T. I'd like to hear your guys' thoughts on this.
```

---
## \#2 Posted by: Pantologist Posted at: 2017-04-01T04:01:17.893Z Reads: 763

```
Basically, they geared it for speed and not torque. That is almost a 1:1 gear ratio. ~30T motor pulley and 32T wheel pulley. 

Roughly the same power as a regular Evolve board unless they actually put name brand cells in this one.
```

---
## \#3 Posted by: VikasG Posted at: 2017-04-01T04:31:00.076Z Reads: 746

```
They didn't give me too many details about the battery other than "we changed battery settings". So I'm pretty sure they discharged the battery at a higher rate than they were rated for and/or they just put some really high quality cells in there. Either way, I'm 100% sure there were more changes than just the gearing.
```

---
## \#4 Posted by: Pantologist Posted at: 2017-04-01T05:23:11.776Z Reads: 705

```
You are probably right. Their regular battery sagged with normal use so there is no way they could increase that without something going haywire :stuck_out_tongue:

I bet it was a pack of LiFePO4s ;)
```

---
## \#5 Posted by: VikasG Posted at: 2017-04-01T05:45:27.559Z Reads: 666

```
That might be unlikely, their BMS communicates with their ESC. Due to LiFePO4 operating at a different voltage, the BMS wouldn't be compatible - making the ESC not work properly. 

They could be using Samsung 25R cells. They have a 20a continuous, but I believe they can do 100a burst. You only really draw max power for a short time during "take-off", so I assume setting up a 10s4p pack of 25R's could effectively produce 400a bursts - thus providing enough power for the short time you need it.
```

---
## \#6 Posted by: Eboosted Posted at: 2017-04-01T06:17:07.186Z Reads: 609

```
I'm ready to upgrade the electronics of my Bamboo GT. 

Keep the motors but upgrade electronics, has anyone done it?
```

---
## \#7 Posted by: Pantologist Posted at: 2017-04-01T14:40:01.015Z Reads: 575

```
Honestly, the the electronics are fine, the battery is what should be replaced with better cells.
```

---
## \#8 Posted by: okp Posted at: 2017-04-01T15:39:44.681Z Reads: 550

```
yeah that's what I'm gonna do to a GT Bamboo of a friend of mine. Double the battery pack and custom carbon enclosure for the fancy finish.
```

---
## \#9 Posted by: VikasG Posted at: 2017-04-01T17:56:23.792Z Reads: 520

```
Make sure you use the BMS that comes with the original battery! Otherwise the remote will be stuck in ECO mode.
```

---
## \#10 Posted by: okp Posted at: 2017-04-01T18:11:44.199Z Reads: 505

```
why? there's only a discharge cable + charge cable out of the battery.
```

---
## \#11 Posted by: VikasG Posted at: 2017-04-01T18:23:30.420Z Reads: 482

```
There's a BMS underneath the blue shrink wrap. The BMS communicates with the ESC and without that particular BMS, it will most likely give you a battery error and at best it will have you stuck in ECO mode.
```

---
## \#12 Posted by: Pantologist Posted at: 2017-04-01T20:58:13.390Z Reads: 455

```
How does it communicate? With what wire?

That's what @unik is asking.
```

---
## \#13 Posted by: VikasG Posted at: 2017-04-01T21:11:03.575Z Reads: 447

```
I'm not sure. The only information I've got from them in this regard is that if I plan on changing the battery, make sure to use the existing BMS or else the board will be stuck in ECO mode or throw a battery error.
```

---
## \#14 Posted by: Eboosted Posted at: 2017-04-01T22:18:10.805Z Reads: 420

```
What battery are you going to fit? 10S4P?
```

---
## \#15 Posted by: Gabrielruck Posted at: 2017-06-21T21:57:22.582Z Reads: 378

```
if you where to replace the stock battery for some LG 18650 I'm sure you'd get a 25% increase on speed and about 5 km more of autonomy. wich means you could replace the motors for 200kv+ and you wouldn't get burn out eaven with the ESC evolve has.
```

---
## \#16 Posted by: Nath Posted at: 2017-07-25T08:23:01.328Z Reads: 352

```
no. there are two other cables on a gt bms. you need to use it unless you plan to redesign all the electronics
```

---
## \#17 Posted by: Biscione Posted at: 2017-08-02T18:09:55.238Z Reads: 345

```
It is an UART protocol, I managed to spy it, but didn't decoded it yet, I am waiting for the oscilloscope, that's the proper tool for this task:-D
Anyway, shouldn't be big of a deal, but I just refuse to do it with the crappy logic analyzer i have right now...

But anyways, if you want to upgrade your battery, I think you can use the old BMS, and just keep the 10S topology, and you should be safe, I think there should be SW protection for overcurrent, so I would not worry about that, but wouldn't expect higher speed as well with these motors, but a larger range....
<img src="/uploads/db1493/original/3X/8/9/89abdb9fbcf6aca2e721d48aeaac98f98222b240.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/a/e/ae5816991227bd6e1e3e4a12b7cf93ced35e17bd.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/4/2/42d8d312ed81d298eb3ffe96010c7f0db4adf8e8.jpg" width="666" height="500">[Uploading...]() [Uploading...]() [Uploading...]() [Uploading...]()
```

---
## \#18 Posted by: StygianXVII Posted at: 2018-03-28T23:02:59.019Z Reads: 242

```
How can I adjust the ESC on my board too? Do I need to change the gear ratio? I also have 220kv sensored brushless motors on the way if that matters
Thanks
```

---
## \#19 Posted by: Janosh Posted at: 2018-04-22T20:42:31.510Z Reads: 224

```
Did you make any progress of decoding the comunication between the BMS and the ESC?
```

---
## \#20 Posted by: Biscione Posted at: 2018-04-23T16:07:25.324Z Reads: 205

```
Ah, a long time back I have also managed to decoee it as I remember, but I haven't paid too much attention because I am a little bit concerned for the safety of a homemade battery pack.

However, If you want, I can spend some time making some scope captures, and send you all the details you need. with serial decoding and stuff...

Just let me kn9w if needed, and I will upload the scope spy. All you need for reading the captures is picotech toftware for pc based oscillocopes.

regards,
Victor
```

---
## \#21 Posted by: Biscione Posted at: 2018-04-23T16:10:26.744Z Reads: 197

```
BTW:![56|375x500](upload://hYuFlusSiKEHVtL8aQBLjdUeKPf.jpeg)

Can anyone help me with some instructions of how I can get a new deck and front truck?
```

---
## \#22 Posted by: Janosh Posted at: 2018-04-23T16:17:55.987Z Reads: 188

```
Hi,

Ialready ordered a logicanalyser to do it myself.
But if you got something I would appreciate your help.

I think the BMS only provides some voltage data, temp etc. nothing special.
And the ESC does the rest of the work.
If  the ESC does not receive this data it will be stuck in ECO.
```

---
## \#24 Posted by: Biscione Posted at: 2018-04-23T16:37:57.275Z Reads: 178

```
unfortunately this forum only allows me to upload images, so the *.psdata format aint good.
```

---
## \#25 Posted by: Janosh Posted at: 2018-04-23T16:46:19.704Z Reads: 181

```
If you want I can send you a shared folder of my google drive.
```

---
## \#26 Posted by: Eretron Posted at: 2018-05-19T17:55:41.647Z Reads: 162

```
Any update on this? I would like to use custom battery but without bms at all. So I am looking for a way to "fake" the esc  that the bms is connected. 

Thanks in advance
```

---
## \#27 Posted by: AdeyD Posted at: 2019-12-16T16:10:56.628Z Reads: 50

```
Hey dude. Ive been reading ur comments and would like to know here I can get upgraded electronics for my GTX board as I have a BMS down on my board. Thanks AD
```

---
## \#28 Posted by: Eboosted Posted at: 2019-12-16T16:15:57.812Z Reads: 50

```
The best way to upgrade your Evolve Bamboo GT is to swap all electronics and enclosure. You will have an amazing board, double the range, 100% more torque, smooth acceleration and 100% more reliable.

I offer the ebox if you are interested, this consist in a 12S5P battery pack 18650 Samsung 30T cells, BMS for charging, charge port, Focbox Unity, remote control and a the Evolve enclosure.

Please hit mt up by PM to give you the total price.
```

---
