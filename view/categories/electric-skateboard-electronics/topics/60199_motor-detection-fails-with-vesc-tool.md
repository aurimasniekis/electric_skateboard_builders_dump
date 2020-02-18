# Motor detection fails with VESC tool

### Replies: 44 Views: 2082

## \#1 Posted by: mat Posted at: 2018-06-27T11:16:24.759Z Reads: 280

```
Hi!

I have a setup with the following parts:

* Maytech VESC (V. 4.12, firmware 3.38 flashed through VESC Tool)
* Maxon EC 45 motor (https://www.maxonmotor.com/maxon/view/product/motor/ecmotor/ecflat/ecflat45/400106)
* Power supply (5A, ~20V)

I think I read all the topics there are on the forum but I still didn't manage to make the motor detection work in BLDC mode.

Here are the settings from the setup wizard:
![image|690x410](upload://x9EGaKSvBDFmauRnOiUtFWDFUQw.png)
![image|690x412](upload://36QZkIzC1v23uW5QbhZ91aJx9Jq.png)
![image|690x412](upload://aYy5y3rsM37lrC5wPNRCEkRr9un.png)

Here are the settings I tried the tool to work with:
![image|690x412](upload://pp6wNwLfWsPPxq1J0YDOKJ0jakN.png)

I played with all kinds of values for I, omega and D parameters without any luck. The ones that I think are closest to working are included in the last screenshot. Each time I start detection it ends up with **Bad detection result received**. 

Here is a video with motor behaviour:
https://www.youtube.com/watch?v=CpQTeBwQKlE

In the console I checked for faults with commands _fault_ and _faults_ and received FAULT_CODE_NONE and No faults registered since startup.

Some other things I checked:

* The continuity on all the wires is OK
* I swapped phase wires around (the direction of the spinning changed but nothing more)

I also tried FOC mode once, in that mode I was able to fetch all run the detection correctly, however the driving of the motor (either through RPM set or arrow keys) didn't work very well.

Any ideas on what else can I check would be highly appreciated!
```

---
## \#2 Posted by: Blasto Posted at: 2018-06-27T12:16:24.809Z Reads: 236

```
You’re being throttled by the battery cutoffs.

Make these values under 20V

Cutoff start 12V
Cutoff stop 10V 

For lab testing with psu

![image|281x500](upload://a0saLlaClLLM9qbDmtDNpz0Oumw.jpeg)
```

---
## \#3 Posted by: mat Posted at: 2018-06-27T13:01:36.598Z Reads: 216

```
[quote="Blasto, post:2, topic:60199"]
You’re being throttled by the battery cutoffs.

Make these values under 20V

Cutoff start 12V
Cutoff stop 10V

For lab testing with psu
[/quote]

Thanks for a tip! Should I do it even if the supplied Voltage is 20V? I changed the cutoff values to the ones you suggested and the behaviour is the same (at 20V and at 12V from my power supply). Do you have any ideas what I can test?
```

---
## \#4 Posted by: Blasto Posted at: 2018-06-27T13:38:00.360Z Reads: 210

```
Leave the power supply at 20V

Cut off start: if input voltage is lower than this value, your current will be limited. 

Cut off end: if input voltage is lower than this value, power to the motors will be completly throttled.

Other thing you can try is increase your detection current and increase the detection duty cycle (D)
```

---
## \#5 Posted by: mat Posted at: 2018-06-28T13:19:02.445Z Reads: 200

```
I tried modifying the detection current and duty cycle without any success. Do you have any ideas what else could I try?
```

---
## \#6 Posted by: mat Posted at: 2018-06-28T13:36:16.857Z Reads: 197

```
Here is also how the motor behaves during FOC flux linkage measurement, which in this case is successful (however the values seem a bit sketchy to me, especially the KI parameter):

https://www.youtube.com/watch?v=UVT9HkrUmEQ

And the results:
![image|690x83](upload://l4UJX0e8ci9LJy5QOIsNQJiriit.png)
```

---
## \#7 Posted by: Blasto Posted at: 2018-06-28T14:13:28.866Z Reads: 186

```
try these detection parameters for foc detection

I: 2 to 4A 

D: 0.10 to 0.15  

w: 700 to 1200 ERPM

maybe @Deodand can have some input here, i've never played around with fancy maxon motors. I do find your flux linkage very low... but then again, lack of experience with this type of motor
```

---
## \#8 Posted by: Deodand Posted at: 2018-06-28T14:44:06.393Z Reads: 183

```
The flux linkage measurement is definitely too low. Resistance and inducatance measurements look ok.  Since it is a maxon motor the datasheet will give you rpm/V (which is kv) and you can use this to calculate flux linkage (lambda) and input it manually:

lambda = 60 / (sqrt(3) * pi * kv * pole_num)

If this doesn't work you may need to add [choke inductors](https://www.maxonmotor.com/maxon/view/product/accessory/drosseln/347919) to the windings if the winding inductance is too small. You wouldn't need these expensive ones, just an example. Some around 5-10 uH would be more than plenty.
```

---
## \#9 Posted by: mat Posted at: 2018-07-02T12:48:20.395Z Reads: 173

```
An update: All the things mentioned above were failing on me (the only thing I didn't try were the choke inductors). 

I just got my hands on another one of those motors and it works well with VESC out of the box.

Thanks for all the help!
```

---
## \#10 Posted by: briman05 Posted at: 2018-07-02T12:54:33.828Z Reads: 164

```
I would also change the battery max Amps as well
```

---
## \#11 Posted by: mat Posted at: 2018-07-02T13:18:36.051Z Reads: 163

```
Thanks! Would you change it even if working from 5A power supply? With the battery I would probably set it to  whatever is the discharge rate * capacity. Would that be correct?
```

---
## \#12 Posted by: briman05 Posted at: 2018-07-02T17:59:30.078Z Reads: 154

```
You would set it to the discharge rate x how ever many parallels you have
```

---
## \#13 Posted by: Fabrice Posted at: 2018-08-06T13:24:44.030Z Reads: 144

```
Hello, I have also the same problem. When I try to make a motor detection I have a bad result received .
```

---
## \#14 Posted by: briman05 Posted at: 2018-08-06T14:50:18.051Z Reads: 143

```
what firmware are you running? what vesc? what type of motor? and FOC or BLDC?
```

---
## \#15 Posted by: Fabrice Posted at: 2018-08-06T15:26:43.490Z Reads: 137

```
Hello Here what I have

2 x Torque 6355 Motors
2 x VESC : Turnigy SK8-ESC V4.12 For Electric Skateboard Conversion w/BEC
https://hobbyking.com/fr_fr/turnigy-sk8-esc-v4-12-for-electric-skateboard-conversion-w-bec.html
12S battery (2 x 65 5000mah 40C)

Fo now I just connected a single battery to vesc to configure it.

So I connected it to the battery and the motor. Then connected it to the PC. Then I launch VESC-Tool. Here they tell me that my firmware is old and that I have to update it cause I will stay in limited connection.

So I update it and now I'm in : FW 3.38 and 4.8 HW.

I start to configure Motor current Max, Regen and so on based on what I have read and from diyelectricskateboard customer service advises.

Then When I tried to make a Detect BLDC Parameters, I get a status failed ...

I've tried to change cutoff start and end to the barely minimum but nothing ...

I also tried to re-update VESC, still nothing ...
```

---
## \#16 Posted by: briman05 Posted at: 2018-08-06T17:28:36.598Z Reads: 130

```
You flashed the wrong firmware your vesc is a version 4.12 meaning it would be a hw412 in the vesc tool.  You flashed it with hw 4.8 that is the cause of your issues
```

---
## \#17 Posted by: Fabrice Posted at: 2018-08-06T19:32:30.162Z Reads: 134

```

Don't remember they ask me what firmware I wanted ... So I need to downgraded it ?
Is there a bin file for it ?
```

---
## \#18 Posted by: briman05 Posted at: 2018-08-06T20:11:51.387Z Reads: 134

```
no you updated the firmware and but when you flashed the firmware it was for the wrong hardware so you need to try and flash the firmware file for correct hardware which is 412. if you download @Ackmaniac esc tool it has a very easy step through guide to do your motor detection and remote set up after you do the firmware update
```

---
## \#19 Posted by: Fabrice Posted at: 2018-08-06T21:36:28.910Z Reads: 131

```
So I try to reflash it now im in FW 3.01 HW 4.10

Detection work (Thanks=), it spin but not with the remote controller ...

I'm going to use y-splitter instead of CANBus. Do I have to configure each VESC independently then the receiver each time ? (I know i have to cut a wire to only have 5 V for the reveiver)

Best Regards
```

---
## \#20 Posted by: briman05 Posted at: 2018-08-06T22:05:35.678Z Reads: 124

```
Yes you will have to do each one independently honestly canbus or a lot easier because one is master one is slave is for master would be 0 and the salve would be 1
```

---
## \#21 Posted by: Fabrice Posted at: 2018-08-06T22:14:18.728Z Reads: 116

```

Thing is if the slave one goes down it's a shame but ok. But if the master goes down the slave also. So after many reads on the subject Y-splitter vs CANBus I chose a side !
```

---
## \#22 Posted by: briman05 Posted at: 2018-08-06T22:15:27.745Z Reads: 114

```
Just make sure everything is exactly the same.
```

---
## \#23 Posted by: Fabrice Posted at: 2018-08-07T07:30:22.825Z Reads: 114

```

I will post here how everything goes .
```

---
## \#24 Posted by: Fabrice Posted at: 2018-08-15T17:56:50.855Z Reads: 108

```
So I have more issues with the remote controller this time.

When I plug and pair it then use the trigger nothing happen = no motor speed.

blue light stop to blink on the receiver when i switch the remote on but that all.
```

---
## \#25 Posted by: briman05 Posted at: 2018-08-19T01:49:01.219Z Reads: 104

```
Do you have the Vesc set current or current no reverse or something like that?
```

---
## \#26 Posted by: Fabrice Posted at: 2018-08-21T14:03:25.934Z Reads: 108

```

Hello, So I'm not really sure of where it came from. I retried the procedure many time then when arrive to App Settings i just make next holding the trigger then it suddenly spin.

I'm gonna say that it is a bit too sensitive but it work.

The last problem remaining is about the speed of each motor. I have noticed that one goes faster than the other since there is 1-2 secondes difference when they stop. Also when I press the Trigger slowly one motor spin when the other one is slow.

I've check the VESC configuration but it's excatly the same for both and I tried to swap the VESC also but nothing changed.

its strange cauz it always the same motor that is slow. I'm not sure if at the end they reach the same speed, I guess but it really bother me.

I also thought it could came from the receiver signal that was different but it doesn't seem. 

Is there a way on VESC Tool to watch both motor ERPM at the same time ?
```

---
## \#27 Posted by: briman05 Posted at: 2018-08-21T18:17:24.468Z Reads: 98

```
Is traction control turned on because that would cause what you are seeing basically the master is lead and the slave is following.
```

---
## \#28 Posted by: Fabrice Posted at: 2018-08-22T07:36:37.018Z Reads: 94

```

Hello I use a spliter instead of CANBus so I have no master and slave.

But ok I'm gonna check that, do you know where this parameter is in vesc tool ?
```

---
## \#29 Posted by: briman05 Posted at: 2018-08-22T12:33:40.661Z Reads: 91

```
under ppm tab
```

---
## \#30 Posted by: Fabrice Posted at: 2018-08-25T13:48:54.028Z Reads: 89

```
So yes traction control is OFF for each so it's not that ....
```

---
## \#31 Posted by: Fabrice Posted at: 2018-08-25T15:46:57.072Z Reads: 89

```
![motor%201%20(slowest)|643x499](upload://bG2rHtcOV1LmqXErARhOwXwtXqb.png)![Motor%202%20(fastest)|690x373](upload://m8V1iFg0J71HpBZIWYDU2YguGqn.png)

Here's images from the vesc tool (taken at the same time on 2 pc connected to one VESC) whitout pushing the trigger. As you see at the very beginning value are already differents.
```

---
## \#32 Posted by: briman05 Posted at: 2018-08-28T11:38:20.286Z Reads: 80

```
They are both at zero erpms the one is drawing slightly more mah and wh but that’s is really it. It could be that one motor has a slightly different kv it should be ok.
```

---
## \#33 Posted by: Fabrice Posted at: 2018-08-28T12:43:59.787Z Reads: 79

```

I confirm they are both the same 6355 190KV.

The only concerned I had was if this difference has a huge impact on the peformance. Cause when I push the trigger they seem to have small ERPM difference (between 500 and 1000). When I brake both stop at the same time. If I just stop pushing and let the wheel stop I see that one stop 2 sec after (so I have concluded it was faster).

That's really weird. But if you say that's not bad. ok.
```

---
## \#34 Posted by: briman05 Posted at: 2018-08-28T21:21:40.165Z Reads: 75

```
When I meant KV I mean the actual kv it could have been made at a different factory than the other one and could have more or less winding when it was made which would effect the kv.  It should not cause a issue.  Are you testing it under your weight or just on the vesc tool
```

---
## \#35 Posted by: Fabrice Posted at: 2018-08-31T17:59:01.845Z Reads: 73

```
 > Are you testing it under your weight or just on the vesc tool

No not yet I haven't finished the enclosure yet.
I made the test without weight on the my work table.
```

---
## \#36 Posted by: briman05 Posted at: 2018-09-01T03:22:03.319Z Reads: 71

```
It is not a true test yet as it will probably not even be something you notice.
```

---
## \#37 Posted by: Fabrice Posted at: 2018-09-01T10:15:41.433Z Reads: 69

```
Do you know where I can find a good anti-spark switch.

https://flipsky.net/collections/new-accessories/products/anti-spark-switch?variant=8291508092988

I bought this one but they lie it is incapble to handle more than 6S. It just fry 

The one from Mboard is a *** too and fry exactly the same and he lie about his product putting his lable on product made by other.

Don't where to find something good ..... and i can't complete the all thing without it.
```

---
## \#38 Posted by: briman05 Posted at: 2018-09-01T12:15:05.611Z Reads: 66

```
I loop a loop key as they pretty much never fail. They may not look pretty but it works.
```

---
## \#39 Posted by: Jansen Posted at: 2019-04-26T02:52:56.978Z Reads: 46

```
Hey @briman05 I believe this is my issue to on why I am failing my motor detection. I flashed the right ack 3.1 firmware but did 4.8 instead of the 410, 411, 412 or whatever it is for the hardware. I can't seem to figure out how to change this though... I can re-flash my focbox with the firmware again but it is still saying 48 for the hardware, any advice or direction you can give me on how to make sure it knows which hardware I have cause I've been trying everything and this seems to be the missing link and I just want to ride this new build so dam bad! LMK what I need to do if you could brotha.... using Acks ESC tool with 3.1 hardware and have it correct on Focbox 1 so just need to do the same for FB 2 and can't figure out how!!! FML
```

---
## \#40 Posted by: briman05 Posted at: 2019-04-26T17:26:20.569Z Reads: 41

```
I think you need to reload the bootloader and then reflash it with the 410,411,412  If you search bootloader on here someone should have posted the link for it.
```

---
## \#41 Posted by: miguelspimpao Posted at: 2019-09-30T19:32:32.140Z Reads: 20

```
Hi guys, I´m new to the DIY esk8 scene. I ordered the cheapest (probably the worst) components avaialable. The components are from Flipsky. It's a chinese brand that have all the components at very reasonable prices.

After the first problem that appeared with the firmware (that I succefully flashed with a st link), now there's a second problem with the motor detection. When programming via vesc tool 1.23, after trying to detect my motor the following message appears: "could not measure motor resistance and inductance".

It's important to say that on friend of mine bought the same components from the same seller and his motor and FSESC is already running and had no problems programming it.

The VESC is a FSESC 4.12.

Anyone there that can help me ?
```

---
## \#42 Posted by: trampa Posted at: 2019-10-01T18:52:10.444Z Reads: 20

```
Contact Flipsky and get a replacement.
```

---
## \#43 Posted by: Miniproto Posted at: 2019-10-01T20:01:44.233Z Reads: 19

```
I had similar issues then found out the older VESC 0.95 version and had no problems after that.
It can be.. if not contact Flipsky.
```

---
## \#44 Posted by: miguelspimpao Posted at: 2019-10-06T10:21:56.040Z Reads: 15

```
Thanks a lot, in 0.95 version it can mesaure the resistance, but not the inductance, and the motor won't spin.. I already contacted Flipsky, waiting for a reply tomorrow.
```

---
