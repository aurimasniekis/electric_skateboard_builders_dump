# Help with DIY electric longboard setup?

### Replies: 63 Views: 3278

## \#1 Posted by: nikoli280 Posted at: 2017-05-19T22:15:48.061Z Reads: 164

```
Hi im a bit confused right now and i hope your can help me.

I will be making a electric longboard with a around 450Wh Litihum Ion pack 18650. I know how to make the pack and is using a spot welder and some 1.5mm thick solid copper wire.

My dilemma is what configuration can work.


Nr. 1  a 6S configuration with 

LG 2500mah 18650 H4 battery x50
BMS 60A - https://www.aliexpress.com/item/6s-24v- ... d4e70e8d45

Motor 90A 380Kv. - https://hobbyking.com/en_us/ntm-prop-dr ... 65w-1.html

100A ESC - https://hobbyking.com/en_us/hobbyking-1 ... -ubec.html

Transmission - http://www.ebay.co.uk/itm/Electric-Skat ... 1305941096?



Nr. 2  Is the same as nr.1 but with this ESC 
https://hobbyking.com/en_us/turnigy-trackstar-1-5th-scale-sensorless-200amp-8s-opto-car-esc.html
I talked to hobbyking support, and they said it was the only one i would use, since braking would harm the motor with regular ESC, And startup would be with pushing. 


Nr. 3 which is the most expensive consists of a 10S configuration.

Motor - https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6354-260kv-brushless-outrunner-motor.html

VESC - https://www.aliexpress.com/item/Maytech-Benjamin-Vedder-Electronic-Speed-controller-VESC-for-electric-longboard-DIY-skateboard/32712595711.html?spm=2114.13010208.99999999.276.vC2rQk

LG 2500mah 18650 H4 battery x50

BMS https://www.aliexpress.com/item/10S-60A-version-D-lipo-lithium-Polymer-BMS-PCM-PCB-battery-protection-board-for-10-Packs/32732403488.html?spm=2114.13010208.99999999.269.ESMXUb



I think nr 3 is the best but im not sure. Im looking forward to your repies and help. i will be using the board for traveling on road and with max speed of 30-35 km/H
```

---
## \#2 Posted by: anorak234 Posted at: 2017-05-19T22:18:01.605Z Reads: 134

```
Go 10s, and use the Samsung 30Q battery for the most bang for your buck with 18650s. You won't be sorry
```

---
## \#3 Posted by: pyttroll Posted at: 2017-05-19T22:18:34.090Z Reads: 132

```
Keep your kv under 200 for 10s.
```

---
## \#4 Posted by: nikoli280 Posted at: 2017-05-20T09:07:54.451Z Reads: 123

```
If i use under 200 it will go to slow. Why do you think i should use under 100

<img src="/uploads/db1493/original/3X/a/a/aa243dea462d11c3305725bf960da56e940603ca.JPG" width="689" height="353">
```

---
## \#5 Posted by: nikoli280 Posted at: 2017-05-20T09:08:22.118Z Reads: 113

```
Why do you think 10S is better? Its also the most expensive solution
```

---
## \#6 Posted by: Jammeslu Posted at: 2017-05-20T10:09:18.870Z Reads: 110

```
You Will hit the erpm limit with to Hugh kv
```

---
## \#7 Posted by: Tuomalar Posted at: 2017-05-20T10:40:00.097Z Reads: 108

```
Change wheel pulley to 36T and buy some bigger wheels for example Kegels or flywheels.
With 10s use 190kv motor so you don't need to limit your vesc and lower kv should give some more torque.
```

---
## \#8 Posted by: nikoli280 Posted at: 2017-05-20T10:56:46.164Z Reads: 107

```
Hi i bought a kit that has 48 teeth on the wheel and 15 on the motor so I have to use that. With that setup what would work best?
```

---
## \#9 Posted by: nikoli280 Posted at: 2017-05-20T10:57:08.066Z Reads: 105

```
What is ermp kimit
```

---
## \#10 Posted by: Tuomalar Posted at: 2017-05-20T12:06:27.273Z Reads: 107

```
Are those HTD3 pulleys? Picture? And what kit do you mean?

erpm = electronic rounds per minute
```

---
## \#11 Posted by: nikoli280 Posted at: 2017-05-20T13:03:56.493Z Reads: 99

```
I use this one for the motor. 

https://www.aliexpress.com/item/1pcs-HTD-3M-Timing-Pulley-15-Teeth-Bore-5mm-for-Width-15mm-3M-Open-timing-belt/32701634326.html?spm=2114.13010608.0.0.jol9is 

and this system but of course not the motor pulley 

https://www.banggood.com/DIY-Electric-Skateboard-Kit-Parts-Pulleys-And-Motor-Mount-For-80MM-Wheels-p-1146629.html?rmmds=myorder
```

---
## \#12 Posted by: Tuomalar Posted at: 2017-05-20T13:22:13.023Z Reads: 101

```
With this kit you can use only 50xx motors. I think you should learn first other people builds so you don't waste your money in wrong/bad parts. 
https://www.electric-skateboard.builders/c/e-board-builds
```

---
## \#13 Posted by: nikoli280 Posted at: 2017-05-20T13:53:44.812Z Reads: 97

```
You are right. But i plan on sawing off the egde of the motor mount if i choose to use a 60mm motor. But im just a bit confused about what i should get.
```

---
## \#14 Posted by: IsTalo Posted at: 2017-05-20T14:54:22.759Z Reads: 98

```
Lets begin, you can use 6s, it is cheaper, but less speed and less torque! If you use the Vesc you can't use a 260kv motor with 10s, because the Vesc have a ERPM limit, if you pass it you can burn your vesc, so do the calculation, Battery Voltage (4.2 x Number of Cells) x KV x 7, if this pass 60k you will need to limit your Vesc in the BLDC tool and lose speed! My opinion is that you need to search a bit more man, there are some mistakes on your build, like, a 380kv motor won't work nicely, it can run, but it will overheat and won't have enough torque! If you want a cheap build do this

-245kv 6364 Sk3
-6s 5000mah 25c
-Bms
-Vesc
-Switch and another things
-Diyelectric Mechanical Kit
```

---
## \#15 Posted by: IsTalo Posted at: 2017-05-20T14:56:13.692Z Reads: 88

```
Man, what is the 50xx motors mounting hole size? 25mm?
```

---
## \#16 Posted by: Tuomalar Posted at: 2017-05-20T15:13:49.086Z Reads: 92

```
My APS 5065 was 30mm/22mm or something.
```

---
## \#17 Posted by: IsTalo Posted at: 2017-05-20T15:42:37.678Z Reads: 86

```
So It is like a 63mm, the 63mm is 30mm too
```

---
## \#18 Posted by: Tuomalar Posted at: 2017-05-20T16:05:16.732Z Reads: 90

```
No it is not. But ofc it varies in some motors.
<img src="/uploads/db1493/original/3X/4/d/4dc2c884a4b36400a9d81dfea8fab64beaf7e8bb.JPG" width="375" height="500">
```

---
## \#19 Posted by: nikoli280 Posted at: 2017-05-20T16:07:42.554Z Reads: 88

```
Hmm i would like to use 10S. but what motor should i use and can i make it with 15 teeth motor pulley and 48 teeth wheel pulley with 70mm wheels. 

https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-149kv-brushless-outrunner-motor.html
https://hobbyking.com/en_us/turnigy-aerodrive-sk3-5065-236kv-brushless-outrunner-motor.html
https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-213kv-brushless-outrunner-motor.html
```

---
## \#20 Posted by: Rory Posted at: 2017-05-20T16:21:10.174Z Reads: 83

```
You could perhaps try this motor: 
https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6354-260kv-brushless-outrunner-motor.html
```

---
## \#21 Posted by: IsTalo Posted at: 2017-05-20T16:28:10.138Z Reads: 79

```
<img src="/uploads/db1493/original/3X/f/1/f1054393e5c49b30ee11a201ef724f7d2f6a0965.PNG" width="690" height="273"><img src="/uploads/db1493/original/3X/9/5/952419b40d96654a670f58ea0d8c5a84254845c7.PNG" width="690" height="280">

Look, this is the 63 and 50mm from Alien
```

---
## \#22 Posted by: Tuomalar Posted at: 2017-05-20T16:30:13.977Z Reads: 73

```
Ooh so Alien one those who varies. That 50xx i draw was Alien and right one from sk3 and r-spec
```

---
## \#23 Posted by: nikoli280 Posted at: 2017-05-20T16:46:28.520Z Reads: 72

```
Hi can someone help me with this setup and say if it will work.

Motor- https://hobbyking.com/en_us/turnigy-aerodrive-sk3-5065-236kv-brushless-outrunner-motor.html
Li-ion 10S pack.
Vesc - https://www.aliexpress.com/item/Maytech-Benjamin-Vedder-Electronic-Speed-controller-VESC-for-electric-longboard-DIY-skateboard/32712595711.html?spm=2114.13010208.99999999.299.M8caBO




<img src="/uploads/db1493/original/3X/6/5/65f3033839e98d40e385323f824051d14ebe297c.JPG" width="690" height="399">
```

---
## \#24 Posted by: Tuomalar Posted at: 2017-05-20T17:30:31.983Z Reads: 64

```
Change kv to 190 or lower battery voltage. 8s should be fine. Maytech's vesc are okay, but buy vesc-x or diy vesc if u want little better.
```

---
## \#25 Posted by: nikoli280 Posted at: 2017-05-20T18:28:53.202Z Reads: 63

```
Can this setup work? and do you know any good 50mm motors with 200kv ?
<img src="/uploads/db1493/original/3X/a/a/aab75c180799a9bb6e8a121cd2f1f6a51939497f.JPG" width="690" height="410">
```

---
## \#26 Posted by: nikoli280 Posted at: 2017-05-20T18:51:27.546Z Reads: 59

```
I think i have cracked it, what do you clever guys say? Can this work?

Motor - https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-213kv-brushless-outrunner-motor.html
10S - Litium Ion
10S 60A BMS.
Vesc? https://www.aliexpress.com/item/Maytech-Benjamin-Vedder-Electronic-Speed-controller-VESC-for-electric-longboard-DIY-skateboard/32712595711.html?spm=2114.13010208.99999999.299.M8caBO


<img src="/uploads/db1493/original/3X/1/9/196f193a6457c09055c2fa1e49fc890bd077cc09.JPG" width="690" height="377">
```

---
## \#27 Posted by: Tuomalar Posted at: 2017-05-20T18:59:23.592Z Reads: 49

```
That's fine. You should check that motor mounting pattern. I don't know how heavy you are or is there bad hills so hard to say how big motor you need.
```

---
## \#28 Posted by: nikoli280 Posted at: 2017-05-20T19:01:10.986Z Reads: 54

```
Yes i have allready ordered the 50mm tracktion and pulley set. So there is properly some modifications that i need to do to make the motor fit. But dont you think 2mm. solid steel is thick enough for the mount?
```

---
## \#29 Posted by: Tuomalar Posted at: 2017-05-20T19:06:12.391Z Reads: 48

```
To be honest that motor mount set is last one i could buy. It's dirt cheap, but there are so many better options
```

---
## \#30 Posted by: nikoli280 Posted at: 2017-05-20T19:24:09.307Z Reads: 48

```
Its cheap yes. But i have received one and the metal on the pulleys is fine quality and the mount is solid metal and the belt is fine to, so i dont se a reason why not to buy it. I just need to make sure its thick enough
```

---
## \#31 Posted by: Tuomalar Posted at: 2017-05-20T19:27:08.758Z Reads: 48

```
That one will be fine. What trucks you are planned to use?
```

---
## \#32 Posted by: nikoli280 Posted at: 2017-05-20T19:29:34.103Z Reads: 52

```
Paris 180mm. And a Madrid board. It will primary be a light transportation board. Thanks btw for your help. Do you have any other advice or suggestions about the build?
```

---
## \#33 Posted by: Tuomalar Posted at: 2017-05-20T19:33:07.169Z Reads: 50

```
If i understand right this kind of build is just like you're looking for 
https://www.electric-skateboard.builders/t/low-guidos-how-to-build-the-cheapest-but-still-good-esk8-video/23449
```

---
## \#34 Posted by: lowGuido Posted at: 2017-05-20T19:55:37.682Z Reads: 47

```
hell yeah it is ;)
```

---
## \#35 Posted by: nikoli280 Posted at: 2017-05-20T19:56:54.831Z Reads: 45

```
What motor and Esc/Vesc did you use?
```

---
## \#36 Posted by: lowGuido Posted at: 2017-05-20T19:59:03.410Z Reads: 43

```
I used a X-car beast 150A ESC from hobby king.
```

---
## \#37 Posted by: nikoli280 Posted at: 2017-05-21T09:26:36.920Z Reads: 45

```
Okay so i decided on the motor. Now my question is about reliability. 

I plan to use this BMS with max current draw continious is 60A. - https://goo.gl/ML7gqj
and i plan to use this VeSC - https://goo.gl/aM5INF
and ofcourse around 50 18650 batteries.

My question is how much should i max set the motor do draw in power? how many amps should i set in the VESC configuration. 

and should i install a fan and some heatsinks? 

What do you guys fink. Im not a wild rider so its mostly just transport
```

---
## \#38 Posted by: Tuomalar Posted at: 2017-05-21T09:41:23.990Z Reads: 46

```
Most of us use 60-80 amps in motor max but it doesn't draw that much. For example i use 40A fuse like almost everybody with vesc and haven't blew none despite my style is very agressive.

People have very mixed experienses with those cheap bms. I haven't tried but i know there is couple of more reliable ones. Like supower or batterysupports.
```

---
## \#39 Posted by: nikoli280 Posted at: 2017-05-21T09:56:29.380Z Reads: 45

```
Where do you place this 40A fuse? and how does your configuration look. I could buy from batterysupport.com its not that much more expensive. 

What do you think about heat? Should install heatsinks and fans on the BMS and esc or should i run the power around the BMS and then only use it for ballance chargegin?
```

---
## \#40 Posted by: Tuomalar Posted at: 2017-05-21T11:00:37.329Z Reads: 40

```
In my opinion you need bms only for charging, but everybody use it as fail safe between battery and vesc. If you only use it in charging you don't need that big bms. 10A is more than fine.

I don't think you need any fans or heatsinks. Ofc it helps if you live in hot enviroment and ride lot of hills.

My fuse is in negative line. I bet it should be on positive like it is in vedder's anti-spark but i don't have space to put it there.
```

---
## \#41 Posted by: nikoli280 Posted at: 2017-05-21T11:26:33.509Z Reads: 37

```
What do you do with short circuit protection and HV and LV protection. Did you make your board with 18650, if so how did you design the batteries? and what fuse do you use?

Thank you btw again for your help. I hope i dont ask to many questions
```

---
## \#42 Posted by: SilentException Posted at: 2017-05-21T11:40:57.597Z Reads: 38

```
How do you plan going 48T on wheel pulley on 83mm wheels?!? Pulley itself is like 82mm...

Edit: Oh, OK, it is 3M pulley. Your eBay link is broken in the first post...
```

---
## \#43 Posted by: nikoli280 Posted at: 2017-05-21T11:58:54.519Z Reads: 38

```
I will use this setup. https://www.banggood.com/DIY-Electric-Skateboard-Kit-Parts-Pulleys-And-Motor-Mount-For-80MM-Wheels-p-1146629.html?

Its the easiest for me
```

---
## \#44 Posted by: SilentException Posted at: 2017-05-21T12:17:28.826Z Reads: 38

```
Yes, as long as it is 3M it will work just fine. My mystake was thinking it was a 5M setup :) Not sure about the quality of that kit from BG but let us know...
```

---
## \#45 Posted by: nikoli280 Posted at: 2017-05-21T12:20:12.541Z Reads: 39

```
I have ordered some extra belts just in case. The metal is fine, its only the motor mount im a bit concerned about. Its only 2mm thick at the thinest. However its solid steel. Do you think it would be a problem? I am concedering buying a 0.5mm solid steel plate at taking myself many hours to cut out.
```

---
## \#46 Posted by: lowGuido Posted at: 2017-05-21T12:31:46.965Z Reads: 37

```
that kit looks acceptable.
although I'm more for making my own..

it wouldnt take hours to cut your own bracket.
```

---
## \#47 Posted by: nikoli280 Posted at: 2017-05-21T12:33:05.174Z Reads: 37

```
How thick do you think it would need to be? and what tools would you use. I dont have acces to some of the heavy duty automatic metal cutters
```

---
## \#48 Posted by: lowGuido Posted at: 2017-05-21T12:44:10.982Z Reads: 36

```
did you no watch my video? hack saw and hand file.
```

---
## \#49 Posted by: nikoli280 Posted at: 2017-05-21T12:56:56.126Z Reads: 35

```
Ahh that was your video, cool. How thich was the metal you uesd?
```

---
## \#50 Posted by: lowGuido Posted at: 2017-05-21T13:12:57.216Z Reads: 36

```
I used 6mm aluminium
```

---
## \#51 Posted by: KTMinni Posted at: 2017-05-21T13:43:21.385Z Reads: 35

```
Go 10S5P with some 30Q, 25R or HE2 cells
```

---
## \#52 Posted by: nikoli280 Posted at: 2017-05-21T14:02:50.061Z Reads: 34

```
Yep that is exactly what i though i would do, just with the LG HE4  insted of the HE2? Why do you think the HE2 is better?
```

---
## \#53 Posted by: KTMinni Posted at: 2017-05-21T17:23:36.043Z Reads: 31

```
They are just cheaper typically, and only 500mAh less but it's preference.
```

---
## \#54 Posted by: nikoli280 Posted at: 2017-05-21T17:36:33.627Z Reads: 34

```
Hi i found this esc. It can be programmed via computer. I was just wondering, is this as good as a Vesc? 

https://hobbyking.com/en_us/turnigy-super-brain-100a-brushless-esc.html
```

---
## \#55 Posted by: nikoli280 Posted at: 2017-05-21T17:52:56.899Z Reads: 32

```
And can you recommend some good 80-83mm longboard wheels? I have looked at the Orangutange Kegel. But they are quite expensive
```

---
## \#56 Posted by: KTMinni Posted at: 2017-05-21T18:37:16.334Z Reads: 30

```
It can accomplish some of the same things but with much less accuracy.  VESC is still recommended
```

---
## \#57 Posted by: KTMinni Posted at: 2017-05-21T18:37:36.597Z Reads: 31

```
And as for wheels look for ABEC flywheel clones.
```

---
## \#58 Posted by: nikoli280 Posted at: 2017-05-21T19:10:29.147Z Reads: 34

```
Great but i need some 80mm or 83mm. 90 mm is to big for me.
```

---
## \#59 Posted by: nikoli280 Posted at: 2017-05-21T19:11:03.068Z Reads: 34

```
Okay but why is it diffrent? And where do you find the best and cheapest Vesc? i found a Maytech for 109 dollars.
```

---
## \#60 Posted by: KTMinni Posted at: 2017-05-21T19:13:45.465Z Reads: 35

```
Maytech is fine if it has a bootloader.  Trust me, save up a bit more and get a VESC.  Diyelectric has VESCs for $99 I believe
```

---
## \#61 Posted by: nikoli280 Posted at: 2017-05-21T19:26:09.907Z Reads: 33

```
I live in europe so DIYelectric gets really expensive if i have to buy it from the US.

Can you say if this maytech has bootloader? Btw what is a bootloader

https://www.aliexpress.com/item/Maytech-Benjamin-Vedder-Electronic-Speed-controller-VESC-for-electric-longboard-DIY-skateboard/32712595711.html?spm=2114.13010208.99999999.342.SvbitA
```

---
## \#62 Posted by: KTMinni Posted at: 2017-05-21T20:30:59.998Z Reads: 35

```
It's really something you need to ask the seller.  A bootloader allows you to put firmware on the VESC and actually use it
```

---
## \#63 Posted by: Alex.Scheff Posted at: 2018-03-01T16:35:31.467Z Reads: 15

```
What type of "calculator" is this? :sweat_smile:
Thanks
Alex
```

---
