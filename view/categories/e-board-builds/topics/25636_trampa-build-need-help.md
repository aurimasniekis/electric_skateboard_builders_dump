# Trampa build need help

### Replies: 90 Views: 4425

## \#1 Posted by: Oozytoast Posted at: 2017-06-18T22:09:47.583Z Reads: 314

```
Hello everyone 

I have build a trampa e board with vesc's running 12s

I have been having some trouble with the bldc tool and or a motor or vesc

One motor seems to work great but the other seems to clunk and not detect the hull sensor

<img src="/uploads/db1493/original/3X/6/2/6290981afb3ff0adde1375bc92544b86263f9107.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/3/2/3239f60a66a867ef29e3a651a3a91557ce1b7414.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/d/c/dcfe44fdc77c95e02499ff77bd47b41433109735.JPG" width="666" height="500">
```

---
## \#2 Posted by: Oozytoast Posted at: 2017-06-18T22:12:28.430Z Reads: 291

```
Here is some video of the issue 


https://youtu.be/J-wxmxOZ1ZY

https://youtu.be/otboGsuxCZI
```

---
## \#3 Posted by: Oozytoast Posted at: 2017-06-18T22:17:29.208Z Reads: 279

```
Here are some tool screen shots 

<img src="/uploads/db1493/original/3X/0/8/08327750e8c6447bf661536ea497327835cdfe6a.png" width="690" height="460"><img src="/uploads/db1493/original/3X/b/3/b30b7679f519499a9456648f9025e345f5c9cc17.png" width="690" height="460">
```

---
## \#4 Posted by: JLabs Posted at: 2017-06-18T22:27:14.092Z Reads: 246

```
Did you disable PPM, apply settings, and reboot. Then measure all parameters in the FOC tab click apply and then enable PPM again and reboot one last time?
```

---
## \#5 Posted by: Oozytoast Posted at: 2017-06-18T22:58:18.748Z Reads: 243

```
I didn't have ppm disabled the first time but I just re did the (measure r and l ) followed by (measure A (req:r) followed by (calc CC) and it donsent help. It will now only spin that motor in sensorless mode when I enable hall it doesn't even spin
```

---
## \#7 Posted by: Oozytoast Posted at: 2017-06-18T23:30:37.158Z Reads: 242

```
Seems after re running all the detention steps again it works in hall mode after I brought my battery voltage up to 40v but there is still a knocking noise in the motor
```

---
## \#8 Posted by: lunasicc Posted at: 2017-06-19T00:46:16.943Z Reads: 234

```
i guess u could try swapping the motor leads over to the other esc, then you could pin point if it actually is esc related
```

---
## \#9 Posted by: Oozytoast Posted at: 2017-06-19T03:45:47.968Z Reads: 235

```
thats a good idea lunasicc I'll try that 

in the mean time here is a video showing the noise and some fun testing

https://youtu.be/8_9P9yPokzQ
```

---
## \#10 Posted by: laurnts Posted at: 2017-06-19T08:46:56.651Z Reads: 218

```
Something is wrong with the hall sensor / the vesc. The ticking sound only audible when you're riding in low speed (with hall sensor mode on). I also have quite similar issue, one of my hall sensor didn't even get detected with BLDC mode. Maybe @trampa can shed some light here.
```

---
## \#11 Posted by: Nordle Posted at: 2017-06-19T09:04:55.902Z Reads: 211

```
For that price they just could add double or triple halls-.-
```

---
## \#12 Posted by: trampa Posted at: 2017-06-19T10:14:27.886Z Reads: 211

```
You need to check if that is a mechanical issue or a motor sound.
How tight is your belt? I would say its the bearing in the spoke.
Maybe you have some play there.

Please do the following: De-tension your belt, unwind the wheel nut, take out the outer bearing, take out the bearing spacer, drop your bearing back in and carefully tighten up your wheel nut, just to the point where any play is eliminated.
You can check that by putting your board on the side and trying to push / pull the wheel up and down. 
Eliminate any Play.

Now ride again and see if the noise is still there.

Frank
```

---
## \#13 Posted by: Oozytoast Posted at: 2017-06-19T11:35:15.140Z Reads: 211

```
Thanks everyone I will dissasemble and pin point the source tonight. I also have heel straps on the way so once this knocking is gone the jumping begins <img src="/uploads/db1493/original/3X/c/a/ca830683f2db105de604137e1b26c54a9906cd9e.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/0/e/0eefd175092d144ff3e255fabf03a5d30cc90b33.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/7/8/78cb98e4dec45e9cf3773f3ec248a6636541b321.JPG" width="374" height="500">
```

---
## \#14 Posted by: trampa Posted at: 2017-06-21T07:24:51.972Z Reads: 195

```
There is another thing you should change. The motor cables need to be rerouted and fixed to the aluminium bard around the motor. This prevent that the motor cables will brake after a while. This is easy to to and will help your motor cables to stay healthy.

Frank
```

---
## \#15 Posted by: Oozytoast Posted at: 2017-06-21T16:40:31.223Z Reads: 188

```
Thanks for all the help I will do both as soon as work doesn't get in the way 

As for the price of the components I have had cheaper parts and they don't compair so far 

The quality of trampa is top notch down to every bolt
```

---
## \#16 Posted by: Oozytoast Posted at: 2017-06-26T17:50:43.945Z Reads: 184

```
So I took everything apart and fixed the spacer in place with lock tight. Not quite sure where the sound was coming from but it is gone now. 

The next step is to figure out why one motor fails the hall setup under f o c 

Then I need more torque i am cogging a lot on take off and I don't think I should at118 kv and 12s
```

---
## \#17 Posted by: trampa Posted at: 2017-06-26T17:54:16.405Z Reads: 180

```
Halls should work seamless. Did you try to ride your board reversed, motors in front, pulling.

Frank
```

---
## \#18 Posted by: Oozytoast Posted at: 2017-06-30T15:43:22.635Z Reads: 182

```
https://youtu.be/95dCdmQgo1g

This seems to be my biggest problem now
```

---
## \#19 Posted by: Oozytoast Posted at: 2017-06-30T16:21:32.081Z Reads: 174

```
I have only been trying foc should I try set it up on bdlc?
```

---
## \#20 Posted by: Oozytoast Posted at: 2017-06-30T18:02:53.239Z Reads: 186

```
https://youtu.be/xlfz1Sathr4

So I took it out foc and sensorless and now I have quite a bit of torque 

So the fact that the board runs great sensorless and fails the detect sensor tests leads me to believe I have faulty sensors of incorrect programming 

Also would the larger tires at a lower pressure work well for more traction ?
```

---
## \#21 Posted by: Oozytoast Posted at: 2017-07-01T15:21:23.897Z Reads: 178

```
https://youtu.be/TEo_GTxLA9U

Rabbit
```

---
## \#22 Posted by: Oozytoast Posted at: 2017-07-04T11:45:57.624Z Reads: 161

```
It seems like most people are not using vesc because of a lack of power 

I am also having them shut off all the time when going up hill then I loose all breaking ability 

From what I read it seems like roxxy are the preference any sujestions would be great
```

---
## \#23 Posted by: Okami Posted at: 2017-07-04T19:59:58.313Z Reads: 162

```
Not to leave empty space here, I think the leader in off road mtb builds is @ NoWind.

You probably saw the roxxys there with him too. Some other people tend to use Max6, I think and also NoWind used it on some builds.

FVT 120 12s are also available but I wont be able to tell you firsthand experience as I havent tried them and @Idea had more experience / cooperation with them in general, I think.

--

@Oozytoast does your vesc has any heatsinks or active cooling? That might also improve the situation.. it looks like your vescs are sitting in closed box anyways.. so at least some airflow would probably be welcome.
```

---
## \#24 Posted by: benwong Posted at: 2017-07-05T00:50:58.943Z Reads: 166

```
I am using FVT 12S now found out that ESC not that smooth like vesc on acceleration and braking. But this ESC can give you alot power when you need it as quite suitable on offroad usage. The power kick in is way too much for me. Unfortunely, not much offroad at here and i only riding on footpath. Too much power for me. <img src="/uploads/db1493/original/3X/3/5/359edf66a76dd1134b46b44a25a2a1282764a9ac.JPG" width="690" height="460">

And i going to try VESC tonight. Want know the feel of power output acceptable or not. If VESC work for me. I gonna sell my FVT 12S.
```

---
## \#25 Posted by: Oozytoast Posted at: 2017-07-05T02:54:39.497Z Reads: 158

```
Thanks so much everyone I think I will order some new esc' s and maybe even a direct drive from Jens 

Can't seem to find a good source for FVT s
```

---
## \#26 Posted by: Oozytoast Posted at: 2017-07-05T11:33:13.072Z Reads: 152

```
I would buy them let me know
```

---
## \#27 Posted by: trampa Posted at: 2017-07-06T08:10:17.740Z Reads: 152

```
What max amps do you have for the motor? 45 A should be set.
Do you cool your VESCs, or are they in a box without ventilation?
Maybe you have a broken sensor wire. That is easy to fix. 
Why don't you put some tape around your drives and seal off your motors. All that dirt is entering everywhere.

Frank
```

---
## \#28 Posted by: Oozytoast Posted at: 2017-07-06T12:18:17.419Z Reads: 145

```
I was running the motors and battery at 45 amps but I was lacking power so I went to 60 amps and it's been better. I will tie everything up and close things off this weekend but I would rather have a system that works well for me first. Most riders seem to agree that the vesc is just weak for off-road use.

The hall sensors might be ok and the vesc's might be bad, the motors spin nice and slow when testing
```

---
## \#29 Posted by: trampa Posted at: 2017-07-06T12:47:18.732Z Reads: 145

```
Maybe you just need two VESC SIX. I do not recommend to use hobby controllers like voltage controlled BLDC controllers.
You will have zero control over the currents in your system and no safety features like temperature sensing.

Frank
```

---
## \#33 Posted by: Oozytoast Posted at: 2017-07-09T01:29:52.602Z Reads: 138

```
https://youtu.be/X_uI1iSgBu4

This video shows the cogging I face when starting on a hill
```

---
## \#34 Posted by: Oozytoast Posted at: 2017-07-09T01:31:24.853Z Reads: 139

```
https://youtu.be/yoT4SsPcifU

This video shows the cut off that happens when I loose traction 

I will post my vesc settings soon
```

---
## \#35 Posted by: Oozytoast Posted at: 2017-07-09T13:44:30.921Z Reads: 134

```
The more max motor amps and battery amps as well as start up boost I give it the better it performs. I currently have 60 max battery and motor and 0.09 boost. Think I can go higher ?
```

---
## \#36 Posted by: Oozytoast Posted at: 2017-07-09T13:46:27.408Z Reads: 130

```
I plan to get the vesc 6 or touque boards 12s escs since my sensors seem done for
```

---
## \#37 Posted by: Oozytoast Posted at: 2017-07-09T17:34:13.552Z Reads: 123

```
Here goes nothing based on my batteries 5 amp x 25c rating they should handle 125 amp max draw (at least that's how I understand it)
```

---
## \#38 Posted by: Okami Posted at: 2017-07-09T17:41:15.565Z Reads: 129

```
The cogging up hill looks really bad, I would have stopped there already midway and end the suffering hah..

Though.. i dont really know how to help you, all I can imagine is, that sensored mode does not work properly and as Im no Vesc expert i wont be able to help.. All I can see is that u should post your question in vesc related thread? or just write a few people personally, who you think would be able to give you a good advice.

I somehow think vescs should be able to work somewhat okay, there are users who use them without problems, for example, check @Duffman mbs build
```

---
## \#39 Posted by: trampa Posted at: 2017-07-09T18:13:03.785Z Reads: 132

```
Since the sensors seam to work, when setting them up, it seams like your VESCs have an issue. The motors should start to spin up perfectly sweet, no matter of the load. We do not have to tweak any settings to get perfect startup.
If you like I can put you on the beta program and you can try VESC-Tool and FW 3.26 for your HW 4.12 version.

Frank
```

---
## \#40 Posted by: Oozytoast Posted at: 2017-07-10T03:27:59.220Z Reads: 131

```
https://youtu.be/OrP2VFPDrvA

That would be awesome Frank I zip tied the motor wires like you said and I am planning a better inclosure with vents. I had a bad anti spark plug and I think that may have fried the vesc sensors. For now I'm running 70 amps motor battery max and the cogging is almost gone. There are still cut off issues when the wheels slip but this is getting real fun
```

---
## \#41 Posted by: benwong Posted at: 2017-07-10T07:35:33.211Z Reads: 124

```
Good to hear that cogging is solve while putting more amps value on motor max. I am still wondering want go for VESC or not since i just flash another firmware and feel the power kick in is controlable. Did you connect two VESC with canbus or y splitter?
```

---
## \#42 Posted by: Oozytoast Posted at: 2017-07-10T12:29:19.036Z Reads: 122

```
I am using can bus to connect the two vesc's 
I would not say my problems are solved I still have cogging while starting on steep hills and now the bigger problem is the cutoff 

As soon as my wheels loose traction and slip the system shuts down for 5 seconds I loose forward and breaks. This is bad because it usually happens while I'm going up a hill then I roll backwards down the hill with no breaks.
```

---
## \#43 Posted by: trampa Posted at: 2017-07-10T21:11:38.480Z Reads: 124

```
I'm sure we will get that sorted very soon. Some software magic will help.

Frank
```

---
## \#44 Posted by: Oozytoast Posted at: 2017-07-12T00:10:29.908Z Reads: 120

```
Tonight I will update to the new vesc software and reduce my amps back down to the recommended 50 After frank advised me to drop it I looked into it and the motor seems rated for 2500 watts so 50 amps x 44 volts puts me at 2200 watts. If I understand it correctly 

Thanks again Frank
```

---
## \#45 Posted by: rich Posted at: 2017-07-14T09:59:14.733Z Reads: 115

```
Hey Oozytoast,
did the software solve your problems?
The last days i saw this thread and felt bad for you.
Yesterday i had my first ride with my 136kv motors and i can't believe i'm having exactly the same problems! The knocking (with loose belt) i'll try to fix like frank told you.
The cogging is a desaster, it's not possible to start from a dead stop, only with no load or sometimes on flat concrete, on any other terrain there is no power and i feel helpless :sob:
[quote="trampa, post:39, topic:25636"]
The motors should start to spin up perfectly sweet, no matter of the load. We do not have to tweak any settings to get perfect startup.
[/quote]

Well...... that's what i want.
I'll try it with other vescs to know if the vescs or the motors are the problem, also i'll try unsensored mode to see if there's a difference in performance (right now it feels unsensored in hybrid mode)
```

---
## \#46 Posted by: trampa Posted at: 2017-07-14T11:29:43.099Z Reads: 114

```
To did down to the problem, i need to know your ESC manufacturer and the FW you use.

Frank
```

---
## \#47 Posted by: rich Posted at: 2017-07-14T11:40:45.927Z Reads: 114

```
My vescs 4.12 are from scramboards, i think the manufacturer is flier (with heatsinks). I use FW 2.54 by Ackmaniac with motor max 40A each.
But also both vesc's temp sensors are faulty, maybe they have problems with hall sensors, too.
I'll test it with maytech vescs (shame on me) the next days, too and let you know.
Thanks @trampa!
```

---
## \#48 Posted by: Oozytoast Posted at: 2017-07-14T12:16:22.689Z Reads: 122

```
I will have an answer tonight work has gotten in the way again. But with all that work I ordered these 

http://www.electric-skateboard.builders/t/motormounts-for-trampa-mtb-e-toxx-dual-direct-drive/18992/12
```

---
## \#49 Posted by: rich Posted at: 2017-07-17T12:39:49.701Z Reads: 127

```
[quote="Oozytoast, post:1, topic:25636"]
One motor seems to work great but the other seems to clunk and not detect the hull sensor
[/quote]

I think i know what's the problem!
Yesterday i tested different vescs and motors and realized that 3 of my 4 vescs have broken hall sensor ports, i'm so upset! Since there is no warranty i could have bought 2 VESC SIX for this money!!!
I have 1 working vesc for 4 sensored motors on 2 builds now :rage:

To check that do motor detection again (i also thought the sensors are working first).
When your sensor port is good it looks like this:

<img src="/uploads/db1493/original/3X/9/a/9a9db5e037cc34c2c2b9fa5b9b68e5b9ffded5f1.jpg" width="690" height="388">

If the sensor ports are bad you get this: 

<img src="/uploads/db1493/original/3X/5/b/5b16ea8abc66d0c5e5d3e69f58d68c5f56e7b6a6.jpg" width="690" height="388">


So @trampa if people (like me) claim the motor sensors it's 100% the motor contoller or bad extension cables.
Unfortunately i have no idea how i could afford 4 VESC SIX :disappointed_relieved:

The trampa motors a really great and strong. i was riding a steep path uphill (which i can't ride with my mountainbike, too steep) with no problems (of course with catching some speed before climbing).
Also the brake force is very powerful!
I love this motors but there's one thing i don't like: The keyway, the key and the pulley are not one unity, the pulley has play in both directions and the grub screw is on the rounded side of the shaft. I put a lot of thread locker on the grub screw but after 20km one pulley is loose now.

I have different motors where keyway, key and pulley fit 100% with no play, also the grubscrew is on top of the key (so it's like a flatspot). These pulleys came loose after 6 weeks daily riding WITHOUT thread locker. After putting thread locker it never ever came loose again.

The only solution for trampa motors i think is to dremel a flatspot like people do on SK3's motors, but i don't like to do that, i have to check if my other pulleys fit better.
```

---
## \#50 Posted by: JohnnyMeduse Posted at: 2017-07-17T12:55:43.293Z Reads: 109

```
Could you post a picture of your connection on the vesc and of the vesc....
```

---
## \#51 Posted by: trampa Posted at: 2017-07-17T13:26:31.851Z Reads: 108

```
Sorry to hear your Maytech ones are broken. One hall sensor per board usually does the trick.
I do lock down my pulleys with blue lock anyway. So I don't face the same issues. Some heat will let you disassemble the pulley again.

Frank
```

---
## \#52 Posted by: Blasto Posted at: 2017-07-17T13:34:31.589Z Reads: 117

```
[quote="rich, post:49, topic:25636"]
Yesterday i tested different vescs and motors and realized that 3 of my 4 vescs have broken hall sensor ports
[/quote]

When testing your vescs, flip the phases to make the motor go in the other direction.

I highly dought it's the vesc sensor port is the source of your problem. Check those adapters carefully
```

---
## \#53 Posted by: JLabs Posted at: 2017-07-17T14:11:52.307Z Reads: 116

```
I'm not sure if someone mention this all ready but expanding on what @Blasto said...

Some motor's sensors only work with one combination of phase wires, so if the phase wires are not plugged in the correct order sensor detection will fail. I had this happen with my motors in the past but have sense corrected the issue.
```

---
## \#54 Posted by: rich Posted at: 2017-07-17T15:14:51.887Z Reads: 122

```
[quote="JohnnyMeduse, post:50, topic:25636, full:true"]
Could you post a picture of your connection on the vesc and of the vesc
[/quote]

Have to work the next 8 hours...... i'll post pictures tomorrow. There you'll also see details why Maytech vescs are dangerous.

But i've tried different connections. With short phase wires (10 cm), with long (80 cm which i use on mtb). Also sensor cable was directly plugged to vesc, once with 30cm extension and once with 80 cm 22AWG (which i use). One vesc is detecting the hall sensors no matter which sensor cable or phase wire, i tested them all. The other 3 vescs fail......


[quote="trampa, post:51, topic:25636"]
One hall sensor per board usually does the trick.
[/quote]

Really? I have to test it. So the hall sensor on master controller and disabled traction control?
The slave in hybrid mode like the master?
That would be awesome......

[quote="Blasto, post:52, topic:25636"]
When testing your vescs, flip the phases to make the motor go in the other direction.
[/quote]

I have tried all possible variations of phase wire combinations but always the detection fails on 3 of 4 vescs 4.12.......

[quote="JLabs, post:53, topic:25636"]
Some motor's sensors only work with one combination of phase wires
[/quote]

I think that's not my case but it would be interesting how you handle it when the motor goes the wrong direction if the hall sensors are only working this way? Riding reverse? :joy: 

Thanks to all of you for your feedback!
```

---
## \#55 Posted by: rich Posted at: 2017-07-18T14:41:28.843Z Reads: 118

```
Here some pics of one maytech 4.12 with broken sensor port. Maybe you can see what's wrong with it.

<img src="/uploads/db1493/original/3X/d/6/d66809b2ac13a934695162577fbc88da8461801b.jpg" width="690" height="388">

<img src="/uploads/db1493/original/3X/e/7/e738b5eb52e790d6c97600b5d28db6a5d0d88aee.jpg" width="690" height="388">

Here you see the JST legs are not cut.
@Martinsp  mentioned that he short his vesc because the legs pierced through the plus lead.

<img src="/uploads/db1493/original/3X/4/2/42b27a3fff541e48ee39a225815332d17bb14ad5.jpg" width="690" height="388">
```

---
## \#56 Posted by: JohnnyMeduse Posted at: 2017-07-18T14:58:30.033Z Reads: 114

```
[quote="rich, post:55, topic:25636"]
Here you see the JST legs are not cut.
[/quote]

The damage cause by percing the power will be much more destructive than just affecting the sensor, it would kill the vesc instantly.

Also it look like from the picture that you might have a cold solder joint over the ground pin 

<img src="/uploads/db1493/original/3X/2/a/2aa0511bf4fd525df53be7ebf3b81688d9233170.JPG" width="690" height="388">
```

---
## \#57 Posted by: rich Posted at: 2017-07-18T16:13:09.539Z Reads: 112

```
[quote="JohnnyMeduse, post:56, topic:25636"]
Also it look like from the picture that you might have a cold solder joint over the ground pin
[/quote]

Wow, thanks to your eagle eyes!!!! :eyeglasses: That could be the reason, i'll resolder the GND and test it again.
```

---
## \#58 Posted by: Martinsp Posted at: 2017-07-18T17:02:29.120Z Reads: 108

```
Yup I killed my Maytech VESC that way :D not fun :smiley:
**Also be sure to update your firmware to the newest one and BLDC-tool because i would not be surpirised if maytech did not use the latest firmware... there is a bug that multiplies the max current ramp step by 10 every time you write and read config... the correct value should be 0.04** Maybe they use the nevest firmware, maybe not.. worth checking, there have been some folks with this bug recently. :)
I might have blown my second VESC that way :D I think so because I took care of the hardware faults or whatever prior to turning it on...
```

---
## \#59 Posted by: trampa Posted at: 2017-07-18T21:01:05.063Z Reads: 107

```
I dropped @rich  on Beta. So he can use FW 3.26.
The missing Bootloader can be updated via VESC-Tool. I hope you will get the sensors working.


Frank
```

---
## \#60 Posted by: Silverline Posted at: 2017-07-18T21:19:46.030Z Reads: 103

```
So you are saying that people with maytech vesc without bootloader , can flash bootloader and all the other stuff with the new upcomming vesc GUI ?

Btw. How Long does it take before you guys ships a urban carver board 😇 looking forward to receive mine.
```

---
## \#61 Posted by: trampa Posted at: 2017-07-18T21:22:44.445Z Reads: 107

```
Yes, Vesc-Tool can ad the missing boot loader via usb. Easy...

I'll check for the delivery of the missing parts for the Urban carver.

Frank
```

---
## \#62 Posted by: Silverline Posted at: 2017-07-18T21:24:08.431Z Reads: 109

```
Cool, so no need for ftdi adapter any more. 

Regarding the board, cool thanks 😎 No Rush, just asking.
```

---
## \#63 Posted by: trampa Posted at: 2017-07-18T21:26:38.168Z Reads: 105

```
No need anymore. This tweak only works if no bootloader is installed.
```

---
## \#64 Posted by: rich Posted at: 2017-07-19T09:43:29.762Z Reads: 108

```
@JohnnyMeduse you are my hero!!!!!!!!
After resoldering the sensor port is working now :grin:

My other two  4.12 controller with broken temp sensors and sensor ports i gonna replace with 2 PCB's from @esk8 i ordered last night, i trust them.

@Martinsp well it's FW 2.18 (the latest). I clicked read configuration, my max current ramp was 4.00 instead of 0.04 :astonished:

@trampa can't wait to go sensored this weekend!
Also you probably saved my vescs with the use of FW 3.26, downloaded VESC-TOOL GOLD last night...... Thanks!
```

---
## \#65 Posted by: Martinsp Posted at: 2017-07-19T10:19:49.608Z Reads: 102

```
If it works you might be lucky... The ramp step error destroys DRVs
```

---
## \#66 Posted by: rich Posted at: 2017-07-19T10:35:34.282Z Reads: 102

```
@Martinsp  I won't try it! I'll switch to FW 3.26 this week
```

---
## \#67 Posted by: Martinsp Posted at: 2017-07-19T10:42:15.751Z Reads: 106

```
@rich No absolutely don't try it. I meant it that you got lucky and the high current ramp step did not destroy your vesc before you noticed that.
```

---
## \#68 Posted by: Oozytoast Posted at: 2017-07-19T10:54:29.458Z Reads: 109

```
https://youtu.be/SDcAKQDSkjc

My vesc's are all back working sensorless but the hall detection still fails with the latest software :(
```

---
## \#69 Posted by: rich Posted at: 2017-07-19T11:42:11.195Z Reads: 105

```
@Oozytoast do you see the detected hall sensor table when doing motordetection (not FOC)? Could be you have also cold solder joints somewhere.

Great you ordered spur gears from @nowind ! Did you ordered short shafts somewhere in case you use the spur gears with your trampa motors?
```

---
## \#70 Posted by: rich Posted at: 2017-07-19T13:06:23.047Z Reads: 98

```
I've never used them, only bench test.... :wink:
```

---
## \#71 Posted by: Martinsp Posted at: 2017-07-19T16:38:53.605Z Reads: 96

```
That is probably the reason it didn't break... I believe that is how I killed my Maytech VESC...
```

---
## \#72 Posted by: Oozytoast Posted at: 2017-07-19T16:57:10.535Z Reads: 96

```
I was thinking I would just cut the shafts and I will try bldc mode thanks
```

---
## \#73 Posted by: rich Posted at: 2017-07-19T17:09:34.828Z Reads: 93

```
I think you'll miss a lot of fun without sensors no matter if belts or spur gears!
When i experienced the difference i can tell you more....
```

---
## \#74 Posted by: Oozytoast Posted at: 2017-07-19T18:13:35.382Z Reads: 89

```
Yeah I just need a way to tell if it's the motors or the vesc that's the problem
```

---
## \#75 Posted by: rich Posted at: 2017-07-19T18:21:30.495Z Reads: 95

```
I'm sure it's the vesc... which manufacture or shop you get it?
I have 4 cheap vescs and as i wrote only one sensor port worked (now 2 :smile:)

I will never ever buy cheap.....
```

---
## \#76 Posted by: Oozytoast Posted at: 2017-07-19T18:33:16.054Z Reads: 96

```
Diy electric skateboards / tourqe boards I think
```

---
## \#77 Posted by: Oozytoast Posted at: 2017-07-20T02:01:32.815Z Reads: 95

```
Just went for a ride on the board after setting up the foc mode and the cogging is bad on grass hills, next I will try bldc mode. I would really like to know if there is a way to test the hall sensors before I spend 800$ on new vesc's
```

---
## \#78 Posted by: rich Posted at: 2017-07-20T07:13:08.028Z Reads: 96

```
[quote="Oozytoast, post:77, topic:25636"]
I would really like to know if there is a way to test the hall sensors
[/quote]


Again, as i said do motor detection in BLDC and see if the text is:

HALL SENSOR DETECTION FAILED
OR
DETECTED HALL SENSOR TABLE

below Integrator limit and BEMF Coupling.

If one vesc detects the hall sensor and the other vesc doesn't, take the motor from the "bad" vesc and connect it to the "good" one and start motor detection again.
Then you should know if both hall sensors are working and if you have one bad vesc.

In my case it was just one single cold solder joint on the sensor port of the vesc which is not visible with the eyes, even on the close picture i couldn't see it. You need experts like @JohnnyMeduse who can save your life (and vesc)!

I'm sure you can talk to @torqueboards in case of a faulty vesc but try motor detection first.
```

---
## \#79 Posted by: Oozytoast Posted at: 2017-07-21T00:40:10.591Z Reads: 94

```
<img src="/uploads/db1493/original/3X/4/a/4a9ad2d0b660dc1516c232c2810ba695abb06d99.JPG" width="374" height="500">

Still fails on bldc 

I ordered vesc 6 s I sure hope they are as good as people think they will be
```

---
## \#80 Posted by: rich Posted at: 2017-07-21T00:46:21.845Z Reads: 92

```
Bad! The same results on both vescs?

Anyway vesc 6 is the best option!
```

---
## \#81 Posted by: Oozytoast Posted at: 2017-07-24T02:25:31.821Z Reads: 87

```
It is the same on both

So I just switched to bldc mode with the startup boost to 0.09 and it's much better performance 

No more cutoff happening 

It's much noisier of course
```

---
## \#82 Posted by: rich Posted at: 2017-08-07T20:39:44.490Z Reads: 79

```
Hey, does your system work now? Mine works so fine now, take a look:

https://www.electric-skateboard.builders/t/sensored-motors-cogging-and-jittering-whats-wrong/29245/62?u=rich
```

---
## \#83 Posted by: Oozytoast Posted at: 2017-08-20T18:49:09.243Z Reads: 81

```
https://youtu.be/jYZel_hfpH8

Got all my new components but my vesc6 doesn't seem to update any ideas @Nowind @trampa
```

---
## \#84 Posted by: Oozytoast Posted at: 2017-08-20T18:51:24.484Z Reads: 85

```
<img src="/uploads/db1493/original/3X/9/d/9dbf08aaf344b5f8287437f103a778c3e9626f63.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/5/8/5817bd7b694e6cebb366119ad604b23731dd732a.JPG" width="375" height="500">
```

---
## \#85 Posted by: trampa Posted at: 2017-08-20T20:17:38.091Z Reads: 83

```
Did you upload the bootloader? Read the sticky threads on the vesc-project forum.

Frank
```

---
## \#86 Posted by: Oozytoast Posted at: 2017-08-20T21:06:26.223Z Reads: 83

```
https://youtu.be/aZVrBeEXdgM

Thanks frank I got the boot loader installed and firmware updated. Now one of the motors detects the hall sensor and works great but the second motor or vesc fails hall detection. Any ideas ?
```

---
## \#87 Posted by: rich Posted at: 2017-08-21T00:30:45.900Z Reads: 83

```
[quote="Oozytoast, post:86, topic:25636"]
the second motor or vesc fails hall detection. Any ideas ?
[/quote]
change phase wire combination, if the motor spins in the wrong direction but detect the sensor you can click "Invert motor direction" in VESC-Tool (I think it's called like this or similar). I had this with one trampa motor.
```

---
## \#88 Posted by: Oozytoast Posted at: 2017-08-21T01:07:37.893Z Reads: 80

```
Thanks for the suggestion but I switched two phase wires and it still failed twice
```

---
## \#89 Posted by: rich Posted at: 2017-08-21T01:26:52.684Z Reads: 79

```
There are 6 possible phase wire combinations :wink:
If you find a way it works I would do detection again without belts (I know many screws...).
The wobble of your pulley (or hub) in the video above looks really bad! Are all screws tightened? You should fix that.
```

---
## \#90 Posted by: ripcurldog Posted at: 2018-06-20T10:24:14.517Z Reads: 51

```
Hi, I am having the same issue with my Trampa motors. The Keyway clicks and the grub screw always comes loose.  Nothing works (glue, loctite, etc.). The only option I have left is to grind the motor shafts to a flat spot,but I really don't want to do that.  Did you end up doing that to your Trampa motors?
```

---
## \#91 Posted by: rich Posted at: 2018-06-20T11:05:49.940Z Reads: 49

```
On my Trampa motors I put thread locker on the shaft and key, too. It holds but you'll need heat to remove it (e.g. blow torch). I would modify the key as I described in your thread. No clicking = no problem.
```

---
## \#92 Posted by: ripcurldog Posted at: 2018-06-20T12:00:11.685Z Reads: 51

```
Thanks Rich.  Yes, I am in Singapore on a work trip at the moment, but when I get home, I plan to implement your changes. I guess I will try those and if the problem persists, my last option will be to dremel the shaft down.
```

---
## \#93 Posted by: Eboosted Posted at: 2018-06-22T04:18:59.574Z Reads: 43

```
@ripcurldog use Loctite 680 don't ever use grub screws and keyways again. To remove them use this approach

https://youtu.be/9b09jZt9_Zc
```

---
## \#94 Posted by: jaredching Posted at: 2018-06-24T14:48:16.951Z Reads: 29

```
Hi Trampa, desperately need help with the Urban Carver electric set up. I've got to the point where I have connected the VESC with the motor, but it will not sense it properly - I have tried adjusting the parameters I, D and W, I have also set D to 0 as I have seen a previous post on ESk
```

---
