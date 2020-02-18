# Connecting a Brushed Motor to Vesc

### Replies: 28 Views: 4495

## \#1 Posted by: msthg5000 Posted at: 2016-11-26T18:58:14.503Z Reads: 312

```


I have a brushed DC motor (with 2 wires)
which I would like to connect to a VESC (with three wires for motor). After
doing some research I discovered that the VESC does support DC motors, however,
I was unable to figure out how to connect the brushed motor to the VESC. Can
anyone, give step by step instructions on how to connect the motor to the VESC
and how configure the Brushed DC motor using the BLDC tool. 

 

Note: The BLDC tool has a tab for DC
motors. Is that what you use to configure the VESC. Also I am using 2 DEWALT
20V MAX* Compact XR Lithium Ion Battery Pack- so is it possible for you guys to
tell how to configure the Motor for that battery setup.
```

---
## \#2 Posted by: laurnts Posted at: 2016-11-26T23:17:13.531Z Reads: 284

```
I am sorry but VESC is build for brushless motor only, it can't be used for brushed motor. For brushed motor ESC you can try to use https://www.indiegogo.com/projects/ragebridge-2-next-gen-motor-controller#/. Personally I havent got any experience building esk8 with brushed motor.
```

---
## \#3 Posted by: msthg5000 Posted at: 2016-11-26T23:21:50.751Z Reads: 278

```
However, when I tried to connect the brushed DC motor to the VESC it ran for 2 seconds then stopped. Doesn't this mean that it can run the brushed DC Motor at the correct setting? This was on FOC settings.
```

---
## \#4 Posted by: laurnts Posted at: 2016-11-26T23:32:41.885Z Reads: 257

```
As I remembered properly, Benjamin stated by himself that VESC are not meant for brushed motor. Brushed motor doesn't need ESC anyway. Just hook up voltage potentiometer and you have speed control in there.
```

---
## \#5 Posted by: rpn314 Posted at: 2016-11-26T23:40:10.378Z Reads: 244

```
I'm with you, I thought that's what DC meant....so what does it mean?
```

---
## \#6 Posted by: msthg5000 Posted at: 2016-11-26T23:41:30.906Z Reads: 236

```
The thing is we are making a scooter and it already has a brushed DC motor mounted so we would prefer not to take of the motor and mount a brushless one. Here are some images that led me to believe that connecting a brushed dc motor is possible to the VESC.<img src="/uploads/db1493/original/3X/8/a/8a81a542bac2e90de31b71a0c91ffe4ed9ee71a8.PNG" width="647" height="500"><img src="/uploads/db1493/original/3X/5/1/51a7994a0d298c82bac22c8d1c25092c18db1ad3.PNG" width="690" height="338">
```

---
## \#7 Posted by: Pedrodemio Posted at: 2016-11-26T23:50:31.186Z Reads: 207

```
My guess is that, as a lot of other features, BLDC tool has the option to be select, but that is not actually implemented on the firmware, take motor temperature limits, on the hardware side it has everything ready, but not working on the current firmware
```

---
## \#8 Posted by: rpn314 Posted at: 2016-11-26T23:58:35.839Z Reads: 200

```
Looking through the firmware on github, there's definitely something implemented. Still looking through it to see if it does what you need it to.
```

---
## \#9 Posted by: msthg5000 Posted at: 2016-11-26T23:59:54.173Z Reads: 199

```
Thank you any help will be very much appreciated!
```

---
## \#10 Posted by: laurnts Posted at: 2016-11-27T00:30:31.737Z Reads: 191

```
Sorry I might be wrong. I believe previously it wasn't supported, maybe now it does. But I would like to see brushed motor working with VESC as well.

Could you please post your VESC configuration and also state what VESC version you have.
```

---
## \#11 Posted by: msthg5000 Posted at: 2016-11-27T00:44:29.426Z Reads: 189

```
I am unable to post that information until Monday as this is a school project and I will not have access to the VESC until Monday. But here is a picture of the exact VESC I have so you might be able to tell. Furthermore, the VESC is not configured because of the whole brushed, brushless situation, however, I have given info on the battery we are using so if you might be able to tell me the best configuration for the VESC,<img src="/uploads/db1493/original/3X/a/4/a4fda3a843231bfb3943a278a3525898f8e936f9.jpg" width="690" height="491"> that will be very much appreciated.
```

---
## \#12 Posted by: erwincoumans Posted at: 2016-11-27T01:00:11.116Z Reads: 180

```
[quote="laurnts, post:4, topic:13711, full:true"]
As I remembered properly, Benjamin stated by himself that VESC are not meant for brushed motor. Brushed motor doesn't need ESC anyway. Just hook up voltage potentiometer and you have speed control in there.
[/quote]
VESC supports brushed DC motors just fine. In addition, Benjamin has several videos of brushed DC motors online:
https://www.youtube.com/watch?v=qqNOx57f2OU
```

---
## \#13 Posted by: msthg5000 Posted at: 2016-11-27T01:55:07.830Z Reads: 177

```
Could it be possible for you to explain how to setup the VESC with the brushed DC motor. A step by step instructions guide would be nice.
```

---
## \#14 Posted by: erwincoumans Posted at: 2016-11-27T03:32:54.209Z Reads: 167

```
[quote="msthg5000, post:13, topic:13711, full:true"]
Could it be possible for you to explain how to setup the VESC with the brushed DC motor. A step by step instructions guide would be nice
[/quote]

There is not much to tell: connect to the VESC using BLDC_Tool, select DC (instead of BLDC or FOC) in the most left tab. Then connect the first and third power cables (leave middle one open). Make sure the voltage going into the VESC doesn't exceed your DC motor voltage.

I just tried it with a brushed DC motor (12Volt) and it works just fine.
```

---
## \#16 Posted by: msthg5000 Posted at: 2016-11-27T15:28:56.560Z Reads: 143

```
[quote="erwincoumans, post:14, topic:13711"]
Then connect the first and third power cables (leave middle one open)
[/quote]

What do you mean by this?
```

---
## \#17 Posted by: lox897 Posted at: 2016-11-28T10:01:30.753Z Reads: 139

```
There are three wires coming out of the vesc on the middle side. Just use the side ones and not the middle to connect the motor. Not sure if polarity matters though.
```

---
## \#18 Posted by: msthg5000 Posted at: 2016-11-29T20:50:41.126Z Reads: 128

```
Thank you everybody for your help, the VESC is now working with the motor. 

**THANKS!**
```

---
## \#19 Posted by: jga Posted at: 2016-12-10T16:08:07.134Z Reads: 122

```
I suspect I will have the same problem: I want to change my AT big skate from lead to Li-ion battery, and I believe I have a brushed motor on it. I have just ordered a 10S4P and a VESC, and I am glad to see it is possible to make it work.
Was it difficult to do the set-up with the VESC?

And with regard to erwincoumans remark above
 [quote="erwincoumans, post:14, topic:13711"]
Make sure the voltage going into the VESC doesn't exceed your DC motor voltage.
[/quote]
my motor says 36V so do I need to limit the output of my battery through the VESC as it will be slightly above that limit?
```

---
## \#20 Posted by: Lambjr088 Posted at: 2018-08-30T23:10:16.701Z Reads: 72

```
I know its been awhile on this post but I want to know as well. "my motor says 36V so do I need to limit the output of my battery through the VESC as it will be slightly above that limit?" @lox897  @erwincoumans @msthg5000
```

---
## \#21 Posted by: Pedrodemio Posted at: 2018-08-30T23:18:00.388Z Reads: 75

```
You will be fine, what overheat a motor is the current

Of course in brushed motors too much voltage can damage/destroy the brushes, but no a bit more than the rated
```

---
## \#22 Posted by: Lambjr088 Posted at: 2018-08-31T01:40:13.469Z Reads: 65

```
@Pedrodemio So if the current goes over its rating it can be damaged? But im guessing the current would have to be continuous in order to overheat and damage?
```

---
## \#23 Posted by: Pedrodemio Posted at: 2018-08-31T01:41:34.728Z Reads: 65

```
Yeah, if I’m not mistaken the VESC still limits the current with brushed motors, so you can gradually increase it as you fell if it’s getting too hot
```

---
## \#24 Posted by: Lambjr088 Posted at: 2018-08-31T01:44:36.708Z Reads: 64

```
Awesome this was helpful now I can rebuild my wife's pocket mod hahaha
```

---
## \#25 Posted by: ricoghardforth Posted at: 2018-12-30T08:26:25.870Z Reads: 60

```
I’m trying to setup a Flipsky VESC in DC mode to run a brushed 24v 120w zy6812 motor on 6S for my sons build. He’s 9 and only weighs 20kg.   I’ve had it turning with very conservative battery/motor current values but it did’nt run very fast or with much power. Prior to this we were using a rc car esc which only allowed us to go to 4S but top out about 10mph and he wanted it to go a little bit faster.  So I thought I’d try it on 6S but couldn’t find a cheap brushed rc car esc over 4S but the flipskys on eBay are so cheap now i’d thought I’d give one a go.
So what sort of min and max motor/battery settings should I be using for this setup.  Can’t find any max or continuous current spec’s for this motor but 120w/24v is 5amp isn’t it.  The battery is made up of 3 x 2S 40C 5000mah lipos in series.  Currently I think I’ve got max motor current at 5 amps.  Do I just keep upping this until the motor starts getting warm.
```

---
## \#26 Posted by: ricoghardforth Posted at: 2019-01-04T14:14:27.871Z Reads: 45

```
I doubled the motor current up to 10Amps and the powers back to similar as it was with the RC car esc.  Motor doesn't appear to be getting to warm either.  The top speed is up from 10mph to maybe  13-14 mph at a guess so he's pleased.  It means he can keep up with me as we cruise around the estate.  I've also ordered another  HM-10 Bluetooth module we can see some live figures for speed, current and voltage.
```

---
## \#27 Posted by: ricoghardforth Posted at: 2019-03-26T13:31:08.097Z Reads: 37

```
When you use the VESC in DC mode can you use dual motors as in two motors connected in parallel to the two VESC outputs (centre output phase not connected) .   Would I need to double up the AMPS limits say if I was going from one 150W motor to two 150W motors so 300W in total.  I know you can't with brush-less motors but I have seen this in Brushed ESC RC cars before.
```

---
## \#28 Posted by: SlimSh8y Posted at: 2019-06-30T11:14:29.733Z Reads: 28

```
@ricoghardforth As far as I'm aware NO you cannot connect two motors either in series or in parallel to just one VESC. You would need anothe VESC fo add another motor. Then you can either connect the two VESC with a CAN BUS connector and run them as a master and a slave or you can split the remote receiver connection between the two VESC and use them both as masters. Doing so you will want to split your battery max amps between the two motors (you can fudge this a little for performance, just pay attention to the readings & possible faults you get in the BLDC tool and as always check for overheating or any undesirable motor activity) as your one battery will now be powering two motors, then adjust your motor max amps until you get the performance you are looking for while paying attention to heat and battery drain accordingly. The VESC do have thermal cutouts so just pay attention to the heat created then adjust your cutouts and/or motor & battery settings to prevent damage or add a few P's to your battery setup and increase your battery max amps. Hope this helps. Getcha Roll On!
```

---
## \#30 Posted by: ricoghardforth Posted at: 2019-09-13T09:06:10.288Z Reads: 10

```
We are talking about using the VESC in 2 wire DC mode for a brushed motor not using the normal 3 wire mode using a brush-less motor . There are not phases for the motors to get out of sync like there is with brush-less motors.   I'm sure you can do this with normal DC brushed ESC from the RC world the ones you use in the big crawler models.
```

---
