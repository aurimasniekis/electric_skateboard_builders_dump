# How do I add temp sensors to a motor and wire them to a VESC?

### Replies: 30 Views: 5141

## \#1 Posted by: deke997 Posted at: 2016-11-06T02:23:18.034Z Reads: 357

```
Hey guys,

I noticed that BLDC Tool has a setting for motor temperature limits. However, I don't know how to actually wire a temp sensor to the vesc. Is this doable? I haven't seen anyone on here talking about temp sensors on their motors..

Also, if it is possible, which sensors do I use? I was thinking about a cheap probe sensor like [this](http://www.ebay.com/itm/1M-NTC-Thermistor-Accuracy-Temperature-Sensor-1-3470-Waterproof-Probe-Cable-/361327463528?hash=item5420cb8c68:g:ObEAAOSwLVZViRP6) one.

Let me know!
```

---
## \#2 Posted by: saul Posted at: 2016-11-06T02:49:35.030Z Reads: 359

```
pretty sure it uses the temp sensor in the drv chip.

you could add a thermistor or something on one of the vesc analog lines. but you'd have to modify the firmware to read the proper pin and configure the sensor.

Totally doable if you can solder and program, but I don't think its worth the work.
i think v6 will have more temp sensors...
```

---
## \#3 Posted by: zmoney Posted at: 2016-11-06T02:53:33.792Z Reads: 341

```
If you want to check the temp of the Mosfets then you can go under Realtime Data, click on the Temperatures tab, and check off Active Sampling.
```

---
## \#4 Posted by: Namasaki Posted at: 2016-11-06T04:05:48.262Z Reads: 328

```
[quote="deke997, post:1, topic:12563"]
 I haven't seen anyone on here talking about temp sensors on their motors..
[/quote]
I don't think motor temp is an issue normally. 
If your motors are running too hot, it's likely because of the setup. Too high KV or too high gearing  
I've  checked my motors after climbing a fairly steep hill and they barely got warm.
10s, 190kv, 15/36 gears and 83mm wheels
```

---
## \#5 Posted by: deke997 Posted at: 2016-11-06T12:30:39.806Z Reads: 301

```
[quote="zmoney, post:3, topic:12563, full:true"]
If you want to check the temp of the Mosfets then you can go under Realtime Data, click on the Temperatures tab, and check off Active Sampling.
[/quote]


I do not want to check the temp of the Mosfets. I want to check the temp of my motor.
```

---
## \#6 Posted by: deke997 Posted at: 2016-11-06T12:38:09.992Z Reads: 285

```
[quote="saul, post:2, topic:12563, full:true"]
pretty sure it uses the temp sensor in the drv chip.

you could add a thermistor or something on one of the vesc analog lines. but you'd have to modify the firmware to read the proper pin and configure the sensor.

Totally doable if you can solder and program, but I don't think its worth the work.
i think v6 will have more temp sensors...
[/quote]

That does sound like a lot of work.. I will be prototyping some new designs, and I really need some sort of temperature monitor. I was hoping that the VESC could do it, because I would like to see a temperature graph over time compared to a graph of output amperage, and the VESC has some nice graphs on the Realtime Data tab.

I wouldn't be against soldering to the VESC and programming, but I would need some assistance from someone on the forum who know a bit more than me. If that ends up being too much work, are there any other solutions that will give me what I'm looking for?
```

---
## \#7 Posted by: deke997 Posted at: 2016-11-06T12:40:50.293Z Reads: 270

```
[quote="Namasaki, post:4, topic:12563"]
I don't think motor temp is an issue normally. If your motors are running too hot, it's likely because of the setup. Too high KV or too high gearingI've  checked my motors after climbing a fairly steep hill and they barely got warm.10s, 190kv, 15/36 gears and 83mm wheels
[/quote]

I will be testing some pretty extreme setups, so I definitely need a temp monitor.
```

---
## \#8 Posted by: trbt555 Posted at: 2016-11-06T13:24:10.657Z Reads: 259

```
If you check the schematics on Github you'll see the MCU has an input for an NTC temp sensor:
<img src="/uploads/db1493/original/3X/b/0/b076bd8cf1554d3d5230a133cd5086086b9cc17b.jpg" width="494" height="384">

And there is a separate schematic for the sensor:
<img src="/uploads/db1493/original/3X/e/e/eed7fe68d0c60f12cf88918ff5ffb6df6060f136.jpg" width="313" height="355">

I've never heard of anyone usng this functionality though. Perhaps Vedder himself could help you over on his dedicated forum.
```

---
## \#9 Posted by: Namasaki Posted at: 2016-11-06T18:24:22.261Z Reads: 231

```
In that case, you could be the first to setup real time motor temp monitoring with the Vesc.
```

---
## \#10 Posted by: Pedrodemio Posted at: 2016-11-07T02:09:10.772Z Reads: 223

```
Somebody asked vedder on his forum about this, at the time the temperature cut-off was not implemented, don't know if he put it to work in the later firmware releases
```

---
## \#11 Posted by: deke997 Posted at: 2016-11-08T22:31:09.669Z Reads: 213

```
As soon as I get some free time, I'll ask vedder about how I can implement this. If VESC 6.0 still hasn't been released in the next month or two, I'll figure it out and keep you guys updated!
```

---
## \#12 Posted by: Maxid Posted at: 2017-01-19T16:02:24.684Z Reads: 204

```
Can't we just use the pin in the hall sensor plug? I mean it literally says it is for motor temp measurements :confused:
<img src="/uploads/db1493/original/3X/3/e/3ee0471a4303a348f93819a46cd605d4c3cde8a2.PNG" width="690" height="190">
```

---
## \#13 Posted by: Okami Posted at: 2017-01-19T16:10:42.305Z Reads: 205

```
So - how is it going for you?

Did you come up how to add external temp sensor to a vesc?

Or are you gonna wait for vesc 6 then ;)
```

---
## \#14 Posted by: deke997 Posted at: 2017-02-07T22:37:53.644Z Reads: 197

```
[quote="Maxid, post:12, topic:12563"]
Can't we just use the pin in the hall sensor plug? I mean it literally says it is for motor temp measurements :confused:
[/quote]

That's exactly what I plan on testing!

[quote="Okami, post:13, topic:12563"]
So - how is it going for you?

Did you come up how to add external temp sensor to a vesc?

Or are you gonna wait for vesc 6 then :wink:
[/quote]

I haven't gotten time yet. I'll probably tackle this during spring break. I'll keep you guys updated.
```

---
## \#15 Posted by: evoheyax Posted at: 2017-06-19T22:57:51.555Z Reads: 175

```
Any luck with adding the temp sensor?
```

---
## \#16 Posted by: Ackmaniac Posted at: 2017-06-19T23:07:06.595Z Reads: 173

```
I implemented the motor Temps sensor check once for Duffman in the firmware but the tests were not successful. If anybody has a temp sensor wired in the same configuration as the PCB temp sensor (same resistors) then I am happy to help with the software. It's not hard to implement temp cutoffs in that case. But I don't have temp sensors installed. Another cool feature would be to add another temp sensor to the slave vesc which checks the battery temperature. But no cutoff is needed there because these Temps will never be a issue as long as the battery isn't undersised for the system. So it only would be for interest.

OH and the motor Temperatur isn't added to the actual 2.18 firmware. It's only avaliable in the bldc-tool but does nothing in the firmware.
```

---
## \#17 Posted by: notger Posted at: 2017-08-09T23:53:40.867Z Reads: 160

```
How is it going with temp-sensor "inplementations".
2.18 is still the actual Firmware,....
So will the VESC 4 Firmware actually be further developed, probably not cause of the VESC6.
So it would be up to some of you coding-freaks out there to finish this work, ahh ? ,-)
```

---
## \#18 Posted by: lrdesigns Posted at: 2017-08-10T04:39:31.112Z Reads: 164

```
The trampa motors have a built in temp sensor. So surely someone has these and version 4 vescs. 

http://www.trampaboards.com/electronic-motors-c-532.html

It would be really cool if you can get this to work with your firmware. I wonder if it will work on the new 3.1 firmware?

As to the people who asked what you need to hook one up? A 10k ohm thermistor. From the temp pin in the motor angle sensor set, - thermistor - back to ground. 

https://www.sparkfun.com/products/250
```

---
## \#19 Posted by: notger Posted at: 2017-08-10T09:42:52.602Z Reads: 155

```
[quote="lrdesigns, post:18, topic:12563"]
The trampa motors have a built in temp sensor
[/quote]

But that does not mean that it is supported by the VESC.

[quote="lrdesigns, post:18, topic:12563"]
I wonder if it will work on the new 3.1 firmware?
[/quote]

what ? a new FW, is it just for VESC 6 or also for VESC 4 ?

greets

Gernot
```

---
## \#20 Posted by: evoheyax Posted at: 2017-08-10T15:13:16.325Z Reads: 158

```
Do you need anything else? how is that hooked up, since theres only 2 pins?
```

---
## \#21 Posted by: lrdesigns Posted at: 2017-08-10T15:25:37.092Z Reads: 150

```
I don't think so, one leg goes to the sensor pin on the vesc and the other leg to ground. Simple.
```

---
## \#22 Posted by: rich Posted at: 2017-08-11T20:39:28.885Z Reads: 141

```
I have trampa motors, HW 4.12 and FW 3.26, the motor temperature realtime data is 
working  and motor temp cutoff should work, too but I never got the motors that hot.
```

---
## \#23 Posted by: notger Posted at: 2017-08-11T22:19:45.062Z Reads: 145

```
So you have a VESC 6, right ?
Semms the motor temp is implemented then in the new Firmwares.

what maximum Watts or Amps*Volts are you using on the Motor ?
```

---
## \#24 Posted by: rich Posted at: 2017-08-11T23:02:23.692Z Reads: 144

```
No, I have dual V4.12 with the new 3.26 firmware and the new VESC tool instead of BLDC tool. Additional to VESC 6 Vedder programmed new firmware for the old hardware 4.xx, too in combination with VESC tool.  I'm a beta tester but the new firmware and VESC tool should be public soon.


[quote="deke997, post:1, topic:12563"]
I noticed that BLDC Tool has a setting for motor temperature limits
[/quote]
Yes, but FW 2.18 and BLDC tool can't deal with motor temp sensor, but FW 3.26 can do it. In VESC tool you can monitor realtime data of mosfet temp & motor temp, it's great! Here a screenshot, it's T Motor :grinning:

<img src="/uploads/db1493/original/3X/d/4/d487e272d43b1458c348c15f1e7004c9487b49c6.jpg" width="690" height="388">

On my MTB I run my motors in FOC and 45A motor max each, just for safety but I also gonna try 50-60A (the motors are rated 60A) and see if there is a difference but it's still very powerful. I found out that motors with hall sensors need FOC for proper startup, The new firmware has a lot of improvements regarding FOC.
```

---
## \#25 Posted by: notger Posted at: 2017-08-12T15:37:04.960Z Reads: 132

```
Whoo, I'm really looking forward to the release, can't wait to see the functions of the new tool.

one Question in advance:
does it have a "Watt-controll" like @Ackmaniac 's BLDC-Tool and the option of adding cruise controll to a RC-> PPM control like (GT2B-receiver)?? 

greets
Notger
```

---
## \#26 Posted by: rich Posted at: 2017-08-12T16:23:37.181Z Reads: 123

```
There is no Watt control mode but adjustable throttle curve. There are also improvements in FOC. I doubt cruise control is possible like in FW 2.54 but I'm sure @Ackmaniac will work on a new mod once FW 3.26 is public. I hope so because his app is not working with the new FW and V4.12
```

---
## \#27 Posted by: Ackmaniac Posted at: 2017-08-12T16:28:15.481Z Reads: 130

```
The app works with it, but only for like 5 minutes. Then it doesn't work anymore (could be 5 min or after a restart). just thought the UART connections are fried because of a broken Bluetooth module. But when you flash the firmware back to 2.54 it works again. So it must be software related. 
But at the moment it only is possible to show the reltimedata.
```

---
## \#28 Posted by: rich Posted at: 2017-08-12T16:44:34.510Z Reads: 123

```
Hey Ackmaniac, love your app, had it running a couple of days with FW 2.54 and 2.18. With FW 3.26 the app connects to the HM-10 but the realtime data values stay zero. After FW downgrade it worked again as you said. I run FOC with FW 3.26 now and won't downgrade again so I'm looking forward to use your app in the future because it's great, thumbs up!
```

---
## \#29 Posted by: evoheyax Posted at: 2017-08-12T16:58:30.967Z Reads: 123

```
I'm assuming vedder has changed the firmware quite a bit. Just as started putting together the 2.18 firmware in my mind.

Is there any way I can get my hands on this firmware? Need to update my app asap for this firmware.
```

---
## \#30 Posted by: rich Posted at: 2017-08-12T17:05:28.477Z Reads: 120

```
[quote="evoheyax, post:29, topic:12563"]
Is there any way I can get my hands on this firmware?
[/quote]

As far as I know it should be released soon.
```

---
