# &#124; 37&rdquo; Arbor Deck &#124; Caliber II Trucks&#124; Single R-Spec 190kv Motor &#124; Enertion mount &#124; Space Cell &#124; Vesc &#124; 2.4 Receiver &#124;

### Replies: 30 Views: 3982

## \#1 Posted by: Fababuba Posted at: 2015-12-26T00:18:41.744Z Reads: 192

```
Hi, I've been scrolling through the forum for awhile now and I finally got my parts in the mail yesterday. I am half way done but I am not sure how to connect my receiver to the Vesc(I dont think I have all the wires...) <img src="/uploads/db1493/original/2X/b/baa5fd34c34f10168d5031c2d253863d96246649.jpg" width="689" height="390">   
This is all I have, can someone tell me what wire I need and where it goes. Thanks! 

Also I got my Vesc from enertion, does anyone know if the are programmed to work with the R-Spec motors? or do I have to do it myself? 

I'm pretty sure I know what I am doing, just not confident that everything isn't going to blow up lol.
```

---
## \#2 Posted by: lowGuido Posted at: 2015-12-26T00:26:39.657Z Reads: 185

```
if you got the VESC from enertion then it should be pre programmed fro the R-spec.
as for the reciever you need a servo cable to connect it to the 3 pins sticking out of the lower left corner of the VESC.
<img src='/uploads/db1493/original/2X/4/49377e00c46084f3105b9b1f90f8e445584d1aba.gif'>
```

---
## \#3 Posted by: kai Posted at: 2015-12-26T00:27:47.414Z Reads: 175

```
You plug the connector into receiver and the three prongs sticking out toward the capacitor on the vesc.
```

---
## \#4 Posted by: Fababuba Posted at: 2015-12-26T00:35:52.043Z Reads: 174

```
The servo cable is male to male right?
```

---
## \#5 Posted by: lowGuido Posted at: 2015-12-26T00:38:08.573Z Reads: 171

```
its female to female the way I see it.
```

---
## \#6 Posted by: chaka Posted at: 2015-12-26T03:36:56.641Z Reads: 170

```
Servo wires refer to the casing instead of the actual connection pins and sockets. The casing is male so they are referred to as male even though the physical connector is a female type.
```

---
## \#7 Posted by: lowGuido Posted at: 2015-12-26T03:42:41.742Z Reads: 166

```
well that's confusing.
```

---
## \#8 Posted by: chaka Posted at: 2015-12-26T03:48:49.974Z Reads: 171

```
This should clear things up a little. 
<img src='/uploads/db1493/original/2X/5/5d3795f6b2b9b94bcb7118994bf61a5f2f5fd9ec.jpg'>
```

---
## \#9 Posted by: lowGuido Posted at: 2015-12-26T03:56:50.777Z Reads: 157

```
regardless of what they call it, I still see the pins as male and the holes as female.
I'm old school like that.
```

---
## \#10 Posted by: chaka Posted at: 2015-12-26T03:58:19.636Z Reads: 158

```
You are correct. I see it that way too but you will have a hard time searching google for it otherwise.
```

---
## \#11 Posted by: lowGuido Posted at: 2015-12-26T04:03:06.652Z Reads: 165

```
[quote="chaka, post:10, topic:807"]
You are correct.
[/quote]

well as it turns out, I'm incorrect.

but I'm happy to continue to be wrong on this one.
```

---
## \#12 Posted by: kai Posted at: 2015-12-26T08:03:32.047Z Reads: 156

```
i feel that way too. On the bigger end one on the pic has the male end ( female to me) under the extra black housing over it on the one i got. Cut it off and snapped the pins inside and it looks just like the other end.
```

---
## \#13 Posted by: NIK Posted at: 2015-12-26T10:46:31.920Z Reads: 158

```
Dont forget to bind your receiver bruv. Youtube got tons of that. I don't know what others opinion on binding, but my receiver without binding, is a bit different using the throttle. Normally, you can push the stick down or up to de/accelerate, but my experience without binding makes it de/accelerate using the direction wheel (circle knob). kinda weird but its okay now after binding. Basic RC.
```

---
## \#14 Posted by: sgaana Posted at: 2015-12-26T19:13:48.783Z Reads: 158

```
@NIK What do you mean by binding the receiver ?
```

---
## \#15 Posted by: Fababuba Posted at: 2015-12-30T20:43:35.490Z Reads: 160

```
<img src="/uploads/db1493/original/2X/a/af5f6feebdda6821aa847d2ae912736139970d2b.jpg" width="689" height="390">

Alright I got the servo cable and by following various tutorials online I tried binding my receiver to the transmitter, but it doesn't work. The light on the receiver refuses to bind and doesn't stop flashing, I'm at a loss can anyone tell me what I'm doing wrong?
```

---
## \#16 Posted by: NIK Posted at: 2015-12-30T21:24:51.137Z Reads: 155

```
Before u turn on the radio controller, did u push the pair/bind button at the transmitter and then u turn it on?. Or do u turn it on first and then press pair/bind?
```

---
## \#17 Posted by: Fababuba Posted at: 2015-12-30T21:34:05.775Z Reads: 152

```
I turned it on first then hit the pair button on the transmitter, I'll try both ways a couple times more though.
```

---
## \#18 Posted by: NIK Posted at: 2015-12-30T21:34:25.063Z Reads: 154

```
Sorry @sgaana . I didn't see your reply. Try searching on youtube of the how to bind RC controller. Short video can make u go long way. Btw @Fababuba , center the white ST.TRIM and TH.TRIM (the white round knob) on your transmitter before u turn it on. Lemme make it clear:

 1. Turn OFF everything
 2. Turn ON the SPACE CELL, and I assume it is well connected
 3. Put your BIND jumper key/wire on the BIND Channel and it will blink
 4. Push the PAIR/BIND button on the remote control while it is turn OFF
 5. Turn ON the remote controller

I did mine same as the steps and I use the same remote controller as yours. Almost as sleek as nunchuck. haha
```

---
## \#19 Posted by: Fababuba Posted at: 2015-12-30T21:38:06.944Z Reads: 147

```
You're a legend, it worked! Thanks I didn't realize that you had to press and hold the pair button before turning on the controller.
```

---
## \#20 Posted by: NIK Posted at: 2015-12-30T21:41:16.159Z Reads: 146

```
Glad I could help. WE E.SK8 BUILDERS ARE LEGEND. lel Have fun enjoy your ride.
```

---
## \#21 Posted by: Fababuba Posted at: 2015-12-31T05:45:30.939Z Reads: 151

```
So I got everything to work, motors spinning and responsive breaking but then decided to configure my VESC for the space cell and motor because I wasn't sure if the VESC was optimized. I got bldc tool 2.5 and updated my firmware to 2.7 from 1.14 and changed the current limits settings to optimize it for the space cell. Now its no longer responsive to my controller and the motors don't spin. I'm not sure whats wrong at all.. I tried reloading the firmware to the VESC and loaded the xml file that onloop posted for the r-spec motors.

Also is there a difference in the firmware that you load? I know the file is named default.bin but each folder has its own default.bin file. I currently have the default.bin from hw_410_411 loaded.
<img src="/uploads/db1493/original/2X/0/0b8464fd030e334d207b12ee99410b415a2e2c6e.jpg" width="689" height="390">
```

---
## \#22 Posted by: EnertionSupport Posted at: 2015-12-31T06:15:41.347Z Reads: 132

```
[quote="Fababuba, post:1, topic:807"]
Also I got my Vesc from enertion, does anyone know if the are programmed to work with the R-Spec motors? or do I have to do it myself?
[/quote]

If you have 6355 R-SPEC motors the vesc is programmed & ready to go! if you want to change the parameters, such as fine tuning the PPM settings for your radio transmitter, please use this version of BLDC tool. https://drive.google.com/file/d/0B4M52aF7FaMWM2lsalBNbjlWNWM/view?usp=sharing
```

---
## \#23 Posted by: Fababuba Posted at: 2015-12-31T06:23:21.409Z Reads: 134

```
@EnertionSupport Thanks, but I already update my firmware this morning and I now my motor won't respond to my inputs, can you help me out?    

This was in my earlier post

So I got everything to work, motors spinning and responsive breaking but then decided to configure my VESC for the space cell and motor because I wasn't sure if the VESC was optimized. I got bldc tool 2.5 and updated my firmware to 2.7 from 1.14 and changed the current limits settings to optimize it for the space cell. Now its no longer responsive to my controller and the motors don't spin. I'm not sure whats wrong at all.. I tried reloading the firmware to the VESC and loaded the xml file that onloop posted for the r-spec motors.

Also is there a difference in the firmware that you load? I know the file is named default.bin but each folder has its own default.bin file. I currently have the default.bin from hw_410_411 loaded.

IMAG0304.jpg2688x1520 2.4 MB
```

---
## \#24 Posted by: EnertionSupport Posted at: 2015-12-31T06:34:39.848Z Reads: 131

```
WARNING: If firmware is incorrectly installed you can damage the hardware.

**Make sure you have the correct app selected.** 
Go to: "App Configuration" Tab 
In "General" Tab (choose PPM) 
Click "PPM" Tab (choose "current no reverse with brake")

[Also be sure to read all of the VESC FAQ's][1] 


  [1]: http://www.electric-skateboard.builders/search?q=vesc%20faq
```

---
## \#25 Posted by: Fababuba Posted at: 2015-12-31T07:08:35.079Z Reads: 128

```
@EnertionSupport 
Is there a way to check if I incorrectly installed my firmware? Will the VESC show any specific symptoms? The BDLC tool recognizes firmware 2.7 and reads all of its settings, both leds are also functional on the VESC.   
Or is there still a possibility that updating the firmware broke the VESC?
```

---
## \#26 Posted by: EnertionSupport Posted at: 2015-12-31T07:17:10.826Z Reads: 129

```
If there are no obvious hardware faults, if everything seems normal it probably is, so your problem is probably due to some settings being incorrect. You would need to screen capture all the BLDC pages for me to know if your settings are wrong.
```

---
## \#27 Posted by: Fababuba Posted at: 2015-12-31T07:33:16.362Z Reads: 136

```
@EnertionSupport<img src="/uploads/db1493/original/2X/1/15052fb0b6d6a48996bc9eefcb1651182566e69c.PNG" width="690" height="368"> <img src="/uploads/db1493/original/2X/4/4d291f6dcec941ccee3144fdc8f1917cf224fdb0.PNG" width="690" height="368">
<img src="/uploads/db1493/original/2X/e/e26797359c3dad38481dcc04e0ab7dde26ead63e.PNG" width="690" height="367"><img src="/uploads/db1493/original/2X/2/25573fe1ef7961936d0b31cad3f31f9054666a1c.PNG" width="690" height="369"><img src="/uploads/db1493/original/2X/d/d2b3796ce4e766171d8eff69060bc83c028ce3da.PNG" width="690" height="368"><img src="/uploads/db1493/original/2X/0/09c62f26ec16686ec11ab7b1699ffacba71ca9c5.PNG" width="690" height="368"><img src="/uploads/db1493/original/2X/d/d516b187d5c9cfcc0af843c91c028fb70658af20.PNG" width="690" height="368">
<img src="/uploads/db1493/original/2X/d/d61e611aeaa66c26fa00d375086f8d7612c7687f.PNG" width="690" height="368">
Thanks I really appreciate your help.
```

---
## \#28 Posted by: EnertionSupport Posted at: 2015-12-31T15:12:51.160Z Reads: 128

```
Thank you for the screen captures!

have you tried getting your motor to spin with the detection tool? Using the detection will give you nearly the same numbers as the XML file for the R-SPEC motors. The difference is that the motor will spin up in the process, would should help us to pinpoint the problem. 

If the detection is successful, than you can confirm the VESC is able to spin the motor, and then it is just down to finding any settings that could be conflicting. 

While the detection is going, see if there are any faults in the "realtime data" section. The fault code can be seen in the bottom left of that page. You can see some examples of troubleshooting a VESC with the realtime data in this thread: 

http://www.electric-skateboard.builders/t/vesc-blew-up-any-ideas-edit-solved/201/17

If the detection is unsuccessful, hopefully the fault code will give you a clue as to what went wrong. 


----------
As for the PPM, have you turned on the "PPM display" (located at the bottom of the PPM tab) to see if the VESC is at least reading your inputs? after turning your PPM to "disabled", check that little box and see if the bar moves with throttle/brake inputs from your remote. 

Hopefully this will help us get one step further to having your VESC up and running.
```

---
## \#29 Posted by: Fababuba Posted at: 2015-12-31T16:45:43.403Z Reads: 122

```
@EnertionSupport
I got it to work! I'm not actually sure what fixed it but it started working after I changed the some of the ppm settings.
```

---
## \#30 Posted by: EnertionSupport Posted at: 2015-12-31T17:09:55.075Z Reads: 122

```
awesome, glad to here you are up and running again.
```

---
