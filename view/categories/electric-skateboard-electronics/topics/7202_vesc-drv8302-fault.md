# VESC DRV8302 Fault

### Replies: 35 Views: 4313

## \#1 Posted by: racidon Posted at: 2016-08-06T03:40:09.471Z Reads: 272

```
Kind of over the constant barriers I have with just having a simple eSk8. Can anyone please tell me how to fix this issue or even what ESC I can use in place of the VESC using SpaceCell Pro 3 (10s3p) and SK3-6372? I don't want to have to wait for the week or two I will now have to wait for my other VESC because of the PoS postal service that Enertion uses sent my VESC to the other side of the country. I also don't want to order another one because I don't want to have to deal with the postal service Enertion uses.
Here's a screen cap of realtime data (moto detection fails) 
<img src="/uploads/db1493/original/2X/4/4980c41032252c84c1edfe0bad7fb327402d5475.png" width="690" height="406">
```

---
## \#2 Posted by: Jinra Posted at: 2016-08-06T04:24:27.288Z Reads: 254

```
Looks like your DRV is fried, could you take a look at it and tell us if you see any burn marks on it? Mostly likely you'll have to get it replaced.
```

---
## \#3 Posted by: onloop Posted at: 2016-08-06T04:48:27.351Z Reads: 249

```
some DRV faults can be resolved by a simple reboot, some can be related to connection problems with your phase wires, or a bad motor detection, please rule out the obvious stuff.
 
Please post some photos, also check the power wires are not shorting the pins.

There are about 11 different things that can cause a DRV error.

Is this an Enertion VESC?
What country are you in?
Did you buy the VESC Platinum?
You might be interested in buying the [platinum warranty](http://www.enertionboards.com/electric-skateboard-parts/1yr-vesc-replacement-warranty/) separately & we can send you a brand new unit.
```

---
## \#4 Posted by: racidon Posted at: 2016-08-06T05:01:14.035Z Reads: 242

```
no obvious burn marks, I also tried without a connected motor and got the same result, does the same error happen if no motor is present?
```

---
## \#5 Posted by: racidon Posted at: 2016-08-06T05:03:09.703Z Reads: 237

```
looks like the motor case has been cutting into the wire unsulation. I will check out possible shorts.  It's enertion, not platinum, Australia, if you check out my topic about courier companies you'll understand the frustration is more directed to Couriers Please that you use.
If I order another off you could I pay the difference for express Aus post?
```

---
## \#6 Posted by: Jinra Posted at: 2016-08-06T05:03:24.047Z Reads: 234

```
Have you tried rebooting like onloop suggested? You could try re-flashing the f/w (if you know what you're doing). I would imagine it would still error without a motor.
```

---
## \#7 Posted by: Jinra Posted at: 2016-08-06T05:03:57.754Z Reads: 230

```
See this thread, very important!

http://www.electric-skateboard.builders/t/vesc-faq-negative-squared-cross-mark-warning-negative-squared-cross-mark-risk-of-short/6805/71
```

---
## \#8 Posted by: racidon Posted at: 2016-08-06T05:04:26.411Z Reads: 221

```
reboot is turning on/off yeah?
I have no issue with flashing firmware, it can be done via USB yeah? Also will I need to backup my XML to apply settings or will I need to re-do it all?
```

---
## \#9 Posted by: Jinra Posted at: 2016-08-06T05:05:20.947Z Reads: 221

```
You could back up the XML, but it shouldn't be too much to reconfigure. You can do it on the firmware tab in BLDC tool.
```

---
## \#10 Posted by: racidon Posted at: 2016-08-06T05:05:59.090Z Reads: 217

```
Already know about that, the VESC I have was to replace my one that had this issue before onloop knew about it
http://www.electric-skateboard.builders/t/spacecell-or-vesc-problem-no-connection-blue-light-on-l3-100/6686/13
```

---
## \#11 Posted by: racidon Posted at: 2016-08-06T05:11:22.119Z Reads: 201

```
how do i know the version of vesc I'm working with (most recent from enertion) is it 4.8?
```

---
## \#12 Posted by: Jinra Posted at: 2016-08-06T05:12:15.900Z Reads: 198

```
Should be 4.12, but it's printed on the PCB itself.
```

---
## \#13 Posted by: racidon Posted at: 2016-08-06T05:44:10.682Z Reads: 194

```
The firmware version was 2.18, but all the firmwares I seem to be able to get all read as 2.15 and BLDC tool stays in limited connection
```

---
## \#14 Posted by: Jinra Posted at: 2016-08-06T05:47:39.378Z Reads: 191

```
hardware version and software version are different. New Enertion VESCs should be h/w 4.12 and f/w 2.18. If you flash the wrong version for the hardware you might brick the VESC.

Not sure what you mean by having 2.18 but reading as 2.15?
```

---
## \#15 Posted by: racidon Posted at: 2016-08-06T05:50:00.632Z Reads: 191

```
I know that. Sorry I wasn't clear.
My HW version is 4.12
I originally had 2.18 FW on the VESC before I did the re-flash. I used firmware that came with my BLDC tool (2.17/2.18 compatible tool) and each of them are reading as 2.15 FW
I went to Vedder's site and downloaded the 2.18 zip file of firmwares and each of these are reading as 2.15
Is there something I'm missing? Could you possibly attached a confirmed 2.18 default firmware please?
```

---
## \#16 Posted by: Jinra Posted at: 2016-08-06T05:51:13.319Z Reads: 188

```
Download from vesc.net.au. It should include a folder with a bunch of f/w's for different revisions.
```

---
## \#17 Posted by: Blasto Posted at: 2016-08-06T05:51:14.088Z Reads: 186

```
The firmware version and the bldc tool need to align, they need the same number

If you have firmware 2.18 get it here, thats the latest
http://vesc.net.au/download-now/

If you have firmware 2.15, you need the 2.15 bldc tool, get it here
http://vesc.net.au/BLDC-TOOL/Windows/OLD%20Versions/
```

---
## \#18 Posted by: racidon Posted at: 2016-08-06T06:03:43.616Z Reads: 182

```
I think it was just a tool error. Looks like I had to close it and open it back up again for it to get the correct firmware. Not sure why...
Should any of the three phase wires have a connection to each other?
I ran a circuit test and all three are positive for a connection
```

---
## \#19 Posted by: Blasto Posted at: 2016-08-06T06:06:31.633Z Reads: 179

```
[quote="racidon, post:18, topic:7202"]
Should any of the three phase wires have a connection to each other?
[/quote]

Yes and no, connect them, if your motor runs in the wrong direction, flip two wires
```

---
## \#20 Posted by: racidon Posted at: 2016-08-06T06:09:19.271Z Reads: 170

```
Sorry thought it went without saying. Flashing the firmware I still have a DRV fault
```

---
## \#21 Posted by: Blasto Posted at: 2016-08-06T06:14:04.808Z Reads: 158

```
Well this could be one of many things, first post a picture of your setup including the motor connections
```

---
## \#22 Posted by: lilracerboi Posted at: 2016-08-06T06:17:08.858Z Reads: 159

```
Does the DRV fault come up as soon as you turn it on?
I remember before my VESC ultimately died, it also had a DRV error, but it wasn't consistent.
When I turned it on, it would run fine, forward and reverse, but if I put it in a neutral state the VESC would flash red and show the DRV fault, then it would reset itself and repeat the process.

I did a motor detection and the DRV fault somehow disappeared.
No idea what happened.

This was happening while the Space Cell Pro 4 was hooked up, but I don't believe my issues were cause by it.
```

---
## \#23 Posted by: racidon Posted at: 2016-08-06T06:56:38.045Z Reads: 155

```
can do, just have to charge my phone.
How much of the motor internal wires be shielded? They seem like they are able to touch each other, however it looks to me they are all part of the windings in general
```

---
## \#24 Posted by: racidon Posted at: 2016-08-06T06:59:27.798Z Reads: 150

```
It might have the error on boot as it does flash red when first turned on however the DRV fault isn't there by the time I have it connected and only appears if I move the throttle
```

---
## \#25 Posted by: Jinra Posted at: 2016-08-06T07:03:11.072Z Reads: 148

```
They're enamel coated for insulation. Sometimes this can wear off and short though...
```

---
## \#26 Posted by: racidon Posted at: 2016-08-06T07:04:06.650Z Reads: 146

```
Well now I'm even having troubles keeping a stable connection via USB. It only lasts a few seconds before it freezes up and won't connect again until reboot.
So two main questions remain unanswered
What ESC can I use in place?
@onloop if I paid extra for a VESC would you deliver express via AusPost? (not dealing with Couriers Please ever again)
```

---
## \#27 Posted by: racidon Posted at: 2016-08-06T07:05:58.450Z Reads: 143

```
So should any of the 3 phase wires make any connection with another? IE if I connected a light and battery using two of the wires should that light then light up?
```

---
## \#28 Posted by: Jinra Posted at: 2016-08-06T07:08:43.332Z Reads: 141

```
Not sure how windings are done, but if they are shorting you can tell by trying to rotate the rotor can (no power needed). If there's heavy resistance, then it's shorting. You can also test it out by touching two of the phase wires together when unplugged.
```

---
## \#29 Posted by: onloop Posted at: 2016-08-06T07:15:06.398Z Reads: 142

```
Use a different cable, also try a different PC.

to use AUS POST express i would need to literally go to the post office, lots of time & manual work for that to happen, Couriers Please collect from my door. Also, i probably don't have any VESC in stock at the moment, that's a question for my warehouse manager. support@enertionboards.com

there are no other ESC i would recommend.

You really need to post pictures of what you are doing, what is the setup like.... Two dead VESC in a row normally means user error. Something is going wrong somewhere.
```

---
## \#30 Posted by: racidon Posted at: 2016-08-06T07:30:28.547Z Reads: 146

```
Confirmed it isn't currently shorting. but if the wires are put on the right angle they do. Seems the motor casing is quite sharp and has slowly cut into them. I'll pull it apart over the weekend and this issue myself I think so when I finally get my other VESC I don't have this issue again.
It would also explain why the damn thing came to a dead stop and threw me with the amount of resistance that applies.
```

---
## \#31 Posted by: Jinra Posted at: 2016-08-06T07:32:12.174Z Reads: 137

```
yea that'll do it. you'll most likely need a new ESC too, or repair your current one.
```

---
## \#32 Posted by: racidon Posted at: 2016-08-06T07:33:58.277Z Reads: 141

```
Tried a different computer and 3 different cables.

Aus Post does offer eparcels, they also have Star Track that do pick up. However your business not mine. I just won't purchase from anyone now using couriers please. The VESC you guys sent me on the 3rd of Aug showed up at my door on the 5th (SA -> Vic). The other VESC you sent me on the 2nd of Aug is currently in Perth. Couriers Please outright lied to me multiple times in regards to this parcel and others.
I will post pictures once my phone is charged.
But here's one of tracking the parcel I just mentioned 

<img src="/uploads/db1493/original/2X/2/291972907d4bb9f78f60aaad2dfd33e6379ab196.png" width="674" height="174">

Edit:
Thought I should add my first VESC failed due to error on your part or your warehouse's part as admitted by you guys. So making the assumption of User error because of a past fault (even though I gave information on that) is quite insulting.
```

---
## \#33 Posted by: racidon Posted at: 2016-08-06T07:36:35.729Z Reads: 133

```
A career in computers will make it impossible for me to solder a new DRV on :slight_smile:
My hands are way too shakey for that
```

---
## \#34 Posted by: racidon Posted at: 2016-08-06T10:37:39.689Z Reads: 140

```
<img src="/uploads/db1493/original/2X/6/6ee8807880d6d28afe60b6875d855d7377b3c92c.jpg" width="300" height="500">
<img src="/uploads/db1493/original/2X/0/04115f5c758a8724932f0db3e3df821043882266.jpg" width="690" height="414">
<img src="/uploads/db1493/original/2X/5/52ddcf1c71ec84524ee38df7d9cb4eb2a1964088.jpg" width="690" height="414">
<img src="/uploads/db1493/original/2X/2/20682fe3c226fd7dfaee0a159dd71619a64eab2f.jpg" width="300" height="500">
<img src="/uploads/db1493/original/2X/8/8bd4f36955cf627fb453a0c16de295cb511dd8b8.jpg" width="690" height="414">
<img src="/uploads/db1493/original/2X/0/0c3069b247a92f92dd802cc4495dd404c36e8e65.jpg" width="300" height="500">
<img src="/uploads/db1493/original/2X/4/45bbec1331e3d89bf9a986497de16095c1c7c474.jpg" width="690" height="414">
<img src="/uploads/db1493/original/2X/f/f58e9263754faadcdbf8e5e3ea652dbf51c0ae9b.jpg" width="300" height="500">
<img src="/uploads/db1493/original/2X/3/32b238a3f847f27b72a1e23fd93bcc37cbd45175.jpg" width="300" height="500">
<img src="/uploads/db1493/original/2X/8/8a2a91260025d70339449a83509b65492672fa12.jpg" width="300" height="500">
```

---
## \#35 Posted by: racidon Posted at: 2016-08-06T10:44:06.876Z Reads: 133

```
I added images of how bad my soldering skills are (with limited tools)  (please note that it did have electrical tape over it like the rest. 
There's also images of the VESC showing no obvious burns although at this stage I'm quite certain it's a dead DRV. 
I might talk to chaka about getting him to repair for a cost and throw an idea his way about making it easier to use.
I'd also like to ask does anyone know of some form intermediary connection you could use for the mosfets to detect short circuits and cut power to the VESC? I'm sure car ESCs have this.
There's also an image of how I setup to use my setup with the computer (easier than having an entire board next to my PC).

The last of the motor and wires are showing the cut marks that have occurred. I'm going to put sikaflex in and around this area to prevent the wires moving. It should also help prevent "wicking" with water if I were to hit a puddle.
```

---
