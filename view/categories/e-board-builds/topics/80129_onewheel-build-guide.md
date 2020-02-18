# Onewheel Build Guide

### Replies: 734 Views: 21823

## \#1 Posted by: Sindre Posted at: 2019-01-06T23:39:28.960Z Reads: 1079

```
Post your Onewheel build guides here!
![DSC02095|690x459](upload://7wo7j5eNmBaRrfnORvRLz3D4EGI.jpeg)![DSC02107|690x459](upload://pHWgjMUnc27QyZTRDsjWyazbagO.jpeg)  ![DSC02101|690x459](upload://qGKid9xVHWMSGuINEmADPIabtme.jpeg)

Firmware is not complete, but found code for a self stabilizing robot with the same gyroscope. Was first planning on using a microbit, but it was to laggy. Thinking of dooing the pid controlling in the vesc6, and need to convert pwm signal to ppm to make the code work.

https://github.com/kattemjau/OneWheel


Parts list:
10 inch hub motor with tire: http://bit.do/10inchhub
12s 3p 18650 pack from used laptop cells
vesc6: http://bit.do/vesc6
Arduino
Gyro: http://bit.do/gyroscup
Switch: http://bit.do/switchs
Motor mounts: https://a360.co/2CQGT64
End piece: https://a360.co/2CUvRwZ

Bought aluminium profiles, length 30 inches. Drilled holed according to mounts, and mounted all the pieces. In depth video coming.

TODO:
Shorten length to 20"-25".
Finish code, make stronger motor mounts.
Testing
```

---
## \#2 Posted by: moon Posted at: 2019-01-06T23:42:02.081Z Reads: 971

```
I think you are like the only one
```

---
## \#3 Posted by: mikenyc Posted at: 2019-01-07T00:26:22.672Z Reads: 963

```
Doesn't the Vesc6 ship with an IMU? Why use an Arduino?
```

---
## \#4 Posted by: AlanZhou Posted at: 2019-01-07T01:23:03.863Z Reads: 951

```
I would definitely build a onewheel but there are no good toturals lol.
```

---
## \#5 Posted by: Sindre Posted at: 2019-01-07T12:24:34.987Z Reads: 936

```
There is no gyro in the vesc, it is possible to rewrite firmware for the vesc and alter the pcb layout to connect the gyro over i2c. It seems not worth the hazzle right now. I am working on theese smaller vesc6 that will be perfect for theese kinds of builds.![49643205_2241519969298164_8509075540525711360_n|690x388](upload://3d59Ufi4cc6SjbCxrp647oy9QST.jpeg)
```

---
## \#6 Posted by: mikenyc Posted at: 2019-01-07T12:45:47.284Z Reads: 895

```
I could have sworn mpu9150 is in the bom
```

---
## \#7 Posted by: moon Posted at: 2019-01-07T12:48:27.781Z Reads: 866

```
Yeah in the official bom. But even trampa vescs decide to leave it unpopulated iirc, well escapes deffo does.

And Flipsky vesc 6 is not really a vesc 6
```

---
## \#8 Posted by: linsus Posted at: 2019-01-07T12:50:36.367Z Reads: 837

```
Its in the BoM, Vedder had some troubles with it from the first version and decided it wasn't worth the time at that moment. will probably be implemented in later versions.
```

---
## \#9 Posted by: mikenyc Posted at: 2019-01-07T13:14:00.402Z Reads: 826

```
i exchange a couple of emails with @trampa a while back. he mentioned that the new version will include the TDK 410-MPU-9250
```

---
## \#10 Posted by: Remieknaapen Posted at: 2019-01-07T13:24:37.457Z Reads: 817

```
What voltage did you choose for the hubmotor 
to run 12cells? 48v 600watt?
```

---
## \#11 Posted by: trampa Posted at: 2019-01-07T13:31:48.715Z Reads: 791

```
Definitely populated in the new version that is in production as we speak.
```

---
## \#12 Posted by: Sindre Posted at: 2019-01-07T14:18:25.398Z Reads: 781

```
I chose the lowest voltage possible, so i can current limit it in the vesc. It draws arround 1000w ish, going to push it harder
```

---
## \#13 Posted by: Giga Posted at: 2019-01-07T14:22:26.229Z Reads: 788

```
[quote="Sindre, post:1, topic:80129"]
Was first planning on using a microbit, but it was to laggy.
[/quote]

Which way did you feed the VESC? 

E.g. there is a ramp up/down for PPM/PWM signals, also for ADC and the nunchuck (I2C). So maybe it is not the ardunio which is laggy but the VESC having ramps which are too slow for balancing tasks. Also there are the PID controllers running at the VESC. So I would try minimizing the ramping or use UART commands (those don't have a ramp up /down deadtime) and adjust the PID controllers. 

Are you using hall sensors or an encoder?
```

---
## \#14 Posted by: Sindre Posted at: 2019-01-07T16:19:16.592Z Reads: 741

```
Hall sensors, ty for the information about the inputs to the vesc il do more testing. I was sending data through ppm, but are unsure if i was pid tuning it in the vesc. What I ovserved was that when writing ppm to the vesc, the accelleration was jerking. Meaning that it stopped sending data when reading the gyro. To test this we added a delay between eatch time we sent the ppm signal and the wheel stopped eatch time. Meaning the ppm controll from the microbit wasent hardware controlled but rather software controlled, causing a huge problem. We might have done something wrong or miss understood something, but il do some more testing. Im kinda swamped with other projects atm, but il come back to this later
```

---
## \#15 Posted by: Giga Posted at: 2019-01-07T16:59:00.384Z Reads: 713

```
[quote="Sindre, post:14, topic:80129"]
Meaning that it stopped sending data when reading the gyro
[/quote]
Sounds like a timer interrupt problem. 
I dont know the microbit but e.g. you cant use neopixel ws2812 leds together with servo/ppm control on arduino uno since one interrupts the other.
```

---
## \#16 Posted by: ryansinatra Posted at: 2019-01-07T17:02:29.513Z Reads: 688

```
Yeah, id love to build one. This is awesome 👌
```

---
## \#17 Posted by: Komamtb Posted at: 2019-01-07T19:57:22.224Z Reads: 696

```
so you can easaly run that motor with a vesc..?
```

---
## \#18 Posted by: Sindre Posted at: 2019-01-07T21:38:27.920Z Reads: 714

```
The vesc is perfect for this!
```

---
## \#19 Posted by: lrdesigns Posted at: 2019-01-08T01:09:38.837Z Reads: 742

```
What kind of witchcraft :woman_mage: is this? 

![image|574x306](upload://vBzX3tLPAc8hI0l7LAQiNwnjOmI.jpeg) 

Looks cool, what's the main goal of this design? How much power can they handle?
```

---
## \#20 Posted by: Remieknaapen Posted at: 2019-01-08T08:56:58.811Z Reads: 728

```
So just to make sure you ordered the 24v version with 600watt?  And you are runnig it on 12s (+-50v) and it produces aprox. 1000watt? What are the benefits chooaing the 24v instead of the 48v or even 60v version?
```

---
## \#21 Posted by: Sindre Posted at: 2019-01-08T10:37:56.581Z Reads: 669

```
I ordered the 600W + 36V version. This means at 36v the motor draws 16.6A. The amps run through the motor determend the temperature of the motor. So if I can run it at 16.6A at 50v i get a power of 830, but the motor wants to draw closer to 50 V / 2.1686747 OHM = 23 A. Arround 1100w. Im running it at 20 Amps right now.
Basicly i have the option to run them harder
```

---
## \#22 Posted by: Sindre Posted at: 2019-01-08T10:41:45.380Z Reads: 647

```
https://github.com/antonchromjak/MINI4/blob/master/20180124_215852.jpg

Its just a small cheap allarround vesc. Im building an electric couch, electric underwater jetpack, electric gocart, 4wd longboards, drones and hovercrafts. Im testing antonchromjak's design and are going to try to redesign it so i can run water cooling on them. Without cooling they run arround 20-30Amps, with cooling the mosfets can handle 120-200A. Prob needs alot of design changes before theese numbers are achived, and going to try to make them cheaper
```

---
## \#23 Posted by: sayekim Posted at: 2019-01-08T11:39:20.160Z Reads: 625

```
I’m disappointed there is no jet pack included for flight.
```

---
## \#24 Posted by: lrdesigns Posted at: 2019-01-09T01:07:52.692Z Reads: 615

```
I run my dual on 12s and limit each vesc to 18 amps. So maybe it could work for me. I'm skeptical though. Is there anymore info on these other than the github?
```

---
## \#25 Posted by: Sindre Posted at: 2019-01-10T18:54:46.771Z Reads: 596

```
https://vesc-project.com/node/246
```

---
## \#26 Posted by: Remieknaapen Posted at: 2019-01-18T11:26:31.773Z Reads: 606

```
Any news on this project?

I just ordered my hubmotor (600v 36v), can't wait to get started! I'll post some pictures of the design very soon.
```

---
## \#27 Posted by: briman05 Posted at: 2019-01-22T16:37:48.874Z Reads: 589

```
very interesting I want to see a video of this thing in action.
```

---
## \#28 Posted by: pozsy Posted at: 2019-01-29T15:13:09.128Z Reads: 582

```
I'm in a planning phase of something similar and curious, about the range and power(speed, hillclimb) you got with this set up. Have you tested these?
```

---
## \#29 Posted by: Sindre Posted at: 2019-01-29T16:27:31.456Z Reads: 576

```
Hi, I havent tested this yet. I got some serious torque from the motor, so im guessing it might handle it well. I need to redesign the motor mounts, when they break after a short time. I am thinking of integrating the spacer/skrews that came with the motor for this
```

---
## \#30 Posted by: Sindre Posted at: 2019-02-03T00:08:08.115Z Reads: 573

```
Hi guys, im dooing some market research on electric longboards and i would really appriciate some feedback!
https://docs.google.com/forms/d/1vufR2ZtxQFtgaUEYdl-zLTa9ne6JLkzKZyYPP63oG88/edit
I would really appriciate it for those who helped me out!
```

---
## \#31 Posted by: milanteubel Posted at: 2019-02-19T19:05:35.180Z Reads: 536

```
Have you guys made much progress?  I would love to see an update video/pictures of how its coming along!
```

---
## \#32 Posted by: Sindre Posted at: 2019-02-19T21:13:44.225Z Reads: 561

```
Hey, there hasent been anny progress so far. This was originally built as a student project and the group werent to motivated after christmas break and school started. I think to finish the project the motor needs to be bolted to the aluminium frame, made shorter and tweeked the code. The last 10% takes 90% of the time. If theres an update to the project, il post it here. Feel free to post your own build in this thread if you want!
```

---
## \#33 Posted by: Remieknaapen Posted at: 2019-04-03T19:09:07.603Z Reads: 571

```
I did make some progress. I'm still gathering parts so I can't fully work out the 3d model right now.
Currently waiting for the naze32 and velostat to show up so I can start configuring my electronics.
But it's starting to look like something. Rails will be made from a 20x40x20 mm U pofile with a wall thickness of 3mm. Other parts will be 3d printed or milled from wood.

Setup will be: Naze32, Focbox vesc, Peipei Phub 188 36v 600watt, 12s2p samsung 30q 18650, Velostat sensor

![onewheelprint|631x500](upload://rQsg44NJMxrX0xOvJQ77G3gyyfB.png)
```

---
## \#34 Posted by: Sn4pz Posted at: 2019-04-03T19:27:14.816Z Reads: 548

```
Looks VERY good! 

Do you think that you are ever going to go all metal?
```

---
## \#35 Posted by: ervinelin Posted at: 2019-04-04T00:39:12.525Z Reads: 532

```
Looks awesome. Which firmware are you using?
```

---
## \#36 Posted by: Remieknaapen Posted at: 2019-04-04T16:59:52.280Z Reads: 531

```
Thanks for the compliments.

Firmware I want to use comes from here: https://www.electric-skateboard.builders/t/onewheel-skateboard/15901/80?u=remieknaapen

Only metal parts will be the alluminium rails and the motor mounts. All the other parts stay plastic or wood.
```

---
## \#37 Posted by: megatesla Posted at: 2019-04-08T20:29:39.011Z Reads: 531

```
I ordered the 600W + 36V hub motor 9 days ago from that seller but it still hasn't shipped. No reply to messages on Aliexpress. I also visited the Pei Scooter website and contacted them there. Also no reply.

I do hope they ship it. I haven't found any other viable hub motor/wheel options.
```

---
## \#38 Posted by: megatesla Posted at: 2019-04-09T20:04:38.644Z Reads: 518

```
phew! Motor shipped today! 9 Days after ordering.
```

---
## \#39 Posted by: Surfer Posted at: 2019-04-09T20:23:50.090Z Reads: 520

```
Mind you to share the link of that motor?
I'm thinking to build a Onewheel too! 
I'm just planning the stuff because I can't code firmware, it should be kind of plug and play, trying to about that it just come to my mind the new vesc6 plus, it has gyro and Accel built in and firmware ready. I think is just to play with the PID controller settings. But really don't know.
What do you thing guys? It will work?
```

---
## \#40 Posted by: megatesla Posted at: 2019-04-09T20:26:59.531Z Reads: 513

```
Here you go. I haven't been able to find any similar motor for sale.

[Pei Scooter on Aliexpress](https://www.aliexpress.com/item/10inch-10-inch-10x6-00-5-5-wide-tyre-brushless-gearless-dc-wheel-hub-motor-balance/32823573279.html?)
```

---
## \#41 Posted by: MaxGoldenson Posted at: 2019-05-04T00:00:05.145Z Reads: 495

```
You are all welcome, I just finished a V1 Code with PID for Arduino to control a one wheel. Feel free to use my code, and ask questions. I will answer if I can.
LINK:
https://github.com/GAM3TIN/One-Wheel-code
```

---
## \#42 Posted by: Remieknaapen Posted at: 2019-05-08T21:54:08.492Z Reads: 471

```
Hi MaxGoldenson,

Have you tried this code using arduino on a actual board? I wonder if an arduino is fast enough ?
```

---
## \#43 Posted by: Sindre Posted at: 2019-05-08T22:09:11.486Z Reads: 462

```
It is, early drones was made arround arduino 32u4 mcu
```

---
## \#44 Posted by: MaxGoldenson Posted at: 2019-05-08T22:28:23.677Z Reads: 450

```
It is fast enough on an Arduino Uno, but the code is old and I've recently updated it to work with foot sensors and fine-tune along with being able to tell your weight to adjust the k i, k p & k d values
```

---
## \#45 Posted by: MaxGoldenson Posted at: 2019-05-08T22:28:55.223Z Reads: 424

```
I'm still working on it though
```

---
## \#46 Posted by: MaxGoldenson Posted at: 2019-05-08T22:31:17.212Z Reads: 422

```
Also Arduino is way easier to work with having to reprogram your vesc and all that crazy stuff
```

---
## \#47 Posted by: kalebludlow Posted at: 2019-05-09T00:13:00.384Z Reads: 419

```
Damn its super cool to see someone working on this. Do you have any sort of build process or parts list so people could start building their own?
```

---
## \#48 Posted by: Remieknaapen Posted at: 2019-05-09T04:33:56.012Z Reads: 419

```
Do you have that code available with the footpad sensors? I would like to try it and see if i can get it to work.
```

---
## \#49 Posted by: mikenyc Posted at: 2019-05-09T12:44:20.244Z Reads: 412

```
Have the footpad sensors been specified? A BOM would be great!
```

---
## \#50 Posted by: MaxGoldenson Posted at: 2019-05-09T20:15:04.445Z Reads: 443

```
Hello all who have commented, 

The code with the foot sensors is still a work in progress (the code works, but adding the foot sensors has broke other parts in the code) I have also added a Kalman filter to the gyro (so that there is minimal drift). The new code should be up soon. If you want to contact me about this project, or have any questions contact me at maxwellgoldenson@gmail.com, leave a comment on this form, or you can google hangout me (maxwellgoldenson@gmail.com) at 3-4pm (PST may 9th) To discuss.(this will be the best way, because I can share the most updated code along with answer most questions (as best I can). Good luck! And feel free to contact,
-Max

ALSO, If any of you are experienced in C++ then feel free to contact me (best via hangouts or email) To help me finish the code faster.
```

---
## \#51 Posted by: MaxGoldenson Posted at: 2019-05-09T20:16:35.172Z Reads: 422

```
If you want to discuss about this contact me on google hangouts from 3-4pm (PST may 9) today, and I can give you the work-in-progress code, and explain it.
```

---
## \#52 Posted by: MaxGoldenson Posted at: 2019-05-09T20:17:08.888Z Reads: 466

```
UPDATED CODE:

This code has compatibility with PID and Kalman filter built in along with foot sensors to turn it on.
The hook-up guide is a follows

Arduino-MPU6050

A4-SCL
A5-SDA
5V-VCC
GND-GND

Arduino-footsencors  
GND-ONESIDE
A0-OTHERSIDE

GND_ONESIDE
A1-OTHERSIDE
you will also need a 10k ohm pull up resistor from 3.3 to A0 and A1.

Arduino-VESC

PIN3-DATA
GND-GND
5V-5V

If you have any questions please comment on this form or contact me at maxwellgoldenson@gmail.com.

Links;

VESC

https:///products/torque-esc-bldc-electronic-speed-controller

Foot Sensor (FSR)

https://www.amazon.com/Adafruit-Round-Force-Sensitive-Resistor-FSR/dp/B00XW2MIRQ/ref=asc_df_B00XW2MIRQ/?tag=hyprod-20&amp;linkCode=df0&amp;hvadid=312727440900&amp;hvpos=1o3&amp;hvnetw=g&amp;hvrand=10104964395484814044&amp;hvpone=&amp;hvptwo=&amp;hvqmt=&amp;hvdev=c&amp;hvdvcmdl=&amp;hvlocint=&amp;hvlocphy=1013581&amp;hvtargid=pla-571396511975&amp;psc=1

Arduino 

. https://www.amazon.com/Teensy-3-2-with-pins/dp/B015QUPO5Y/ref=sr_1_3?gclid=CjwKCAjwiN_mBRBBEiwA9N-e_lwzqPukBJAB7jffS6Xo3iaYqIrGLus2Pp_4HR84tU6UIPkwBmX-MxoCzqYQAvD_BwE&amp;hvadid=176320835894&amp;hvdev=c&amp;hvlocphy=1013581&amp;hvnetw=g&amp;hvpos=1t1&amp;hvqmt=b&amp;hvrand=13756269608124661101&amp;hvtargid=kwd-35744547392&amp;hydadcr=3016_9782497&amp;keywords=teensy+arduino&amp;qid=1557721656&amp;s=gateway&amp;sr=8-3

CODE
https://github.com/GAM3TIN/ONEWHEEL_KALMAN_PID/tree/master
```

---
## \#53 Posted by: DAddYE Posted at: 2019-05-20T03:06:22.975Z Reads: 399

```
Thanks man! Anything else? Is there a motor in US? 

I’m not super experienced with c++ but I’m still an engineer :) so I’ll try to help out
```

---
## \#54 Posted by: Relys Posted at: 2019-05-20T05:04:11.235Z Reads: 415

```
I'm interesting in building one of these too. I can program in C and ASM if you still need help.

What do you plan to use for motor mounts? I imagine the wood is much weaker compared to the aluminum rails the OneWheel uses. Do you think it would be possible to use OneWheel rails (OEM or aftermarket)? Speaking of compatibility. What about tire options. Would this motor be compatible with Hoosier tires?

Also, what do you think about adding "LIDAR" (most likely ultrasonic or IR) sensors to the bottom front of the board? Like this board: https://www.hoverboard.com/ Might help prevent nose dives due to terrain. Maybe an Ultrasonic sensor like: https://www.amazon.com/WYPH-Ultrasonic-HC-SR04-Distance-Measuring/dp/B00P5W1JLM/ref=sr_1_6?keywords=Hc-sr04+Ultrasonic&amp;qid=1558330264&amp;s=electronics&amp;sr=1-6

Anyways, just wanted to say again how great a project this is. Hope it inspires many more builds to disrupt the OneWheel monopoly.
```

---
## \#55 Posted by: Fungineers Posted at: 2019-05-20T08:01:59.169Z Reads: 375

```
the ultrasonic thing is interesting.
```

---
## \#56 Posted by: Fungineers Posted at: 2019-05-20T08:02:14.130Z Reads: 380

```
@Remieknaapen did you try @MaxGoldenson  code?
Im gonna try it this week.
```

---
## \#57 Posted by: Relys Posted at: 2019-05-20T18:49:14.672Z Reads: 430

```
I think it would be interesting to use 3 of them in the front (that way you have redundancy in case one fails). It would also be interesting to use 3 IMUs as well (as we are kind of developing a safety critical system) lol

Regarding my question about using OEM or aftermarket OneWheel aluminum rails I found a couple of listings on ebay.

Stock XR rails for $175: 
https://www.ebay.com/itm/Onewheel-XR-NEW-Stock-Rails-PREORDER/173899174029?hash=item287d32d08d:g:~tIAAOSwxL1cZLeR

Aftermarket extended XR rails for $200:
https://www.ebay.com/itm/Onewheel-Plus-Billet-Rails-Preorder-Longer-For-Larger-Wheel/333162197731?hash=item4d9203b2e3:g:GP8AAOSwbjNcuF6Z

For a battery pack, has anyone considered using 21700 for extended range? https://www.imrbatteries.com/samsung-40t-21700-4000mah-30a-battery/
```

---
## \#58 Posted by: MaxGoldenson Posted at: 2019-05-22T03:40:35.234Z Reads: 408

```
No, because not only will be an accurate but when you till the ultrasonic sensor will be at a different angle and therefore providing you a different link that it senses. The problem is is that the sensor can't tell you how far from the ground you are but simply how far the sensor is from it's reference.
```

---
## \#59 Posted by: Dan333 Posted at: 2019-05-22T13:51:20.196Z Reads: 399

```
@Sindre Regenerative breaking wont be a issue when motor is 48V and battery pack is 12s…? Also what Vesc setting are you using?
```

---
## \#60 Posted by: Sindre Posted at: 2019-05-22T16:15:46.377Z Reads: 396

```
Reg braking works fine and no issues with the 12s. I am running 30A on it, and its running fine!
```

---
## \#61 Posted by: MaxGoldenson Posted at: 2019-05-22T16:21:17.630Z Reads: 360

```
you do realize that <b>12s is 50.4v,</b> that will kill a 48v motor.
```

---
## \#62 Posted by: MaxGoldenson Posted at: 2019-05-22T16:22:19.515Z Reads: 356

```
The motor is rated at about 15amps, 30 amps is not good
```

---
## \#63 Posted by: Relys Posted at: 2019-05-22T18:07:54.762Z Reads: 376

```
That shouldn't be a problem since we can calculate the gyroscopes distance relative to the ground (on a flat surface) if we use a little bit of trigonometry. We can then calculate the actual distance to the ground using the ultrasonic sensor (which is relative to the position of the gyroscope which is relative to the ground).

Even if we don't want to use the ultrasonic sensor, I think this equation is important as we could use it to implement a "pushback" feature (although instead of doing all the math you could just measure the gyroscope angle while positioning the tip of the board against the ground to calibrate it, but this would only work on flat surfaces). 

However, if you do all the math I think you could interpolate the ultrasonic sensor readings to get the angle of the ground (measured from the tip of the board to the center). You could give a warning if the angle of the ground approaches a certain value (as you can now  measure the exact distance of the nose of the board to the ground) or even allow the board to tilt back within a certain range to avoid nose dive.

I'm not sure how FM implements there version of pushback, but I think it may also be possible to calculate the angle of the ground by observing the amount of power delivered to the motor vs the current acceleration measured: http://trutechmotors.com/white-paper/wp-1-title/

Now that I think about it, we should probably start there and think about Ultrasonic sensors after we explore that method.
```

---
## \#64 Posted by: DAddYE Posted at: 2019-05-22T18:46:24.816Z Reads: 322

```
What version do you suggest 600W / 50v ?
```

---
## \#65 Posted by: CCU Posted at: 2019-05-22T19:21:12.891Z Reads: 334

```
12S(50V max, 43V average) seems a bit high for that motor and there is a high risk of wrecking the FOCBOX at 12S when relying on regenerative braking. 
A 10S battery system should be safe for both.
```

---
## \#66 Posted by: Surfer Posted at: 2019-05-22T19:24:45.963Z Reads: 349

```
The Onewheel has the pushback implemented in 3 ways, when you go up to 25 km/h, when the amps are increasing and getting close to the limit of capability of the battery to deliver more amps or volts to keep you balanced, and the last one when you reaching the limits of the motor, torque, revs/kv. 
 I think is easier to implement the pushback in that way than in the way with the ultrasonic sensor. 
Actually I don't find it useful a sensor that reads the surface since one of the best things of the ow is the ability to go off road, 25 km on a flat and long road could be a bit boring :)
```

---
## \#67 Posted by: Relys Posted at: 2019-05-22T19:46:33.906Z Reads: 358

```
Thanks, this is very useful information. I didn't even consider factors such as capability of battery. You could also limit speed when the battery drops below a certain % to help extended the lifetime of the cells. I don't think any current DIY OneWheel firmware (the Arduino, NAZE32 or VESC6 codebases) implements a pushback feature and is certainly a very important safety feature to have.

In my eyes, once the firmware is feature complete the main issue of DIY builds will be the rails. I don't think wood rails are a good solution long term with the amount of stress the motor produces via torque (not to mention going off jumps, etc.) and think that the aluminum CNC milled rails like the OneWheel uses are the way forward. Unfortunately, not a lot of people have access to CNC tools to build something like that and I don't think there are any open source blueprints for them. I asked about fitting OEM XR rails to this motor earlier but haven't had a response back yet (I suspect most people simply don't have the parts to test).
```

---
## \#68 Posted by: Surfer Posted at: 2019-05-22T20:05:25.903Z Reads: 340

```
You can't limit the speed on a ow the rider has to swift the weight before limit the speed if so instantly nosediving will happen. 
I own a ow but my idea was to go DIY, just are too many things out of my hand, coding is one of the most important things to fine tune the wheel that I can't do. The wheel of the hub motor available is 10", ow uses 11" difficult to find wheels that fit in there, and the wheel is one of the more important part that gives you stability, carving... And there is quite a lot of tested options with kart wheels with different properties, better for carving, less stability and so on.
P.s the spare parts of ow are stupid expensive, the CNC rails are close to 300 dollars!!!
I think the wooden rails are just fine for prototyping
```

---
## \#69 Posted by: Dan333 Posted at: 2019-05-22T20:18:22.201Z Reads: 305

```
well 18650 batteries are 3,7V so that would mean 44,4V no?
```

---
## \#70 Posted by: Dan333 Posted at: 2019-05-22T20:25:35.940Z Reads: 313

```
@Relys the pushback isnt that advanced, a quick boost to push you offbalance backwards and then drop the speed right after the push.

@Surfer I was also thinking about the size differenceof the wheel, so I'm considering to mount a shorter metal base about the width of the wheel and the mount the full length rails a bit above the centerpoint of the wheel to get some more clearance from the ground
```

---
## \#71 Posted by: AlanZhou Posted at: 2019-05-22T20:39:43.330Z Reads: 306

```
that's not true, brushless motors will work at any voltage (to a extent) until the voltage is high enough for the windings to arc you won't have any issues, and even when the wingdings do arc it is not going to cause a cooked motor.

also 48v is nominal voltage, 48v usually stands for 13s, 13s fully charged is 54.6v
```

---
## \#72 Posted by: FredrikHems Posted at: 2019-05-22T20:43:44.567Z Reads: 297

```
Your bearings will crap out way before your windings are going to arc..
```

---
## \#73 Posted by: Relys Posted at: 2019-05-22T21:09:42.308Z Reads: 310

```
In the other thread some people did a group purchase of 10x of these 11 inch wheels: https://www.aliexpress.com/store/product/11inch-350w-500w-wide-tire-hub-motor-phub-44/1470068_32536443206.html?spm=2114.12010615.8148356.4.350c51f63QudcB

Less info on them in the listing compared to the 10 inch ones though.
```

---
## \#74 Posted by: lrdesigns Posted at: 2019-05-23T00:43:36.386Z Reads: 333

```
[quote="MaxGoldenson, post:61, topic:80129, full:true"]
you do realize that **12s is 50.4v,** that will kill a 48v motor.
[/quote]

This is simply not true. 

The main limiting factor on brushless motors is amps which leads to overheating if the amps are too high. The amount of amps is relative to the load you put on your motor and esc settings. Voltage just controls max rpm. 

Also a 12s battery under load will be closer to 45 - 48 volts, so the 48v ratting is actually 12s. 

If its rated at 15a x 48v thats 720 watts. You could easily run it at 10a x 60v = 600 watts, it would run cooler. You would just lose some low speed torque in exchange for higher top speed.
```

---
## \#75 Posted by: Sindre Posted at: 2019-05-23T06:42:01.883Z Reads: 316

```
As long as the motor stays cool there is no problem. This only works with an Vesc that is constant currenting. An regular bldc controller would fry and motor by over volting it, beacuse it would instantly draw more amps than it can handle
```

---
## \#76 Posted by: StefanMe Posted at: 2019-05-23T07:38:43.194Z Reads: 317

```
Anyway... the 36V and 48V motor is the same :P

![2019-05-23%2009_37_36-Alibaba%20Manufacturer%20Directory%20-%20Suppliers%2C%20Manufacturers%2C%20Exporters%20%26%20Importers|674x184](upload://sqGpsalcP2MbqfI41P4d9sgh8fm.jpeg)
```

---
## \#77 Posted by: MaxGoldenson Posted at: 2019-05-24T03:49:21.402Z Reads: 285

```
hahahah thats funny.
```

---
## \#78 Posted by: MaxGoldenson Posted at: 2019-05-24T03:50:12.389Z Reads: 298

```
Want to join our whatts app? (me fungineers and a few others)
```

---
## \#79 Posted by: taz Posted at: 2019-05-24T05:29:49.686Z Reads: 335

```
Unlikely.

We use the same type of outrunners in RC helicopters with 12s and more than double the kv without problems.

Edit: Cafeine has not kicked in yet. Just saw this is not about normal esk8 motors. Disregard my remark.
```

---
## \#80 Posted by: lrdesigns Posted at: 2019-05-24T05:40:24.840Z Reads: 356

```
I think what @FredrikHems said is not falsified by your statement both can be true. 

I think he is talking more like 1000 volts. 

But I dont think its the bearings that break first. What happens first is the bell starts to expand, then becomes unbalanced, then explodes.  There is a youtube video where the do that. I think the motor rpm is like 80k - 100k they explode. 

They could probably go to 150k rpm if they were designed for that. Above that I think you need oil bearings. 

Now I want to research highest rpm motors.

Edit, Found the video, explodes at 200k rpm. :laughing:
https://www.youtube.com/watch?v=1TiePd7qng8
```

---
## \#81 Posted by: StefanMe Posted at: 2019-05-28T05:56:31.300Z Reads: 344

```
[quote="Relys, post:73, topic:80129"]
ough.
[/quote]

what thread?
```

---
## \#82 Posted by: homemademadness Posted at: 2019-06-19T14:10:31.624Z Reads: 315

```
has anyone had succes with max's code yet, i want to build a onewheel and make a very clear full tutorial on my youtube channel(homemade madness), but im no arduino expert
```

---
## \#83 Posted by: Sc0urge Posted at: 2019-06-26T06:25:40.714Z Reads: 308

```
@MaxGoldenson what's the deal with the two foot switches, is one intended for front, and one for rear? i had in mind that i'd only need one, and put it on the front foot, so i could disengage motors etc when the rear of the board is down (ie as i get on/off the deck)
```

---
## \#84 Posted by: Surfer Posted at: 2019-06-26T06:30:40.208Z Reads: 300

```
2 sensor in front, release 1 to disengage.
You can't put the tail down before disengage :)
```

---
## \#85 Posted by: Sc0urge Posted at: 2019-06-26T06:57:01.357Z Reads: 309

```
Sorry, I get what you're saying about not putting the rear down while it's engaged (else the motor would try to drive backwards until you release the switch) that was bad phrasing on my part.

I still don't get what the second switch does.
In my mind
Boarding:

* Left foot on rear (rear down)
* Right foot & pressure on front, brings front and rear level.
* Slide front foot to Engage switch, board now begins to respond to tilt sensor, and adjusts motor speed according.

Dismount/dead man's switch:
* release switch ( still riding, feet still in position).
* Motor stops responding to tilt, all balance manually performed by rider.
* When stationary (or slightly moving for rad sparks) put the rear down.
* Remove front foot.
* Crowd goes wild, ladies swoon, a bald eagle sheds a single tear.
```

---
## \#86 Posted by: StefanMe Posted at: 2019-06-26T07:37:44.418Z Reads: 300

```
I am a little bit exited as well... But the guy from PEI SCOOTER is horrible in communitcations and shipping speed. Parcel is still not at the shipping company. I dont expect the wheel in germany within the next two weeks.

![2019-06-26%2009_36_08-My%C2%A0AliExpress%20_%20Manage%C2%A0Orders|690x218](upload://9KBiH0UD6nqlLQ7MXhg3SV7lZhr.jpeg)
```

---
## \#87 Posted by: DAddYE Posted at: 2019-06-26T15:59:41.679Z Reads: 295

```
I believe the two pressure sensors go on both sides because in theory you should be able to ride in both ways.
```

---
## \#88 Posted by: Surfer Posted at: 2019-06-26T19:00:44.535Z Reads: 309

```
@stefanme don't leave it! We need you to develop this!!! I was so happy the day I see you coming to this thread :slight_smile:

@Sc0urge, the Onewheel has two sensors in the front pad to engage/disengage.
It works when you are pressing both of them then the motor engage, until there is clear, the funny part comes when you have to disengage, you have to lift your heel from the pad while you toes still pressing the another sensor and you are stationary, then disengage happens.

![300px-Sensor|300x225](upload://clBik7LpHLxYrjpFi1j1FlLdXnc.jpeg)
```

---
## \#89 Posted by: Fungineers Posted at: 2019-06-26T19:11:24.190Z Reads: 312

```
Hey guys, been working hard these past few weeks.
The mechanical assembly is almost done. 
The hard part is the code which Im working on. 
@Remieknaapen and @MaxGoldenson are also working on the same thing so might have one soon!
![IMG_20190625_190700|666x500](upload://ovy8YKEgpxGbqLpftv2IhZGrRfu.jpeg) 
Im gonna post updates on the YouTube channel regularly:   
https://youtu.be/65Tv4kycUSg
```

---
## \#90 Posted by: homemademadness Posted at: 2019-06-28T11:51:31.363Z Reads: 308

```
nice, ill be watching :slight_smile:
```

---
## \#91 Posted by: Schell Posted at: 2019-06-30T09:42:49.138Z Reads: 311

```
Hi, how do you plan to build the front footpad? I saw in the previous posts you might use FSRs? I'm wondering if you'll just have a few and use them like a simple switch, or will you try to emulate the two sensor design from future motion?

https://www.amazon.com/Adafruit-Round-Force-Sensitive-Resistor-FSR/dp/B00XW2MIRQ/ref=asc_df_B00XW2MIRQ/?tag=hyprod-20&linkCode=df0&hvadid=312727440900&hvpos=1o3&hvnetw=g&hvrand=10104964395484814044&hvpone=&hvptwo=&hvqmt=&hvdev=c&hvdvcmdl=&hvlocint=&hvlocphy=1013581&hvtargid=pla-571396511975&psc=1
```

---
## \#92 Posted by: StefanMe Posted at: 2019-07-04T14:13:49.856Z Reads: 300

```
But why u need two sensors...? I can see any benefit fromt the second sensor. If u need the second(back) sensor to disengage, for what to u need the first(front) sensor?
```

---
## \#93 Posted by: Surfer Posted at: 2019-07-04T15:31:26.477Z Reads: 291

```
Both sensors are in front, with one foot you press the two of them to engage, when you stop you must lift your heel to release one sensor then it disengage
```

---
## \#94 Posted by: StefanMe Posted at: 2019-07-05T05:43:30.947Z Reads: 288

```
yeah but WHY u need two. Just place a single sensor under your back foot and u have the same... because for disengage u just look onto the back foot sensor... 

For start u look maybe on booth sensors? I also cant see a reason for this. Maybe its more pratical?
```

---
## \#95 Posted by: Surfer Posted at: 2019-07-05T06:16:21.603Z Reads: 268

```
 There is some people Goofy, and some other are regular :slight_smile:
```

---
## \#96 Posted by: yecooboard Posted at: 2019-07-05T07:35:30.465Z Reads: 269

```
I think it is difficult to ride it. But I like it.
```

---
## \#97 Posted by: StefanMe Posted at: 2019-07-05T10:35:52.451Z Reads: 268

```
I think its super easy to ride... much easier then a eskate...
```

---
## \#98 Posted by: aidnani Posted at: 2019-07-12T06:45:41.317Z Reads: 289

```
Little late to the party, but wanted to share one I've been working on too. I'm using a VESC as well, with an ESP32 as the main MCU. This one has BLE built in, so I could easily write an app to tune the PID loop on the fly. I'm also using the MPU9250. It's somewhat rideable at the moment, but the motor doesn't have nearly as much torque as I was hoping, so it stalls out easily. I'm planning on upgrading to the same 36V 600W motor that others are using.    

Source code (in progress!) is here
https://github.com/aksidn8/OneWheelv2

![unnamed%20(2)|666x500](upload://6Sgvv5cX0DL6DRSgJJcuBZRBvhO.jpeg)!
```

---
## \#99 Posted by: StefanMe Posted at: 2019-07-12T06:59:36.508Z Reads: 283

```
Is there any benefit from the the MPU9250 to the MPU6050?
```

---
## \#100 Posted by: aidnani Posted at: 2019-07-12T08:00:51.284Z Reads: 283

```
Not for this project, it's just the first one that came up on amazon. I believe the MPU9250 is basically the same as the MPU6050, with the addition of a magnetometer. My code isn't using that, so it's essentially the same.
```

---
## \#101 Posted by: aidnani Posted at: 2019-07-12T08:05:16.243Z Reads: 275

```
On a sidenote, is there any benefit to implementing your own kalman filter (like @MaxGoldenson has done), rather than using the DMP built into the chip?
```

---
## \#102 Posted by: StefanMe Posted at: 2019-07-12T08:25:30.466Z Reads: 285

```
Not shure. i have motor/wheel, teensy 3.2, MPU6050 but still waiting for the rails and the milled parts.

![OneWheelSW_2019-Jul-12_08-21-31AM-000_CustomizedView132680728|625x500](upload://iULZMqEUvsUO9xDMCdjMvKyTK1P.jpeg) 
![PNG|625x500](upload://1Pkn2w9WcCTnVJ03X3I0BE0cH5s.jpeg) 
![2019-07-12%2010_23_49-Autodesk%20Fusion%20360%20(Education%20License)|690x409](upload://equb3vg2FyR6NVl14UZAs4fxHa6.jpeg)
```

---
## \#103 Posted by: Sc0urge Posted at: 2019-07-12T12:36:31.887Z Reads: 267

```
I've got almost everything I need, just waiting on battery, momentary switch, and some 6mm aluminum plate I'll use as the treads.
I've got rails, wheel and mount, a flipsky 4.12 vesc, and anti spark switch.
I'm going to use Max's code, but mod it a bit to only need one foot switch, might also add a timer so if foot slips or bounces, I don't lose power.
```

---
## \#104 Posted by: Sc0urge Posted at: 2019-07-16T11:53:26.367Z Reads: 285

```
Putting it all together, ended up using 50mm x 30mm aluminium for the bars, then 5mm aluminium plate for the treads. it's about 68mm long.

dummy fit:

[img]https://i.imgur.com/Gk5wixL.jpg[/img]

[img]https://i.imgur.com/lQcTSU1.jpg[/img]

[img]https://i.imgur.com/mSFJY5W.jpg[/img]

@TinnieSinker is going to build a 10s2p battery, then i'm off.
```

---
## \#105 Posted by: TinnieSinker Posted at: 2019-07-16T12:06:03.088Z Reads: 274

```
Oh hi! nice build man! your cells have arrived and will be able to build it in the next week or two
```

---
## \#106 Posted by: aidnani Posted at: 2019-07-21T05:58:19.468Z Reads: 269

```
https://www.youtube.com/watch?v=NZKiaWp6A8E

I've been able to get a rideable version of my OneWheel. Like I mentioned in the previous post, the motor is way under-torqued for this project so I'll be upgrading that soon.

I've written a pretty detailed blog post on how I did it, so hopefully you guys can find it useful!
https://aidnanidev.wordpress.com/2019/07/21/building-my-own-onewheel/
```

---
## \#107 Posted by: Math38 Posted at: 2019-07-22T13:23:54.233Z Reads: 260

```
Hello 

How do you upload the code in the flight controller board ? 
Could you tell us how you do it ? 
thanks
```

---
## \#108 Posted by: Remieknaapen Posted at: 2019-07-23T20:02:52.387Z Reads: 259

```
I'm using ST-link utility to upload the code to my naze32.
I did however receive a HEX. file from someone on youtube.
This guy has modified the code from alexB to work with the naze32. 

If you want the Hex file send me a PM and I can write you a small instruction on how it works and send that together with the HEX. File
```

---
## \#109 Posted by: Math38 Posted at: 2019-07-23T20:23:07.961Z Reads: 248

```
OK I send you a PM
```

---
## \#110 Posted by: Math38 Posted at: 2019-07-23T20:27:45.005Z Reads: 245

```
Sorry I'm not allowed to send PM 

But the hex file can be download in betaflight ? 
Like an upgrade local firmware ?
```

---
## \#111 Posted by: SwarleyAUS Posted at: 2019-07-24T14:46:33.166Z Reads: 246

```
This is my progress thusfar https://www.instagram.com/p/B0TOFtegb7s/?igshid=222wcmigbp7f 

Code: https://github.com/SwarleyAUS/ESP32_1Wheel
```

---
## \#112 Posted by: whittyman98 Posted at: 2019-07-25T03:43:44.461Z Reads: 243

```
Hey guys, I am embarking on my own one wheel build as well and I have gotten all the parts except for the hub motor and tire. I also ordered it from pei scooter and they are taking forever. For you guys who got the same motor how long did it take to arrive? Or even ship?
![image|690x58,100%](upload://rXben0aJq7N96hiSOb5DqD6yi01.png) 

I ordered mine on 6/26/19 and no email whatsoever from pei scooter.
```

---
## \#113 Posted by: Fosterqc Posted at: 2019-07-25T04:26:08.970Z Reads: 236

```
They didn't seem to be out of stock when I talked to them the other day, you should contact them again on AliExpress or email and if they don't respond file a claim with AliExpress (if you ordered there). I'm looking forward to ordering one in the near future after my esk8 build is finished. So your wait does concern me.
```

---
## \#114 Posted by: aidnani Posted at: 2019-07-25T05:23:25.501Z Reads: 233

```
I may have been lucky, but I got my wheel pretty quickly. I ordered it July 11, and just got it yesterday. Same exact phub-188 wheel.
```

---
## \#115 Posted by: whittyman98 Posted at: 2019-07-25T20:12:57.844Z Reads: 237

```
Where did you order it from?
```

---
## \#116 Posted by: aidnani Posted at: 2019-07-25T21:50:33.482Z Reads: 250

```
I got it from aliexpress.
https://m.aliexpress.com/item/32823573279.html?spm=a2g0n.orderlist-amp.item.32823573279&aff_trace_key=c16dd8f5ce904cc3a4a9bef5bcda673b-1562984940844-01833-UneMJZVf&aff_platform=msite&m_page_id=8874amp-tm9wclvOiJpqG1vaLoeKXw1564091382064
```

---
## \#117 Posted by: whittyman98 Posted at: 2019-07-25T22:02:48.640Z Reads: 251

```
Okay. Well I'm gonna cancel my order from the actual pei scooter website and reorder it on aliexpress.
```

---
## \#118 Posted by: DAddYE Posted at: 2019-07-26T17:12:10.685Z Reads: 250

```
I’m still torn if I should get 600w/36v or 600w/48v
```

---
## \#119 Posted by: Sindre Posted at: 2019-07-26T17:33:54.976Z Reads: 247

```
I got the 36v and running it on 48v and 55Amp. Its not eaven running hot. I really want to push it to 72v, but my vesc cant handle it. Im using it in an escooter btw
```

---
## \#120 Posted by: aidnani Posted at: 2019-07-26T18:04:25.594Z Reads: 246

```
If you scroll up a bit, @StefanMe had an email from the manufacturer. Apparently they're exactly the same motor haha. Im going to run 36V first, just because my board is heavy enough as is. If its lacking power I'll go to 48V
```

---
## \#121 Posted by: Sc0urge Posted at: 2019-07-27T09:23:52.573Z Reads: 245

```
threw it all together, today (without electronics) to dummy fit it all, and tried some balancing.
turns out i'll need to work on it.
![67706789_2297118803689528_2228285207042064384_n|690x360,75%](upload://MYmfURxezwFPGeq3o9MKyZ1jHf.jpeg) 
https://www.youtube.com/watch?v=plocabqmbkk
```

---
## \#122 Posted by: Surfer Posted at: 2019-07-27T10:02:28.353Z Reads: 238

```
With the motor engaged is a lot more easier, you get the point in the first minute.
Your build looks bad ass!!
```

---
## \#123 Posted by: Sc0urge Posted at: 2019-07-27T10:14:48.090Z Reads: 233

```
thanks mate, when it's up and running i'll post how i put it together, don't want to cost people $$ if it doesn't work.
didn't use a 3d printer, or have to mill out custom mounts, just dremel, drill press, and aluminium box tube.
```

---
## \#124 Posted by: Fungineers Posted at: 2019-07-31T18:28:46.447Z Reads: 234

```
How much current does it draw and is it fast? I couldnt get the motor to run fast enough while testing. Just draws 2 3 amps at no load
```

---
## \#125 Posted by: Fungineers Posted at: 2019-07-31T18:29:15.052Z Reads: 242

```
Progress: 

https://youtu.be/RZwWWSBSPQk
```

---
## \#126 Posted by: Fungineers Posted at: 2019-07-31T18:30:08.069Z Reads: 241

```
Running it on rhe bench was successful but the motor isnt fast. Anyone got the peipei scooter motor running? Is it fast? How much is the current draw?
```

---
## \#127 Posted by: Sindre Posted at: 2019-07-31T19:05:11.877Z Reads: 247

```
It goes like 35-40 kmh at 48v, and at load it draws 50amps, spinning up at no load it takes 20-30 amp. Using the controlls in the vesc tool it freaks up sometimes, try connecting an potmeter to adc0 for testing
```

---
## \#128 Posted by: Fungineers Posted at: 2019-08-04T04:21:28.648Z Reads: 249

```
Hey guys. 
Heres a little teaser. Still needs bumpers.

![IMG-20190803-WA0006|375x500](upload://6yROkYHO5os0rrut7jGs2Zdb6io.jpeg)
```

---
## \#129 Posted by: Tiffa Posted at: 2019-08-04T15:13:41.879Z Reads: 243

```
looks soooo sick. I'm a teenager really looking into making a one wheel but are really getting confused. and plus how much does yours cost.
```

---
## \#130 Posted by: Fungineers Posted at: 2019-08-04T15:27:11.321Z Reads: 230

```
Check the first video in the playlist. Its got a full cost breakdown.
```

---
## \#131 Posted by: Tiffa Posted at: 2019-08-04T15:51:48.728Z Reads: 225

```
I'm on holiday and not able to watch it till tomorrow. Was the build hard. Are you using pressure plates.
```

---
## \#132 Posted by: Tiffa Posted at: 2019-08-04T17:09:37.313Z Reads: 217

```
does yours use pressure plates and I watched the video on my data by the way really interesting and helpful.
```

---
## \#133 Posted by: Giga Posted at: 2019-08-05T01:18:25.002Z Reads: 222

```
Trust me, the OneWheel is cheaper than any DIY.

You will have a learning curve and definitely fry stuff, need some parts to test and extra tools to assemble. 

You will learn quite a lot, no doubt about that, it is a nice hobby to build something, but if you are just doing it because of the costs: Any product sold in series are tested, and "mass" produced, hence cheaper and more robust than DIY stuff.
```

---
## \#134 Posted by: Fungineers Posted at: 2019-08-05T04:48:25.877Z Reads: 222

```
Depends how much you know about motors, batteries, arduino and vesc. I would say medium difficulty. Also depends on where you will source the rails how/where you will make the enclosures. Can you weld or not. So yea, could be challenging.
Yes I used velostat to make pressure pads.
```

---
## \#135 Posted by: Fungineers Posted at: 2019-08-05T04:50:22.372Z Reads: 230

```
I couldnt agree more. However, the Onewheel is overpriced. Mine is gonna cost me around $300. Maybe $400 tops. But I like building stuff. I had calculated the risk of failure = loss of $400 and I was OK with that. Most people are not patient, and they are not willing to risk $400; which is fine. If you are the latter, spend $1000 and get a pint or something I guess.
```

---
## \#136 Posted by: SwarleyAUS Posted at: 2019-08-05T13:16:10.758Z Reads: 239

```
Mine has cost me about AU$450. All I would spend more on now is additional battery capacity. The real cost, as mentioned above, is developing the code... the OneWheel is a complicated beast.

- VESC $100
- Motor $90
- Batteries (6S 6Ah) $120
- Wheel & tyre $60
- Axle and bearings $40
- Sprocket & chain $40
- Hardware $50

If Fungineers' motor works well then you could save some money doing it the 'turn-key' way rather than how I've done it, with an indirect drive system.
```

---
## \#137 Posted by: Khurtana Posted at: 2019-08-06T09:23:39.776Z Reads: 236

```
Is this now available?  Don't mind doing some dirty coding, but it would be great to know how to differentiate a VESC 6 with and without a gyro.
```

---
## \#138 Posted by: Pimousse Posted at: 2019-08-06T12:47:44.829Z Reads: 235

```
The IMU is included in VESC6+, not populated in previous version IIRC.
```

---
## \#139 Posted by: Sindre Posted at: 2019-08-07T07:35:49.497Z Reads: 227

```
The vesc has an spi or i2c output header you can connect an gyro directly to if you wanna do some modification to the code. just buy an breakout board of the gyro/acc
```

---
## \#140 Posted by: Khurtana Posted at: 2019-08-11T02:10:10.203Z Reads: 224

```
How are you going, Sc0urge?
```

---
## \#141 Posted by: Dan333 Posted at: 2019-08-11T17:17:33.973Z Reads: 217

```
For those of you who have the Peipei Phub 188 36v 600watt, what are the settings you used to do the configuration in VESC Tool?
```

---
## \#142 Posted by: Khurtana Posted at: 2019-08-12T00:51:18.998Z Reads: 214

```
Dan, are you using an external gyro or a VESV 6+?
```

---
## \#143 Posted by: Dan333 Posted at: 2019-08-12T04:57:24.309Z Reads: 210

```
Im using a vesc6+ and running a custom firmware with the stabalizationcode..
```

---
## \#144 Posted by: Khurtana Posted at: 2019-08-12T05:26:37.248Z Reads: 205

```
Great stuff, Dan.  Can you supply a link to the custom repo?  Is it an official VESC 6+ or a clone?
```

---
## \#145 Posted by: Khurtana Posted at: 2019-08-12T05:27:03.136Z Reads: 201

```
I'm starting to acquire parts so am in research mode.
```

---
## \#146 Posted by: Dan333 Posted at: 2019-08-12T05:49:26.124Z Reads: 202

```
I've cloned the official one locally, will give out the code when its ready
```

---
## \#148 Posted by: Pimousse Posted at: 2019-08-12T14:08:37.388Z Reads: 214

```
Someone made a PR for adding a self-balancing app to the official FW :
https://github.com/vedderb/bldc/pull/99

It targets EUCs but can be used with for DIY OW I guess.
```

---
## \#149 Posted by: Tiffa Posted at: 2019-08-12T15:42:11.402Z Reads: 206

```
Has anyone finished and live near Stafford UK. As I really want to try one.
```

---
## \#150 Posted by: Khurtana Posted at: 2019-08-13T03:08:45.844Z Reads: 203

```
Hopefully get gets added in the main code.  Now if I could find a cheap VESC 6+ with a built in IMU I'm in business.
```

---
## \#151 Posted by: Khurtana Posted at: 2019-08-13T12:37:10.178Z Reads: 202

```
Can any of our VESC-experienced members give me some advice?  How does this look?  Can you tell if it has an onboard gyro/IMU?  https://www.ebay.com.au/itm/FLIPSKY-FSESC-6-6-Based-on-VESC-60A-ESC-with-Heat-Sink-for-Electric-Q9U7/273902285829?hash=item3fc5d93405:g:fEwAAOSw4u9dDJFI
```

---
## \#152 Posted by: Sindre Posted at: 2019-08-13T13:03:03.954Z Reads: 202

```
Hi, flipsky esc does not include anny gyro. Only vesc6+ includes it. I think trampa sells the originals
```

---
## \#154 Posted by: xjujo Posted at: 2019-08-15T04:18:32.557Z Reads: 196

```
So, my issue as of now is that my onewheel XR controller module is broken. Battery and BMS, and motor is fine. Is it possible to use a Unity to replace the old controller?
```

---
## \#155 Posted by: MysticalDork Posted at: 2019-08-15T07:21:16.568Z Reads: 207

```
Probably, if you are willing to work for it.

The Unity is a dual ESC - you only need one output - half wasted.

The communication protocol used by the onewheel to communicate with its controller is probably not one of the ones that the unity supports natively - reverse engineering required.

I don't know where the IMU on the onewheel is - might be on the controller module, might be somewhere else. Probably best to use your own - more engineering required to make your unity communicate with the IMU, and to get the PIDs right for stable self-balancing.

Honestly if you can get a replacement controller, I'd just do that - less effort than doing a full soup-to-nuts gut-and-stuff with different hardware and software.
```

---
## \#156 Posted by: Surfer Posted at: 2019-08-15T08:08:34.822Z Reads: 199

```
Unity or vesc doesn't reach to 15s as the battery of the XR, only to 12s.
And if you looking to this solution because you want to save some money, that will not work for you.
This still in very early stage of development, actually is almost just rideable.
Btw, what happened to your controller? Did you open it?
```

---
## \#157 Posted by: Dan333 Posted at: 2019-08-15T10:40:55.561Z Reads: 209

```
For those with a VESC 6 who want to try out Mitchells Balance commit
https://github.com/vedderb/bldc/tree/05d81a6e66418855d3c61a8265546015c33fcb6d
https://github.com/vedderb/vesc_tool/tree/30c94918e639e0732ad53d655f0f560240d9b665

I have compiled the firmware (VESC 6!) and vesc_tool
https://drive.google.com/open?id=1lr5dlwLUmzQg9LgtGNpdGcR3M8jowReo

In the Vesc tool configure
App Settings -> General -> [APP to Use] to BALANACE
App Settings -> Balance -> [Use Peripheral I2C Gyro] for internal/external usage
```

---
## \#158 Posted by: xjujo Posted at: 2019-08-15T16:05:49.736Z Reads: 206

```
Yea somehow forgot that the onewheel is literally just one motor so unity would be kinda too much lol. 

Right now, I've verified battery, BMS, motors, sensor pads are fine. Turning on the controller, blue LED is lit just normal. No fast blinking, just the slow dimming in and out (waiting for input). I open the app and I tilt the board and I'm getting all battery percentage, gyro, everything. 

But no front and back LEDs and motor does not engage when I get on. The motor is "on" because there's that resistance when the controller is on, but it's not engaging. 

I found cold solders to the connector port for the sensor pads so I soldered those back on. I checked inductor L1 and it's rock solid. 

I have no idea.
```

---
## \#159 Posted by: Dan333 Posted at: 2019-08-15T16:39:41.830Z Reads: 195

```
maybe the imu is gone?
```

---
## \#160 Posted by: Surfer Posted at: 2019-08-15T17:17:04.233Z Reads: 196

```
Matiss rapsa is your guy, in FB owners group, he knows the shit like nobody else.
Good luck!!
```

---
## \#161 Posted by: Surfer Posted at: 2019-08-15T17:21:29.574Z Reads: 202

```
Thanks buddy for compiling this, I ask to Mitchell and he didn't want it :frowning:
Btw, I have vesc 6 (escape) and it has not populated the mpu 9250, do you think I can put it in, It will work ? :)  I don't know firmware wise, I can't code that, i just can make blinking a led in Arduino :P
```

---
## \#162 Posted by: ShutterShock Posted at: 2019-08-15T18:18:47.239Z Reads: 196

```
Yo if it only cost this much in AU I am totally down to build one in the US haha
```

---
## \#163 Posted by: Dan333 Posted at: 2019-08-15T18:34:51.677Z Reads: 186

```
then you need to configure it to use an external Gyro and it should work.. Im playing around with the costum vesc tool as we speak and it lives! :smiley:
```

---
## \#164 Posted by: Dan333 Posted at: 2019-08-15T18:48:39.417Z Reads: 186

```
the auther does not want to many people asking to many questions on how to get this running as he has not yet had time to write an configuration tutorial, but ask me and I'll see if I can help
```

---
## \#165 Posted by: TowerCrisis Posted at: 2019-08-15T19:23:24.684Z Reads: 184

```
Woah, what vesc is that and how much is it?
```

---
## \#166 Posted by: Dan333 Posted at: 2019-08-15T19:41:51.039Z Reads: 190

```
its the one Im using
http://www.trampaboards.com/vesc-6-plus-benjamin-vedder-electronic-speed-controller-p-26762.html
```

---
## \#167 Posted by: TowerCrisis Posted at: 2019-08-15T19:55:09.520Z Reads: 181

```
That's just a vesc 6 my guy, my comment was about the picture
```

---
## \#168 Posted by: Dan333 Posted at: 2019-08-15T20:11:24.837Z Reads: 186

```
sorry about that, just scrolled up to see what I thought you responded to..
```

---
## \#169 Posted by: Dan333 Posted at: 2019-08-15T20:13:03.856Z Reads: 190

```
those are the vesc mini's
```

---
## \#170 Posted by: Surfer Posted at: 2019-08-15T20:41:41.409Z Reads: 205

```
Wow that's Nice!!!!.

Sorry I didn't explain properly, I mean I can solder the mpu which is not populated in the PCB, once is done, do you think this mpu 9250 is the same than the vesc 6+ you have?
![IMG_20190815_223716|250x500](upload://a76lB8ivmLzyhVWiWnSvQZzyGnF.jpeg)
```

---
## \#171 Posted by: Khurtana Posted at: 2019-08-15T23:38:05.817Z Reads: 193

```
What is the orientation of the gyro?  I believe most EUCs are vertical - we will of course be mounting at 90 degrees - horizontally.  How is this configured?  Via VESC_TOOL?
```

---
## \#172 Posted by: Khurtana Posted at: 2019-08-15T23:42:51.535Z Reads: 185

```
Hi @Dan333, is the IMU JUST an IMU or do you need a Teensy as well?  If I could get away with a VESC mini and a simple external IMU I'll be very happy (my wallet would certainly be!)
```

---
## \#173 Posted by: Fungineers Posted at: 2019-08-18T04:58:31.403Z Reads: 186

```
worked best for me when i selected the 'hub motor' in the motor config wizard. rest is simple.
```

---
## \#174 Posted by: Sindre Posted at: 2019-08-18T07:52:08.483Z Reads: 194

```
Try checking the pressure pads
```

---
## \#175 Posted by: Dan333 Posted at: 2019-08-19T06:36:53.185Z Reads: 186

```
Im unsure as I have the internal IMU..
```

---
## \#176 Posted by: Dan333 Posted at: 2019-08-19T06:44:22.496Z Reads: 191

```
you can check the ref design I guess, but looking at the code and knowing that the MPU-9150 was the old one I guess icm 20948 is what is being used in the Vesc6Plus
```

---
## \#177 Posted by: Dan333 Posted at: 2019-08-19T06:51:40.450Z Reads: 187

```
Do you mean the 'DD...' ?
```

---
## \#178 Posted by: Surfer Posted at: 2019-08-22T22:49:20.903Z Reads: 183

```
Any chance any of you know the pinout for external gyro to vesc?
Thanks
```

---
## \#179 Posted by: Fosterqc Posted at: 2019-08-24T03:08:58.167Z Reads: 184

```
http://vedder.se/2015/08/vesc-writing-custom-applications/
```

---
## \#180 Posted by: Khurtana Posted at: 2019-08-30T04:56:39.538Z Reads: 189

```
Maybe try on the VESC official forum?  Don't think anyone knows here.
```

---
## \#181 Posted by: Ackmaniac Posted at: 2019-08-30T13:49:37.154Z Reads: 187

```
Just use a Arduino which you connect via Serial to the VESC. And then give current or duty commands.
```

---
## \#182 Posted by: Pimousse Posted at: 2019-08-30T15:15:44.795Z Reads: 183

```
Or wait a few that [this PR](https://github.com/vedderb/bldc/pull/99) gets merged. :slight_smile:
```

---
## \#183 Posted by: Surfer Posted at: 2019-09-02T13:31:54.049Z Reads: 176

```
in a matter of days!! this merge will happen :smiley::smiley:
```

---
## \#184 Posted by: Khurtana Posted at: 2019-09-03T13:26:11.773Z Reads: 174

```
I’m liking the progress made on the VESC6+ with the IMU support via the pull request.  I’m now officially in parts acquisition mode.

Alongside the PHUB188 10” tyre and the VESC, what are people recommending for:

1/ Anti Spark switch.  I want to use an AV switch if possible.
2/ BMS and charging system.  Looking for a 12S solution.  If my battery pack is 12S2P does this make a difference to my choice of BMS?  Thanks.
```

---
## \#185 Posted by: Surfer Posted at: 2019-09-03T17:26:47.501Z Reads: 167

```
No difference for the BMS
```

---
## \#186 Posted by: Surfer Posted at: 2019-09-03T19:26:32.827Z Reads: 168

```
Guys! The pull request is already merged to official vesc tool!! @Dan333 maybe you are up to compile it for all of regular humans? ☺️

Edit: yeah If is official there is a installer available in vesc project site, thanks anyway @dan333!! :)
```

---
## \#187 Posted by: Byngham Posted at: 2019-09-05T17:01:22.767Z Reads: 172

```
Noob question for a new build--

If I'm reading this right, it sounds like this is adding an app to run the self-balancing capabilities directly on the VESC 6?  Is that the direction that folks are headed at this point for a OneWheel project?  (rather than programming to run on an Arduino with MPU-6050 gyro connected to it?)

If it is the direction that people are headed, how would other functionality that isn't strictly self-balancing be implemented into the system? (i.e. foot pads to allow machine to activate, etc...)

Thanks for any guidance anyone can offer.
```

---
## \#188 Posted by: Surfer Posted at: 2019-09-05T17:08:21.735Z Reads: 164

```
Yes, I think is the way to go lately, foot pad functionality is coming in the next or two releases
```

---
## \#189 Posted by: murdomeek Posted at: 2019-09-05T18:20:20.498Z Reads: 163

```
how does this ride compared to the real thing?
This build seems fairly budget friendly :)
```

---
## \#190 Posted by: Dan333 Posted at: 2019-09-05T20:14:29.340Z Reads: 167

```
the code for self balansing is comming along and I'm testing each update and having a dialob with the developer.. its getting better and better..
also I am currently impementing some code for velostat footsensor(s) using the free adc on the vesc6+
```

---
## \#191 Posted by: Dan333 Posted at: 2019-09-05T20:16:44.495Z Reads: 159

```
Im using the DieBieMS BMS witch includes a antispark switch and a oled battery display
```

---
## \#192 Posted by: Dan333 Posted at: 2019-09-05T20:27:31.827Z Reads: 159

```
the pull has not yet been accepted to the firmware..?
```

---
## \#193 Posted by: Byngham Posted at: 2019-09-05T21:32:14.315Z Reads: 165

```
Your work to implement velostat foot sensors sounds great!  

We have plenty of work ahead of us with the rest of the build, so waiting a release or two probably won't hurt us.  Do you have *any* idea what sort of timeframe it might be (not gonna hold anyone's feet to the fire or anything, but would like to know if it's likely closer to 6 days, 6 weeks, or 6 months).  I'd be happy to try and help out, but would be starting from scratch to learn the codebase.  It might be better (and get results faster) for me to simply offer to buy you pizza and beer (or your foodstuff and beverage of choice.)
```

---
## \#194 Posted by: Dan333 Posted at: 2019-09-05T21:48:14.984Z Reads: 164

```
functions should be in place But I am getting eratic behaviour from the voltage read so code might be good but hw implemenetation wrong or vice verce ..

anyhow.. here is the newest compilation (footsensor code commented out)
https://drive.google.com/open?id=1WJY9ggXaXBhBqBDRpQ03CQ7F_6sL_kmW
https://drive.google.com/open?id=1vnAtKTQ8TPS8Kdvb25i2i3Ba5oL2ZX0O
```

---
## \#195 Posted by: Surfer Posted at: 2019-09-06T07:45:06.104Z Reads: 170

```
I think I was too enthusiastic, later I realized the last changes where made with the news of Benjamin, not from Michlol, I suppose the code of Michlol will be next release, but just guessing.
Btw I can't connect the mpu9250 with vesc, don't know why, maybe wiring is not correct, but I asked in vesc project forum couple days ago, but no answer at all.
If someone can confirm the wiring I will be sooo happy.

Here is how is connected now:

Vcc to vcc or 5v

Gnd=gnd

Scl=scl

Sda=sda

The only thing I can think now is if sda or scl are crossed like Tx Rx in UART

Edit: copy from vedder answer:

Many of the changes were inspired from your code :-) (Michlol code)
Then I will call it a half merge :slight_smile:
```

---
## \#196 Posted by: Surfer Posted at: 2019-09-08T17:13:30.139Z Reads: 162

```
@Dan333 mind you to give a basic instructions where are the comments for the food pad sensors? I can't find them, the only thingie I know is using one of the ADC free from the vesc.
Thanks mate
```

---
## \#197 Posted by: Fungineers Posted at: 2019-09-10T11:26:21.901Z Reads: 170

```
This was a month ago before my VESC decided to stop working with PWM/PPM. Been trying to get UART communication to work eversince...
https://www.instagram.com/p/B0-R7X6nm5p/?utm_source=ig_web_copy_link
```

---
## \#198 Posted by: NuRxG Posted at: 2019-09-10T16:46:51.367Z Reads: 177

```
There is a "bug"/"missing feature" in the vesc code. It uses a whitelist of I2C addresses for the MPU9250, and at least for the MUP9250 that i got off amazon, the I2C address is not on the list. That is why i made this change.
https://github.com/vedderb/bldc/pull/99/files#diff-53a15c0fa0ae6cf77d3bf13e9efbe03d

This is likely your issue. The options are to wait for my pr to merge, buy a different gyro (MPU6050 works if you have one, BMI is probably the best but i haven't tested it yet.), or maybe there is a jumper or something you can use on the MPU9250 to change the address (not sure if thats real or not, i vaguely recall reading it somewhere)
```

---
## \#199 Posted by: NuRxG Posted at: 2019-09-10T16:49:41.073Z Reads: 176

```
For anyone trying to make velostat sensors, here is a video on what I've found is the best method. I spent almost a year trying different things, and riding on these, so it is pretty legit. (I don't have any more kits for sale, but if there is a big demand, maybe i can make a 2nd batch)

https://www.youtube.com/watch?v=lRXuF9i6rS0
```

---
## \#200 Posted by: Surfer Posted at: 2019-09-10T18:26:39.811Z Reads: 172

```
Welcome @NuRxG this is getting exciting!!! 
Awesome what you are doing man, thanks to bring euc's and ow to the DIY scene.
Yep I installed your firmware and I'm getting data from the gyro, still I didn't figure out how to get pid output working, but yeah I will keep trying :slight_smile:
```

---
## \#201 Posted by: Dan333 Posted at: 2019-09-10T18:30:07.840Z Reads: 170

```
NuRxG's firmware and tool compiled:
https://drive.google.com/open?id=1P4fH0ElScqcCFjRPi1QL67V5vr8w9pFa
https://drive.google.com/open?id=1ohs1fCiWh4iXqvapdxxtC3WteS24tGXl
```

---
## \#202 Posted by: NuclearDynamic Posted at: 2019-09-11T11:15:48.608Z Reads: 165

```
I’ve been watching these videos...keep it up!
```

---
## \#203 Posted by: Pimousse Posted at: 2019-09-11T13:23:33.902Z Reads: 152

```
I'd be interested for 2 units.
Do you have a cost estimation ?
```

---
## \#204 Posted by: butt_stallion Posted at: 2019-09-11T15:16:49.000Z Reads: 155

```
I'd be interested as well
```

---
## \#205 Posted by: NuRxG Posted at: 2019-09-11T16:55:27.493Z Reads: 163

```
I was selling them for 15$ I think I would keep the price the same. Not super profitable and kind of annoying to prepare, but I'm only making a few as a service to the community rather than trying to pay my rent.

Last time i sold the kits, i never heard or saw any posts or anything from any of the buyers which was super bummer. I don't know if anyone actually used them, or they're all sitting in peoples "to do" piles. Maybe if i charge more people will actually use them LOL!
```

---
## \#206 Posted by: NuRxG Posted at: 2019-09-11T17:01:34.088Z Reads: 164

```
I might have some code samples of a nano controlling a vesc with self balancing over uart, but id have to dig them up, as i abandoned that route a long time ago. 

Regardless i based my code on this.
https://github.com/erwincoumans/ArduinoServoTxRx/tree/master/VescUart

I switched from UART to PPM and it seemed to be more stable, and i never went back, however i didn't really do extensive A/B testing, so I'm not so confident in that answer. Regardless my current code is worlds better.
```

---
## \#207 Posted by: Fungineers Posted at: 2019-09-11T17:16:05.365Z Reads: 163

```
Was Arduino uart slow/laggy?
```

---
## \#208 Posted by: Surfer Posted at: 2019-09-11T17:22:20.051Z Reads: 170

```
@NuRxG I thought to use this one nrf 52 + bmi160 do you think it can work? I have a vesc 6 and using external gyro, then I can't use Bluetooth module for fine tuning pid, no more UART ports available. (Bmi160 is not firmware ready yet, buy I think it will be soon)
Also there is a forum member who produces a UART splitter module, that could be a solution, but I don't know if that could create noise or any kind of interference on the readings from the gyro.
![Screenshot_20190911-191328|382x500](upload://5eZbCbz3508Ew91lprhaPv9BexR.jpeg) 
Thanks for your input mate
```

---
## \#209 Posted by: NuRxG Posted at: 2019-09-11T17:31:40.952Z Reads: 168

```
It was twitchy and hard to tune, but I can't promise it was due to UART. Ive come a long way since i last tried that method, and rewritten my code 2 or 3 times on different architectures. Every system will have a weakest link, and across my various systems there were many different weakest links.

Some of them being:

flipsky vescs are shit for self balancing

PPM signals are a few MS each

arduino nano cant run at more than like 400hz (use a teensy, way better!)

complementry filters are lame

MPU6050 random drifting biases

VESC time to read and process an input depending on the source (ive never quantified this, and it may not exist)

The gyro library i initially picked had lots of small hard to find bugs that wasted weeks/months of my life

General signal interference/noise on the lines from gyro to arduino and arduino to vesc, I've never quantified this either but electronics people love to talk about it.

The shape and weight of your build.
 
A good example is that i switched from arduino to teensy to run at 1k, but running at 1k made almost no difference when i was controlling over PPM, that was a major defeat and super depressing. However now that I'm running onboard the vesc switching from from 500hz to 1khz made a HUGE difference in stability.
```

---
## \#210 Posted by: NuRxG Posted at: 2019-09-11T17:43:32.994Z Reads: 166

```
Not sure what a combo module gets you, i bought a regular BMI160 but i haven't tested it yet. Is it not in the firmware? I thought it was in the latest release, I've seen a bit of code related to it.

I don't think a UART spitter will work because bluetooth is UART but the gyro is I2C and you probably cant run them both on the same pins at the same time. But that said i have no clue what a UART splitter is.

The upside is that you don't really need to finetune the PID. When everything else is configured properly, it pretty much just works with a wide range of PID values, and the other config is fairly copy pasteable or at least if a then do x. It is pretty involved getting it all set up, i plan to film a proper video once an actual feature set is released, currently is changed quite a bit over the last month. Ive done all my config over USB, i only added the config to the mobile app last night, and i still cant get my trampa vesc working with any of my bluetooth modules.

Here are the gyros i bought (yes i bought a 5 pack LOL)
https://www.amazon.com/gp/product/B07JJHMDR3/ref=ppx_yo_dt_b_asin_title_o00_s00?ie=UTF8&psc=1
```

---
## \#211 Posted by: Fungineers Posted at: 2019-09-11T18:25:14.843Z Reads: 153

```
Yea I burnt a ton of arduinos and mpus. Uart IS glitchy and unreliable..
```

---
## \#212 Posted by: Surfer Posted at: 2019-09-11T18:33:26.804Z Reads: 151

```
I believe you know it, but just in case, the vesc app only connects with nrf and needs to be flased with Benjamin nrf51-52, other apps like vesc monitor will work with a regular hm-10
```

---
## \#213 Posted by: NuRxG Posted at: 2019-09-11T18:47:15.535Z Reads: 152

```
I never heard that. However in the past i could use a flipsky vesc with a flipsky bluetooth controller and connect to the vesc app no problem. I've never used a nrf, ill have to read up on this, or rewrite the code to make it do what i want lol!

Farther down the line, id like to integrate the vesc with an open source mobile app called wheel log.
```

---
## \#214 Posted by: ArTy Posted at: 2019-09-11T19:23:20.210Z Reads: 150

```
Very nice way to make a sensor, you can tell me how thick those plastic sepacers are?
```

---
## \#215 Posted by: NuRxG Posted at: 2019-09-11T20:10:33.436Z Reads: 147

```
I was doing minimum layer height on my 3D printer which was set to 0.3mm, card stock/thick paper works as well.
```

---
## \#216 Posted by: Sc0urge Posted at: 2019-09-13T04:18:06.432Z Reads: 152

```
hey mate, i'm nearly done, had to put it on hold for a bit to help with my sisters wedding.

the only thing left to do in the build is to hook up the 3 wires for the motor drive, as well as the 5 wires for the hall effect inputs

with the peipei hub the  motor power and hall inputs look colour matched. when i'm wiring these into the vesc, does it matters the order that I wire in the hall effect signals? like do they need to be paired with the relevant motor output?
```

---
## \#217 Posted by: Pimousse Posted at: 2019-09-13T07:02:59.533Z Reads: 151

```
[quote="Sc0urge, post:216, topic:80129"]
does it matters the order that I wire in the hall effect signals? like do they need to be paired with the relevant motor output?
[/quote]
No. Everything will be put in order during the sensors detection process in Vesc Tool.
```

---
## \#218 Posted by: Squab Posted at: 2019-09-13T11:51:50.192Z Reads: 143

```
Hello, I'm new to VESC and such, is this compiled firmware for VESC 6+ or it can be flushed to 4.12? How can i check myself, without destroying my hardware? TY)
```

---
## \#219 Posted by: Fungineers Posted at: 2019-09-13T12:02:32.774Z Reads: 148

```
Ok guys I have to admit Mitch has done an exceptional job here. Talked to him yesterday and Im ready to give this a go. I did get Dans firmware and tool downloaded and works good! 
Can anyone please tell me how are the footpads connected on the vesc4? Mitch mentioned they are nrf. Anyone done it?
```

---
## \#222 Posted by: Squab Posted at: 2019-09-13T12:06:30.775Z Reads: 149

```
You just flushed .bin through VESC-Tool as a custom firmware?
```

---
## \#223 Posted by: Fungineers Posted at: 2019-09-13T12:18:04.304Z Reads: 151

```
Yup! Didnt even need a programmer
```

---
## \#224 Posted by: Squab Posted at: 2019-09-13T12:44:04.762Z Reads: 157

```
Well, after flushing Dan's firmware, my hardware version changed to 60 => no worki-worki.
Going to reflush through programmer and hope that it's working at all))
```

---
## \#225 Posted by: Fungineers Posted at: 2019-09-13T13:03:46.008Z Reads: 160

```
I tried through the programmer and it didnt work. Just reflash the custom firmware from the programmer(not Dans). Then go to vesc tool and flash dans fw. HW should be autodetected.
```

---
## \#226 Posted by: Sc0urge Posted at: 2019-09-13T13:27:56.990Z Reads: 170

```
Finished the build and wiring, now i just need to set up the VESC, and maybe modify @MaxGoldenson code to use only one button

[img]https://i.imgur.com/q7zWD0r.jpg[/img]

[img]https://i.imgur.com/MDWD80i.jpg[/img]

[img]https://i.imgur.com/LERnThZ.jpg[/img]

[img]https://i.imgur.com/j9H8JAr.jpg[/img]
```

---
## \#227 Posted by: Squab Posted at: 2019-09-13T13:45:24.500Z Reads: 156

```
What IMU you are using? MPU-9250 does not work (for me)
```

---
## \#228 Posted by: Sc0urge Posted at: 2019-09-13T14:00:10.443Z Reads: 156

```
I've got a nano and an mpu6050 in the box beside the vesc
```

---
## \#229 Posted by: Fungineers Posted at: 2019-09-13T14:06:34.965Z Reads: 159

```
You need a different library for 9250.
```

---
## \#230 Posted by: Surfer Posted at: 2019-09-13T14:13:58.162Z Reads: 158

```
Buddies if you using the firmware from nurgx, there's not need for Arduino, just connect it directly, Benjamin recommend to use a pull up resistors for sda and scl
```

---
## \#231 Posted by: NuRxG Posted at: 2019-09-13T20:02:17.610Z Reads: 163

```
I've tried a bunch of external gyros and vescs without any resistors and they've seemingly worked fine. But obviously benjamin knows way more about this stuff than me, I'm just a software guy.
```

---
## \#232 Posted by: NuRxG Posted at: 2019-09-13T20:09:15.803Z Reads: 167

```
Since it seems so many of you are using the same motor, here is my wheel frame i designed using t-slot extrusions.
![45%20PM|677x500](upload://bC472pKb6jxxpFsHX1BF2qZgK9O.jpeg) 

And here is a photo of it next to Jonathan's infamous monster wheel, which runs the blezalex firmware.
![06%20PM|500x500](upload://da99LkF7y8WaisgKO4JjR1NFxvZ.jpeg) 

The monster wheel now has suspension and runs really well. Im very lucky to live in a city with two other DIY onewheel makers :innocent:
```

---
## \#233 Posted by: Byngham Posted at: 2019-09-13T20:11:30.553Z Reads: 160

```
I don't quite follow what you are saying, Surfer.  Can you clarify for a non-hardware guy?

With the NuRxG firmware, the foot pads connect to sda and scl?  (and how should the resistors be connected in, and what resistance?)
```

---
## \#234 Posted by: NuRxG Posted at: 2019-09-13T20:31:59.939Z Reads: 158

```
The IMU connects to scl/sda, i forget what ports the footpads connect to but if you hit the help icon in the vesc tool it says where.
```

---
## \#235 Posted by: Randy_bobandy Posted at: 2019-09-14T01:04:39.657Z Reads: 160

```
This is sick! We need a video of it in action asap!
```

---
## \#236 Posted by: Sc0urge Posted at: 2019-09-14T02:43:28.746Z Reads: 165

```
for anyone wanting a handle for their deck, i followed this guy, it took about 10 minutes
https://www.youtube.com/watch?v=bHIc5wz3U6o

the cord itself cost me like 4 bucks, and heaps of left over
https://www.ebay.com.au/itm/50-300FT-550-Paracord-Parachute-Cord-Lanyard-Mil-Spec-Type-III-7-Strand-Core/323634927133
```

---
## \#237 Posted by: NuRxG Posted at: 2019-09-14T05:26:50.004Z Reads: 164

```
Here is the info for wiring footpads to the vesc.
![Screenshot%20from%202019-09-13%2022-25-45|690x388](upload://oEL3JrpAIFjYJJkntYEEsuFDPKt.png)
```

---
## \#238 Posted by: MaxGoldenson Posted at: 2019-09-14T05:34:36.433Z Reads: 157

```
What do you mean? what configuration?
```

---
## \#239 Posted by: Fungineers Posted at: 2019-09-14T07:33:07.318Z Reads: 156

```
@Dan333 squab is right. I tried to flash the firware on vesc4 and adter uploading the firmware, the hw version changes to 6 and the balance app doesnt work. Could you please look into this. 
@Surfer any idea?
```

---
## \#240 Posted by: Surfer Posted at: 2019-09-14T07:49:42.572Z Reads: 154

```
Usually this is not good idea, you can blow your vesc flashing the wrong firmware, don't ask me how I know :) 
It was a bit surprise when you said was working for you. 
Just guessing, this firmware is not official, nurgx is working in his firmware for a merge with the official, when this happens will be available for all versions of vesc, but at the moment nurgx is testing with vesc 6 hence the firmware is available for vesc 6.
Anyway Dan mentioned in his post, the version he compiled was for vesc 6, maybe he can compile some more :) if is in the firmware
```

---
## \#241 Posted by: Sc0urge Posted at: 2019-09-14T11:39:04.588Z Reads: 162

```
are there any VESC tool wizzes in the mix? I'm playing round with VESC tool tonight, and getting some good results, but i'm a n00b, so don't want to toast my setup.
the hardware i've got is
10s2p (30Q) battery, with BMS
flipsky vesc 4.12
36v/600w phub wheel

so far in vesc i've set the motor up as FOC with the below current and set voltage cutoff between 34 and 31v

![image|690x357](upload://xOEKbJaxj4Sbz31Bd7rEDEmfm5O.png)
```

---
## \#242 Posted by: Squab Posted at: 2019-09-14T15:40:33.883Z Reads: 158

```
If you interested in testing, I compiled a version of firmware for 4.10 VESC.
Didn't tested it myself, don't have VESC on me right now
https://drive.google.com/open?id=19DMRn7P3SrriZGUhOLUDqNfGufzAOuaa
P.S. It should work with precompiled VESC Tool from Dan but, if it does not, I can rebuild it with one other change, but it is sketchy)
```

---
## \#243 Posted by: Fungineers Posted at: 2019-09-14T16:06:37.193Z Reads: 150

```
Sweet. Will go home and give it a shot tonight.
```

---
## \#244 Posted by: Fungineers Posted at: 2019-09-14T18:31:54.316Z Reads: 157

```
Ok so i flashed this and it seems to work. The hw version is correct (4.1, mine is 4.12, dont know if that makes a difference). 
One thing is that the write app config button doesnt work. Does nothing. I think it might be swapped with the read default app config button. It seems like when i press the read-default config, it writes the app. 
So far so good, but the IMU doesnt seem to be detected by the vesc. At all. I enabled external mpu, Selected 9250, and enables imu RT app, but the reading is just flat...of course, I double checked my connections. 3v gnd and scl sda to same ports on vesc. Still nothing. Could you see what seems to be causing this. @Dan333 @NuRxG 
Off to bed.
```

---
## \#245 Posted by: Fosterqc Posted at: 2019-09-14T18:49:42.292Z Reads: 157

```
Night! May you dream of floating. 
I'm just waking up.

Two Phub 188 are in my future. 

Seems like a Trampa Vesc 6 would be reliable, but I also might want to use higher than 12S voltages. 

https://lunacycle.com/60-amp-36-72v-ebike-bluetooth-programmable-controller/

I wonder how well the Funwheel would work at 72V?

Do I have enough room for 20S? 

Lol nope but I could try.
```

---
## \#246 Posted by: Surfer Posted at: 2019-09-14T22:37:21.898Z Reads: 158

```
First bench test working!! 
Motor has no sensors and dead bearings.

https://youtu.be/vwJ4MKak-tA
```

---
## \#247 Posted by: MaxGoldenson Posted at: 2019-09-15T23:59:05.724Z Reads: 159

```
Hello all, 
I had a question for whoever made the modded software for the vesc. For the foot pads, is it a physical switch that you need, or can I use an fsr. (force sensitive resistor). Also, have any tips for tuning PID (or what worked for you). 
Thanks a lot,
-Max Goldenson
```

---
## \#248 Posted by: Dan333 Posted at: 2019-09-16T07:08:59.534Z Reads: 153

```
yes I only provide version 6 as stated in erlier posts
```

---
## \#249 Posted by: Dan333 Posted at: 2019-09-16T07:09:53.961Z Reads: 152

```
latest commits compiled for vesc 6
https://drive.google.com/open?id=15HlSBt5IpcamOz7tEQY3Lv2KF_ZYmoXe
```

---
## \#250 Posted by: Dan333 Posted at: 2019-09-16T07:12:07.098Z Reads: 148

```
It is made to handle an On/Off switch, but depending on the resistance on the force switch it can work as an open/closed see details in logical 1's and 0's
```

---
## \#251 Posted by: NuRxG Posted at: 2019-09-16T08:39:16.330Z Reads: 153

```
For foot switches it should be open/closed. But I think FSR are fully open with 0 weight. I dont have any "FSR" but i tested a onewheel v1 foot pad and it worked with my code. If youre making velostat sensors follow the build video i linked above and they will function as open/closed as well.

For PID tuning it is less about the pid tune and more about gyro settings. Make sure both the gyro and the app are running at 1khz, set a low madgwick beta 0.01 or 0.02 should be very stable and easy to tune but 0.10 will have a more floaty onewheel feeling. Add a small gyro offset comp on the 2 axis that arnt the balancing axis, a value like 0.05 is ok (this means it will take 20s to correct a gyro being off by 1 degree). Instead of offset comp you can manually calibrate the gyro using the offsets. All gyro axis should be at 0 degrees a second when resting, and acc should all be 0 except 1g in the direction of gravity. It tends to be the gyro rather than the acc that is off.

Once all that is done PID tuning is easy, i use an "I" value of 0, a P value of 5-10 depending on how stiff i want it, and a D value from 60-200 or so to help get rid of twitchyness. 

If you're using a shitty vesc like a flipsky 6.6 it will probably still make a lot of noise and be twitchy even if you tune it well.
```

---
## \#252 Posted by: Fosterqc Posted at: 2019-09-16T08:46:43.517Z Reads: 145

```
Interesting note there about the Flipsky 6.6 preforming poorly. 

Do you only recommend the Trampa vesc 6? 

Is it possible for you to give me an opinion on running the Phub188 on 72v? 

I would not be able to use a VESC for that but if it doesn't work out I'll switch back to a VESC.
```

---
## \#253 Posted by: NuRxG Posted at: 2019-09-16T08:54:59.389Z Reads: 151

```
I haven't done any real A-B testing. but here are my observations.

Switching from flipsky 4.11 to Focbox, when i lean hard it actually moves instead of just making  whining noise and nose diving.

And then maybe 8 months later on a different build.
Switching from flipsky 6.6 to focbox, change of night and day, flipsky had a dead zone when at center so it wouldnt even turn on the motor till you fall off center by more than 1 degree, it was really noisy like cat in heat, and when it started riding it was coggy. The focbox had none of that.

Then about a week later i switched from focbox to a trampa vesc and i didn't notice a ton of difference. Im still blown away that its not screeching all the time tho, its super quiet, with the trampa, but maybe focbox was just as quiet, i don't recall, and the software is now better too.

Trampa vesc is also nice to have built in imu, so you have rx/tx ports free to use bluetooth. Tho i cant seem to get my bluetooth module to work with it.
```

---
## \#254 Posted by: Fosterqc Posted at: 2019-09-16T09:04:36.602Z Reads: 149

```
I'm kinda curious to try a bunch of things out.

I do have a single FOCBOX (honestly my most prized possession) I was going to use for a board but getting another one is hard and I need dual motors now. 

I want to make two Onewheels for cheap ish so I could take people out for rides. They don't have to match so maybe FOCBOX in one on 12S and make the second one a higher voltage.

I do have the budget for two VESC 6 plus though so maybe just two with those on 12S would be fine. (Focbox would go into some other cool electric shit)

You can see how I'm not sure what I should do.

No rush for this project I will have the hubs in ~2 months. That's enough time for the MotherFOCer or some other cool ESC to come out.
```

---
## \#255 Posted by: NuRxG Posted at: 2019-09-16T09:09:51.518Z Reads: 149

```
As for my opinion on the Chinese motors, run them as high voltage with as many amps as you can shove at them, if they start getting actually really hot then dial it back a bit, or ride on colder days, or melt it to the ground and buy a beefier chinese motor :smiley:

If you guys a DIY building to save $ you're doing it wrong, run everything as overpowered and as dangerously as you can :fire: 

As a side node my motor seemed to have no problem with 1000w. But id rather give it 3000w if i could, i dont have space for that many batteries in my build tho, and im running out of batteries LOL! :crying_cat_face:
```

---
## \#256 Posted by: Byngham Posted at: 2019-09-16T19:28:54.927Z Reads: 138

```
NuRxG--  what motor do you recommend, if not one of the chinese ones?  I'm currently building one with the phub 188.  When we burn that out, or want to do a 2nd iteration, what would you recommend?
```

---
## \#257 Posted by: NuRxG Posted at: 2019-09-17T00:49:58.724Z Reads: 135

```
I don't know, I'm not a motor guy, I'm a send it guy! Whatever motor you have, turn it up! :fire:

Joking aside my main gripe with the phub is the dimensions, the 5.5" diameter means you cant get any nice tires for it. I have a china motor with a 6" diameter i bought about a year ago but it is slightly narrower and i never built a frame for it. It also claimed to be rated for 1000w, so that probably means i need to run it at 4000w :joy::joy::joy:
```

---
## \#258 Posted by: Fosterqc Posted at: 2019-09-17T02:00:31.730Z Reads: 136

```
There is at least one person in this thread using the Hoosier treaded wheel and a belt drive. In theory it should work just as well or better given the greater power and torque. You could also try to make your own Direct drive, if you feel like finding a low low KV motor.

The Phub offers a very clean solution with arguably enough power at 12S. I still think its true potential would be unlocked with 15S-20S.

also its pretty damn cheap
```

---
## \#259 Posted by: MaxGoldenson Posted at: 2019-09-17T02:50:26.814Z Reads: 131

```
@NuRxG what do you mean by " . Make sure both the gyro and the app are running at 1khz, set a low madgwick beta 0.01 or 0.02 should be very stable and easy to tune but 0.10 will have a more floaty onewheel feeling"? what is "madgiwick"?
```

---
## \#260 Posted by: NuRxG Posted at: 2019-09-17T02:51:13.328Z Reads: 134

```
its an option on the IMU page.
```

---
## \#261 Posted by: MaxGoldenson Posted at: 2019-09-17T02:58:15.849Z Reads: 139

```
thanks I was looking for it.
```

---
## \#262 Posted by: MaxGoldenson Posted at: 2019-09-17T03:22:38.652Z Reads: 142

```
@NuRxG One last question, can you re-send the link to the video? or was it the one what you posted a while back?
Thanks
```

---
## \#263 Posted by: MaxGoldenson Posted at: 2019-09-17T04:06:07.885Z Reads: 146

```
@NuRxG what gyro is the vecs mod designed for? Will it work with mpu 6050?
thanks again
-Max
```

---
## \#264 Posted by: Surfer Posted at: 2019-09-17T18:08:32.697Z Reads: 141

```
Yujuuuuu!!! Balance function is officially merged congrats @NuRxG!! Thaaanks!
😁😁🥰🤪🤩
```

---
## \#265 Posted by: NuRxG Posted at: 2019-09-17T19:39:11.938Z Reads: 139

```
Should work with any gyro supported by the vesc firmware. MPU6050 is not one of the listed gyros but i believe it actually works under the 9250 setting.
```

---
## \#266 Posted by: NuRxG Posted at: 2019-09-17T19:46:49.839Z Reads: 141

```
Woah! i saw this comment here first!

This is the greatest moment in my life, and i just like to say...

I drew that EUC icon myself, Immortalized in the GUI forever, EUC MASTER RACE! SUCK IT ONEWHEELERS!!!

:joy::joy::joy::joy:

I'm pretty stoked, now i gotta film an instructional video.
```

---
## \#267 Posted by: Fungineers Posted at: 2019-09-18T03:01:15.874Z Reads: 136

```
Dude! This is awesome!
Congratulations. No more fried arduinos trying to control onewheels anymore thanks to you.
```

---
## \#268 Posted by: MaxGoldenson Posted at: 2019-09-18T05:19:45.360Z Reads: 148

```
Congratulations @NuRxG,

Also I have modeld out the spacer for the foot pads, this is a 3d printable file. 

https://github.com/GAM3TIN/Foot-pads
```

---
## \#269 Posted by: NuRxG Posted at: 2019-09-18T08:09:41.253Z Reads: 152

```
Setup tutorial:

https://youtu.be/0y5ME2SgwLg
```

---
## \#270 Posted by: zorglups Posted at: 2019-09-18T13:39:24.164Z Reads: 144

```
Thank you so much @NuRxG  !!!
I’m following this thread since a few weeks in the hope of building on OneWheel with my son. 
I’m not sure I understood a third of it but this will definitely help !
Thank you for your time and work !
```

---
## \#271 Posted by: Sindre Posted at: 2019-09-18T16:06:49.490Z Reads: 146

```
Sweet man, will def give this a try!
```

---
## \#272 Posted by: Khurtana Posted at: 2019-09-19T04:37:16.466Z Reads: 146

```
Can't see a IMU sensor base orientation?  Am I missing something?
```

---
## \#273 Posted by: sayekim Posted at: 2019-09-19T09:51:51.162Z Reads: 145

```
Next VESC 6 firmware will have self balancing feature. 

https://forum./t/vesc-wand-remote-soon-to-arrive-from-the-future/630/327?u=sayekim
```

---
## \#274 Posted by: NuRxG Posted at: 2019-09-20T17:30:47.227Z Reads: 138

```
The rotation subsection in the IMU config page lets you set your base orientation.
```

---
## \#275 Posted by: Sc0urge Posted at: 2019-09-22T11:44:44.870Z Reads: 140

```
quick question on how not to die.

i've got the arduino sending pwm to the vesc, and it all acts as it should, the only thing is that it seems to go from 0 to breakneck speed pretty fast, and i think if i was standing on it i'd fall on my butt.

i've got the max motor current set as 20A turned the throttle curve way down into negatives, is there anything else to look at, what control type are people using successfully (current, current no reverse etc?)
```

---
## \#276 Posted by: Surfer Posted at: 2019-09-22T11:50:10.641Z Reads: 137

```
This happens because there is no load, is normal
```

---
## \#277 Posted by: Fungineers Posted at: 2019-09-23T06:18:04.534Z Reads: 133

```
It will behave like that on the bench if you are in current mode (no load). Once you ride it, it will ramp up speed normally depending on the load; so this is pretty normal. Just go and ride ;)
If you really want to check if the ramp up is correct, choose duty cycle mode, then it will ramp up in proportion to your angle. Just run duty cycle if you want to test it on the bench.

You want to run either current or duty cycle. You dont want to run the 'no reverse' modes on a Onewheel, would you?
```

---
## \#278 Posted by: Sc0urge Posted at: 2019-09-23T10:21:15.585Z Reads: 130

```
true, i didn't realise what i was thinking of was standard 'current' behaviour, where it's "The output is off when the input is centered. Input less than center brakes until the motor stops, at which point it it starts in the reverse direction."
```

---
## \#279 Posted by: Remieknaapen Posted at: 2019-09-25T08:03:27.603Z Reads: 136

```
Did someone manage to get a FOCBOX working with external MPU6050?
When I flash my vesc with Dan333 the MPU works but the hardware version is wrong and I can't get the motor to work.

Using a compiled versions from Squab (balance_4.10.bin) i do get the motor to spin up but my MPU6050 doesn't work.
```

---
## \#280 Posted by: Sindre Posted at: 2019-09-25T09:24:52.362Z Reads: 130

```
Isent the focbox based on the vesc 6.6 hardware? Using the v4 code could destroy the esc
```

---
## \#281 Posted by: Remieknaapen Posted at: 2019-09-25T09:58:55.870Z Reads: 134

```
Focbox is based on 4.12 hardware. With some small differences in components from what i have read. So v4 should just work. But i can't ge the mpu to respond.
```

---
## \#282 Posted by: Surfer Posted at: 2019-09-25T11:37:09.829Z Reads: 142

```
I try with 9250 and works well but 6050 I can't make it work on first try on a vesc 6

Edit: both imu are working here
```

---
## \#283 Posted by: Jopj Posted at: 2019-09-25T23:28:17.874Z Reads: 144

```
I'm making a DIY onewheel too so decided to post that here!

![P_20190924_002303_vHDR_On|670x500](upload://tOjQXlTNco6cGAPUaEU0aKmQMko.jpeg) 

It uses a phub-188 motor, the original FOCBOX, a trio of MPU9250:s for redundancy and a Teensy 3.6 for running the control software. I'm adapting my old rc-plane autopilot code for it, the poor thing thinks it's flying a weird plane that only has ailerons :smile:

Control box is quite crowded, there's a Flipsky antispark switch to turn the FOCBOX off to prevent it draining the battery.

The battery is also DIY, 10S3P of LG INR18650-M29 cells and a Daly BMS in a printed enclosure.

I'm experimenting with making Velostat sensors with conductive copper tape, and I'll certainly take a good look at the already known working ones posted here. Mine work, but I'm worried about long term stability and how to seal it in laminate without melting the velostat. I'm also thinking about using strain gages in the frame instead of the resistive sensors, that might be a solid option.

Lots of work still to do, but it'll run soon, I hope!
```

---
## \#284 Posted by: Jopj Posted at: 2019-09-25T23:31:54.802Z Reads: 144

```
![P_20190925_214345_vHDR_On|669x500](upload://g73nELOk28Mhw41cqMpfsFmQpdW.jpeg) 
Aluminum profiles are nice in that the grooves can be used to run cables between the control box and battery compartment. I made some effort to make both waterproof, or at least more water resistant, with seals in both boxes and supposedly IP68-rated connectors from Aliexpress, which actually do feel quite good.
```

---
## \#285 Posted by: Jopj Posted at: 2019-09-25T23:36:39.930Z Reads: 144

```
![P_20190723_164923_vHDR_On|670x500](upload://zTHDbrssqGGEvd3Ot7ofBctddGC.jpeg) 
I tested the battery by running my previously built e-scooter with it and cruising around with the front disk brake engaged... I didn't have a proper load so that had to do. Battery did great with a 1000W torture test, dual 0.15mm nickel strip spot welded with the usual arduino + car battery contraption and strengthened with some copper wire did the trick. Cells getting hot is the limiting factor
```

---
## \#286 Posted by: sesat Posted at: 2019-09-25T23:39:50.035Z Reads: 143

```
Very nice :slight_smile:

Why did you choose to make your electronics box just-big-enough, instead of having it encompass that entire space, rail to rail?
```

---
## \#287 Posted by: Jopj Posted at: 2019-09-25T23:41:11.005Z Reads: 144

```
![P_20190923_234914_vHDR_On|670x500](upload://z2l6uFwfxTSPMTEj1iCvgGMciNp.jpeg) 
My previous build was a bit rough, a long range e-scooter. While that works, I'm trying to put some more effort into making this thing "right. Afterall, if something fails I'll instantly eat asphalt and I'd rather not :no_mouth: This thing has seriously loud tweeters and I'll use those to alert if motor is approaching speedl imit, battery gets low, current approaches limits, temperature gets high or anything that would cause issues. I was a bit iffy on the pushback after trying the commercial onewheel so I chose audio.
```

---
## \#288 Posted by: Jopj Posted at: 2019-09-25T23:43:23.327Z Reads: 146

```
![P_20190926_003325_vHDR_On|670x500](upload://l9jPRmzrzQjdpMRb2LYh7JP21DK.jpeg) 
The steps in the rear are to have space for the connector, especially the motor-encoder combo one is quite big. I'd love to have a bit more space in there, but luckily everything fits as is.
```

---
## \#289 Posted by: zorglups Posted at: 2019-09-26T19:39:21.474Z Reads: 143

```
@Jopj : Your setup is awesome !
I hope you get to ride it soon and I hope you write down your BOM, give plans, schematics and code 😋
```

---
## \#290 Posted by: Giga Posted at: 2019-09-27T09:42:02.271Z Reads: 140

```
Are you using CAN or Uart?
```

---
## \#291 Posted by: NuRxG Posted at: 2019-09-27T15:41:22.917Z Reads: 138

```
VESC tool 1.20 is out with the balance app in it! 🎉

WE DID IT!!!!
```

---
## \#292 Posted by: Surfer Posted at: 2019-09-27T16:26:26.293Z Reads: 132

```
Yuuujuu!! Experimental!!! :) :)
```

---
## \#293 Posted by: NuRxG Posted at: 2019-09-27T16:32:08.405Z Reads: 133

```
I prefer the term maverick :crazy_face:

Now that it is out, if anyone is still using external controllers for reasons other than lulz/wanting to roll their own. Please let me know what the app is missing, or even better, add it to the vesc yourself, its open source! I know the app is not perfect, but I think can get closer to a perfect app if we don't all start from 0.
```

---
## \#294 Posted by: Surfer Posted at: 2019-09-27T16:41:45.090Z Reads: 126

```
Like maverick! Hoping one day surfing it!!

Experimental comes from the channel log :)
```

---
## \#295 Posted by: Jopj Posted at: 2019-09-28T10:28:45.747Z Reads: 132

```
Eventually can, I put a can transceiver on the board in anticipation. But uart has to do for now, I don't know of any CAN vesc control libraries and I want to get the rest done before making my own.
```

---
## \#296 Posted by: Jopj Posted at: 2019-09-28T10:38:22.233Z Reads: 133

```
Very cool! I might have used this had I waited a bit, that'd be some space saved in the control box..
```

---
## \#297 Posted by: Jopj Posted at: 2019-09-28T12:09:45.905Z Reads: 133

```
What is the thickness of the velostat used there? I've found my sensors tend to have very low resistance and be hard to measure unless I stack 3-8 layers of the stuff. Maybe mine is thinner?
```

---
## \#298 Posted by: NuRxG Posted at: 2019-09-28T18:14:38.204Z Reads: 137

```
I don't think they sell multiple thicknesses, it's the spacer that does all the magic. Mine is pretty low resistance as well.
```

---
## \#299 Posted by: Surfer Posted at: 2019-09-29T09:08:58.053Z Reads: 139

```
First test ride with @NuRxG firmware!! 
At the moment is just barely rideable, have to understand well the settings and play more with them, but guys this is promising!!!
https://youtu.be/1CmvzBAr_gc

![IMG_20190928_234132|250x500](upload://qW6OebMEqWVUtNh6J7Clm4xpK7y.jpeg)
```

---
## \#300 Posted by: Byngham Posted at: 2019-09-29T23:51:03.932Z Reads: 128

```
I've got my build assembled to the point that I'm trying to test out the components together for the first time.6plus.

I've got a phub188 chinese motor and a VESC 6plus.  The vesc is able to move the wheel, though i'm not sure that it's recognizing the sensors.

My real problem is that I can't seem to get the VESC tool to get the gyro IMU data from the VESC 6 plus.  I've got the App to Use switched from UART to Balance, and the IMU Tyoe is set to IMU_TYPE_INTERNAL.  However, I'm not getting any data in the graphs of IMU data-- no lines at all.

Any thoughts on what I've done wrong?

Thanks.
```

---
## \#301 Posted by: NuRxG Posted at: 2019-09-30T04:52:44.587Z Reads: 132

```
It doesn't sound like you are doing anything wrong, the internal gyro should show data regardless of what app you're using.

Id guess it is a vesc6 and not a vesc6+ or maybe it is busted. Perhaps try using an external gyro :sob: ?

**edit** did you check the realtime IMU data box on the right hand column?
```

---
## \#302 Posted by: trampa Posted at: 2019-09-30T16:06:41.406Z Reads: 127

```
Switch on **IMU data** in right menu bar.
```

---
## \#303 Posted by: Fosterqc Posted at: 2019-09-30T20:02:20.371Z Reads: 130

```
Lol can I commend you for your excellent support to the community. :man_technologist:
```

---
## \#304 Posted by: ducktaperules Posted at: 2019-09-30T20:57:03.904Z Reads: 132

```
these enclosures look awesome. are they 3d printed? what do you use for the seals?
```

---
## \#305 Posted by: Jopj Posted at: 2019-09-30T23:26:14.550Z Reads: 137

```
Yep, printed with a groove for 1mm silicon seal, kinda like o-ring stuff but comes in an endless roll instead. You cut it to length and join the ends with CA

Just got the sensors + griptape installed! Also managed to "ride" a couple of meters without the sensors hooked up by being on my knees and holding the faceplate button as a substitute.. awkward but a start!
![P_20190930_215156_vHDR_On|670x500](upload://siSJC1wpL6XH12xUClD6FB8roKY.jpeg) 

The sensors before mounting. I'm a bit worried about how they'll hold up to being stood on and the twisty motions they need to endure while riding. They are about 0.5mm thick, maybe I should have milled a depression that deep for them so that they won't take all of the pressure, but that might have impeded their function. The construction is very similar to the ones found in this thread (nice design!), but with overlapping tape instead of a single copper sheet and wrapped in contact plastic of the book covering sort.
![P_20190930_193532_vHDR_On|670x500](upload://hslZjdynLsP6XWqVBKb3tRei9f1.jpeg)
```

---
## \#306 Posted by: Jopj Posted at: 2019-09-30T23:44:29.370Z Reads: 133

```
You can make sure it's detecting the sensors by choosing a sensored drive mode and giving it some power. If the sensors have not been detected right, it'll just scream and twitch. If it runs, sensors work. There should also be a hall sensor table in one of the tabs with differing numbers in them, if it's all -1 or 255 then detection has failed. I have the same exact motor as you and my focbox detects the sensors fine, so there should be no problems if it's wired right.

On a related note, I wonder why my motor is so loud in FOC. It has this warbling whining/ringing noise that's fairly loud. Motor runs great, just sounds like a sad raccoon. Changing switching frequency randomly changes the pitch (sometimes higher freq makes lower pitch noise..) but doesn't make it go away. Looking at the spectrum there's not even any noticeable peaks, just a wall of noise. I'm confused, FOC is supposed to be quiet right?
```

---
## \#307 Posted by: NuRxG Posted at: 2019-09-30T23:55:41.453Z Reads: 128

```
Im guessing your vesc is flipsky or a v4?
```

---
## \#308 Posted by: s.white432 Posted at: 2019-10-01T01:04:09.725Z Reads: 127

```
I'm interested in getting the PHUB-188, but was wondering if replacement tyres are available? As far as I'm aware, 5.5 inch hubs are not common for go-karts.

Peipei have advised that they can sell a spare tyre with the motor, but don't sell the tyres separately.
```

---
## \#309 Posted by: Fosterqc Posted at: 2019-10-01T04:27:41.819Z Reads: 122

```
Hmm I'm not sure it matches the Onewheel+/XR exactly, so the Hoosier tire probably wouldn't fit. 

I'm sure China has what you want... Wether you can find it is the question.
```

---
## \#310 Posted by: Jopj Posted at: 2019-10-01T08:58:38.820Z Reads: 121

```
It's a focbox, so 4.12 based
```

---
## \#311 Posted by: NuRxG Posted at: 2019-10-01T09:07:09.896Z Reads: 124

```
OK that is weird, my focbox is fairly quiet. My flip sky vesc6 sounds like a cat in heat.
```

---
## \#312 Posted by: Jopj Posted at: 2019-10-01T09:30:55.115Z Reads: 129

```
Oddly enough I have a flipsky 6.6 too on my scooter, and that's dead quiet in foc. It just starts tripping on abs overcurrent at 80 amps so I use bldc to get over that. Strange things.
```

---
## \#313 Posted by: Jopj Posted at: 2019-10-01T10:02:16.151Z Reads: 132

```
They do sell the tyres for phub-188 separately, here: https://m.aliexpress.com/item/32953994078.html?pid=808_0000_0101&spm=a2g0n.search-amp.list.32953994078&aff_trace_key=2ee0d0d80c814dddbb9af058e898b15f-1558100630648-02513-UneMJZVf&aff_platform=msite&m_page_id=863amp-DQS_bwZUW01PQ2exG26OtQ1569924038201

There's also another motor now available that has a higher power rating of 800W, same tire size as phub-188. Looks to need a wider mounting as the motor is bigger and there's a disk brake mount. https://m.aliexpress.com/item/33050869219.html?trace=wwwdetail2mobilesitedetail&gps-id=platformRecommendH5&scm=1007.18499.139690.0&scm_id=1007.18499.139690.0&scm-url=1007.18499.139690.0&pvid=2e33917f-019c-4f89-a3f5-f9134b94de92&_t=gps-id:platformRecommendH5,scm-url:1007.18499.139690.0,pvid:2e33917f-019c-4f89-a3f5-f9134b94de92&spm=a2g0n.detail-amp.moretolove.33050869219&aff_trace_key=2ee0d0d80c814dddbb9af058e898b15f-1558100630648-02513-UneMJZVf&aff_platform=msite&m_page_id=3093amp-DQS_bwZUW01PQ2exG26OtQ1569924468650
```

---
## \#314 Posted by: Khurtana Posted at: 2019-10-01T10:40:40.031Z Reads: 121

```
This looks interesting.  Which phub188 did you buy for your ewheel?
```

---
## \#315 Posted by: Jopj Posted at: 2019-10-01T11:00:05.036Z Reads: 121

```
I used the 24v 600w version. My battery is 10s but this way I can push higher momentary peaks to help balance better.
```

---
## \#316 Posted by: NuRxG Posted at: 2019-10-01T15:19:21.717Z Reads: 125

```
I have that 2nd motor but I never built a frame for it. A local friend here has one and a frame for it but never got a tire working, he tried a Vega. I may give him my tire but I don't think it will fit his frame.
```

---
## \#317 Posted by: Byngham Posted at: 2019-10-02T01:10:42.419Z Reads: 129

```
NuRxG and Trampa--  The realtime IMU button on the right was what I was missing.  Hadn't realized it was there.  Thanks for that tip!!

Now, I'm trying to deal with the Hall sensors.  I've try to have them detected, but am getting a message of "Bad FOC Hall Detection Result Received"  I've wired the connections from the Phub188 to the VESC6+ as best I can figure--  green and black from the Phub to the same on the VESC (V+ and gnd), then the other 3 from the phub (red, yellow, blue) to the VESC H1, H2, and H3.

Can anyone spot where I would have gone wrong?  Why aren't my hall sensors being detected?

Thanks for any advice people can offer.  You've really been great!!
```

---
## \#318 Posted by: MysticalDork Posted at: 2019-10-02T05:57:57.076Z Reads: 126

```
@Byngham  Try red as positive, black as ground, and green, yellow, and blue as H1/2/3. (I've never seen red be anything but positive/vcc in a hall sensor setup.)
```

---
## \#319 Posted by: Jopj Posted at: 2019-10-02T07:40:47.607Z Reads: 122

```
Yep, as MysticalDork said. Green, blue an yellow are the sensors, red is v+ and black is gnd. Wire it like that and it'll detect them right away granted they didn't get burned.
```

---
## \#320 Posted by: Remieknaapen Posted at: 2019-10-02T08:01:08.009Z Reads: 131

```
Installed the new software last weekend and got everything running including velostat footpad sensors.
Now all of the sudden without changing anything on the hardware or software one footpad stopped working, at least that is what I thought. So i switched the wires from sck-adc1 to adc2-miso and visa versa to check if my footpads where still oke. Conclusion is that the footpads are still oke but the sck-adc2 port doesn't react or receive input when putting 3v on it? Does any of you have a clue of what could be the problem?
```

---
## \#321 Posted by: Byngham Posted at: 2019-10-02T15:38:13.714Z Reads: 122

```
Thanks MysticalDork and Jopj for the feedback.  I'd simply matched the colors from the connector to the colors from the phub188.  Hadn't occurred to me that the connector likely wasn't made to the same specs as the sensors on the motor, but it makes sense.  I'll be wiring that up tonight, and will report back.
```

---
## \#322 Posted by: NuRxG Posted at: 2019-10-02T18:35:24.418Z Reads: 121

```
What hardware version are you using?

I don't have any solution, just curious.
```

---
## \#323 Posted by: Remieknaapen Posted at: 2019-10-02T18:40:27.653Z Reads: 123

```
I'm using focbox, hardware version 4.12 if i'm correct. Is there any way i would be able to assign the footpad to another input channel, or maybe ditch one footpad and only use adc2 miso as footpad sensor input?
```

---
## \#324 Posted by: Fungineers Posted at: 2019-10-02T19:02:23.325Z Reads: 127

```
It would be great if @NuRxG or some other smart person could do a separate tab for each footpad on the app. Like footpad 1 and footpad 2. That way even if one footpad doesnt work its not a total loss and would still work. Or maybe as @Remieknaapen said, have the ability to aasign other pins as footpads. That would be really siiiick.
```

---
## \#325 Posted by: Jopj Posted at: 2019-10-02T21:06:11.008Z Reads: 128

```
https://giphy.com/gifs/gdqRfeW2r5TUyQSs7Y
It works!
```

---
## \#326 Posted by: Surfer Posted at: 2019-10-02T21:10:30.497Z Reads: 126

```
This spring effect!!! Seems to put the beta up on the madgwick settings helps. :)
```

---
## \#327 Posted by: Jopj Posted at: 2019-10-02T21:14:03.254Z Reads: 125

```
I'll keep that in mind. I feel most of the sponginess now is due to the control being super loose. The algorithm also is basically throttle=angle*constant  for now :)
```

---
## \#328 Posted by: NuRxG Posted at: 2019-10-02T21:54:29.738Z Reads: 125

```
It's not so simple to use different pins. I wanted to use the can pins initially but those wouldn't work. I would think any pin can be converted to a digital i/o but perhaps other parts of the vesc firmware are using the pins and fighting me. There are other pins that can work, but then they cant be used for other things, so there is always a tradeoff.

In general the config is already massively complex, and I'm trying to keep it simple. My thinking was that if someone wanted to use just a single footpad you could wire both pins to the single footpad. That of course wont help if the pins don't work. It would be nice to have it configurable, but creating a more confusing setup to accommodate damaged VESCs doesn't seem like the best idea. 

I have a focbox at home, i can test the pins on the latest firmware and see if it works. If it is all good on my focbox, i think the best thing is to modify and build the firmware yourself, its fairly trivial to change the pins, i can show you where. If you can't do that, i can mod it for you and give you a build, but i wont be suppling build till the end of time.
```

---
## \#329 Posted by: NuRxG Posted at: 2019-10-02T22:03:02.052Z Reads: 123

```
Also after testing on a few builds, i can confirm

* EUC: Beta=0.02
* Skateboard: Beta=0.10

These settings give the feeling you want. But by all means please test and tweak and see what works for you. Also be careful raising the beta as it can get real twitchy if you go too high. starting at 0.04 and working up to 0.10 is the smart/safe way to do it.

A good way to test stability is to get it running without a human on it while holding it with one hand, and then bash the tire and see what happens :smiley: if it is ok go for rapid successive bashes :smiley:  if it is still ok, ride it down a flight of stairs and see if it twitches :wink:
```

---
## \#330 Posted by: Remieknaapen Posted at: 2019-10-03T06:08:58.322Z Reads: 121

```
If you are willing to test some other pins on the latest firmware and try it out on your focbox that would be great!! I think i can manage to change the pins if you can show me where to do it.
```

---
## \#331 Posted by: NuRxG Posted at: 2019-10-03T08:16:48.827Z Reads: 129

```
:confounded: This is turning out to be more annoying than it should be. I was hoping it would be as simple as wiring to ADC3, but the vesc4 doesn't have an adc3. So....

Looking at a focbox, there are really only 4 unused pins, the 2 can pins, the ppm signal pin, and the hall sensor temp pin (china motors don't tend to have that sensor). None of these seem especially hopeful, my guess would be the ppm signal or motor temp pins, but try all 4 if you can. I would test for you, but the focbox doesn't have SWD port for flashing with an stlinker making it a pita to test things.

To make the change, you need to change both the **port** and the **pin** in 2 places.

First [here](https://github.com/vedderb/bldc/blob/master/applications/app_balance.c#L105) it is configured to be pulldown. Then [here](https://github.com/vedderb/bldc/blob/master/applications/app_balance.c#L204) it's value is read in each iteration of the control loop.

The ifdef statements can be ignored, they're there to disable footpads on hardware(s) that don't have the pins at all.

Now for what to change it to, there are 3 options.

**Easy Mode**: Look in the [hwconf](https://github.com/vedderb/bldc/blob/master/hwconf/hw_410.h) for port/pin and use the constant values. Tho i looked and i don't see any of these. So maybe this isn't easy.

**Hard Mode**: Look at the wiring diagrams & datasheet and figure out what gpio and pin number to use and set it explicitly.

**Cop Out**: Change both sensor pins/ports to be the working pin/port, and live with a single sensor setup. This one at least is easy.

Sorry this turned out to be way more of a pain than it should be.

P.S. I tested the 1.20 firmware on my focbox and both sensor pins worked fine.
```

---
## \#332 Posted by: Remieknaapen Posted at: 2019-10-03T12:14:51.264Z Reads: 122

```
Thank you so much for your help! Think I'll first try and get the temp pin to serve as input pin for my footpad. Not really good at writing or editing code but it looks like a good challenge to me.

I will let you know if it works !
```

---
## \#333 Posted by: Surfer Posted at: 2019-10-04T11:57:30.096Z Reads: 128

```
Hi Pimousse, if i remember right when it was the the time for purchase Escape vesc you where the only one who did ask stewii to populate the IMU in your vesc, is that right or my mind mixed persons? :slight_smile: if so, I would like to ask if you can make a picture where the IMU lies.
I populate my vesc with the IMU but still doesn't work, I think there is some missing resistors around it, picture coming..![IMG_20191003_223615__01|250x500](upload://1OgiMiR5xALp9v9Kylyby8XmafT.jpeg) 
Appreciate your help, thanks mate!!!
```

---
## \#334 Posted by: Pimousse Posted at: 2019-10-04T12:13:44.564Z Reads: 124

```
I don't remember a request, but perhaps it was me.
What FW do tou use your ESCAPE with ?
No FW have been developed for using the embedded IMU on HW6 design.
The IMU has been moved of MCU pins on the VESC 6+.

So unless you write a custom FW for your ESCAPE, that won't work.
```

---
## \#335 Posted by: Surfer Posted at: 2019-10-04T12:18:19.386Z Reads: 121

```
I'm running 3,62 official vesc firmware, I though maybe will work :( since the balance thingy was implemented.
My code skills tops at hello world! 😭😭.
Thanks anyway!!🤩
```

---
## \#336 Posted by: Byngham Posted at: 2019-10-04T19:06:18.335Z Reads: 122

```
Because of all the helpful advice so far, my son and I have our build still moving along well.  The fix to our Hall sensors see to have resolved it, and the Vesc software are now recognizing it.

Our next task is to work out the foot pads.  I've modeled up and printed out a pattern similar to what NuRxG posted, and have the rest of the materials.  My question at this point is about wiring it up.  If I remember correctly, the help in the Vesc Tool software indicate to connect 3.3v to ADC1 and ADC2 for the two foot pads.  I see connections labeled for providing 5v (like at the bottom of the "COMM" block of connectors on the VESC 6+)  Where do I get 3.3v?  

Thanks for any advice you can give.  I really appreciate it!!
```

---
## \#337 Posted by: NuRxG Posted at: 2019-10-05T02:55:50.009Z Reads: 111

```
The the vesc6+ it is labeled vcc, its right between 5v and gnd.
```

---
## \#338 Posted by: Squab Posted at: 2019-10-05T08:34:40.921Z Reads: 116

```
So, can someone explain to me how this board should behave when I’m holding it under load? If I understand correctly it should try to keep the IMU level, changing direction quite often? Coz my build right now just going forward full throttle, does not change direction if I’m lifting nose up, hence it’s not a self balancing board right now (I’m using flipsky fsesc 4.12 and imu9250, motor is phub-188)
```

---
## \#339 Posted by: NuRxG Posted at: 2019-10-05T08:37:04.697Z Reads: 115

```
Its probably running backwards, you can switch it by changing your motor direction, or physically rotating your gyro 180, or software rotating your gyro 180.
```

---
## \#340 Posted by: Squab Posted at: 2019-10-05T08:44:30.534Z Reads: 115

```
I thought so myself and tried it already, it just changes direction, behavior is the same, just backwards. 
My question is, how should it behave normally? What should I expect when I’m testing it
```

---
## \#341 Posted by: NuRxG Posted at: 2019-10-05T09:03:42.575Z Reads: 112

```
It should balance.

When it is unloaded, can you get the wheel spinning in both directions by moving the gyro?
```

---
## \#342 Posted by: Squab Posted at: 2019-10-05T09:23:35.231Z Reads: 114

```
But it turns off without load. How can I turn off this feature?
```

---
## \#343 Posted by: NuRxG Posted at: 2019-10-05T09:24:35.826Z Reads: 114

```
Overspeed -> Cutoff Duty Cycle = 1

But once you do this the wheel wont turn off without unplugging it. *if you dont have switches wired up*
```

---
## \#344 Posted by: Remieknaapen Posted at: 2019-10-05T14:18:10.978Z Reads: 117

```
Got the 'cop out' mode working!

Going to wire the two footpads in serie so that i still have two physical pads that have to be pressed to turn the board on. Wil try the hard mode in the future, but for now cop wil work just fine. Thanks!
```

---
## \#345 Posted by: Squab Posted at: 2019-10-05T15:50:22.223Z Reads: 119

```
Ty for your help. I think I solved my problem... I was trying balancing by Roll Axis and didn't notice that it is not possible. On the first release of self balancing app there was an option to set up main axis, but now it's gone(
```

---
## \#346 Posted by: Fungineers Posted at: 2019-10-05T17:48:02.469Z Reads: 123

```
Yea @NuRxG mentioned that the option to balance on roll might go in the future, so now it's only pitch. 
Thats why I built my pcb this way:
![IMG_20191002_190217_182|500x500](upload://j0gqEBHSURuwRGRqRdONTqOmvpl.jpeg) 

Cool thing about this pcb is that its the same dimensions as the vesc and the holes match up, so you can just stack it on top of the vesc with standoffs and connect footpads to it and imu on top. I will release it soon once im done replacing my burnt stm chip on the vesc lol. 
Btw heres my first ride before I shorted and killed the stm, if you guys havent seen this already: 
https://youtu.be/HaAcMH4hEHc
```

---
## \#347 Posted by: tubular Posted at: 2019-10-05T17:51:07.291Z Reads: 119

```
Sorry if this was mentioned somewhere, but I can't seem to find it.  Whats the wiring layout from the MPU6050 to the VESC?  I have the VESC 4.12.  Thanks for your help.
```

---
## \#348 Posted by: Surfer Posted at: 2019-10-05T19:01:40.513Z Reads: 120

```
Here is how i connected:

Vcc to vcc or 5v

Gnd=gnd

Scl=scl

Sda=sda
```

---
## \#349 Posted by: tubular Posted at: 2019-10-05T21:08:43.333Z Reads: 122

```
My VESC doesn't seem to have many of those. It's a Flipsky, so I got...

5V, TMP, H1, H2, H3 : USB : CAL, CAH, 5V : 5V, 3.3V, ADC, TX, RX, ADC2 : NC, RST, DIO, CLK, 3.3V.

MPU6050 -> VDD, GND, INT, FSYNC, SCL, SDA, VIO, CLK, ASCL, ASDA
```

---
## \#350 Posted by: ChrisW Posted at: 2019-10-05T21:43:31.983Z Reads: 119

```
[quote="Sindre, post:1, topic:80129"]
Thinking of dooing the pid controlling in the vesc6, and need to convert pwm signal to ppm to make the code work.
[/quote]

VESC6 uses PWM, not PPM, but mislabels it as "PPM".
```

---
## \#351 Posted by: Squab Posted at: 2019-10-06T09:45:56.973Z Reads: 116

```
Scl = Rx
Sda = Tx
```

---
## \#352 Posted by: SwarleyAUS Posted at: 2019-10-07T02:02:50.466Z Reads: 122

```
Trying this app now. Posted on your youtube too but... my board state is going to "Dead", why would that be?

Still having that issue (1), or alternatively the board locks at 85% (2) throttle regardless of IMU position. Not using footpads at the moment and motor is decoupled from wheel (my setup is indirect drive - chain to wheel)

(1) https://photos.google.com/share/AF1QipMdmByh5TpTZOkYmJmFG_qMfDPJQdYlhXjt20x8PcJUCRABvyxi5knryr9nBXue4Q?key=NWNUYi1PUTgwazItRGluSGxFZ2xwVzlHbUhCczFn

(2) https://photos.google.com/share/AF1QipOxGC1s61yhbwNaLAFaoXLvIqntA4tdGQlx8wTrWl_JRj4EHMIdLBdXidfPhvNCVA?key=ZmM3N0FiT3o2cURYcmJWZzQ1dWdEYjREWkhtb19R

(3) settings:

https://photos.google.com/share/AF1QipOYD6O0X2ncgjjX0f6WFBYiXaniJZFr7NeYlHaGmEeEFbjQE459DaCPJDBV6rxxPQ?key=NTVaU1FuM0ItY0hwaHhGTDJnaTJGbUhaMU1TMUlR
```

---
## \#353 Posted by: Surfer Posted at: 2019-10-07T08:19:46.632Z Reads: 115

```
Is going to dead because the cut off is set to 0.9, try to set it to 1.
The another questions, I cannot see good the videos, maybe photo for all setting can help.
Good luck!
```

---
## \#354 Posted by: SwarleyAUS Posted at: 2019-10-07T10:11:56.447Z Reads: 114

```
He says in his tutorial video not to, for good reason - the throttle locks to max if you do set it to 1: https://www.youtube.com/watch?v=0y5ME2SgwLg&feature=youtu.be&t=2209
```

---
## \#355 Posted by: Surfer Posted at: 2019-10-07T16:28:48.202Z Reads: 114

```
![Screenshot_20191007-182649|518x500](upload://v3df3shpW4W3CCXOTSIFSDH5FdW.jpeg) 

Is just some post above
```

---
## \#356 Posted by: NuRxG Posted at: 2019-10-07T17:35:35.013Z Reads: 115

```
Looks like there is 2 things going on in your video.

Firstly look at your pid output, the pid output is unbounded so it can get to really large numbers in one direction and take a while to come back to 0 and change motor directions (if the feedback loop is not complete, aka it is on a bench and the motor is not moving the gyro). When you tilt one way it is fine, but when you go the 2nd way you're letting your pid output get very high and not giving it time to get back to 0.

Secondly it seems your VESC is topping out at 85% duty cycle which is quite weird. Did you set that limit to 85% in your motor config under the advanced tab? What VESC are you running? VESC should be able to hit 95% efficiency aka duty cycle, if your VESC is capped to 85% duty cycle, you will never hit your cutoff at 90%.
```

---
## \#357 Posted by: Jopj Posted at: 2019-10-08T00:49:24.666Z Reads: 113

```
Since many of us are using the phub-188, wouldn't it bea nice to gather a bit of information on how the versions differ, if at all? It's said that the 48V and 36V versions are the same, but I'd bet the 24V version is too. I have the 24V and run it with a 10s pack. With 40V in, it'll reach around 5500 ERPM spinning freely.

I'd be interested in knowing what others using this motor are seeing. ERPM/volt will indicate if they are actually wound different.

I recently improved the software for the Redstar a lot, includes a damping term, changeable neutral stance and pushback, but most importantly some diagnostic beeps to show which limit is being reached first. In my case it's nearly always duty cycle. I can't push enough power in even though I'm supposedly running the motor overvolted. Physically, it only gets slightly lukewarm and certainly could take more. I'm betting the motor is actually meant for a higher voltage than the 24V.
```

---
## \#358 Posted by: SwarleyAUS Posted at: 2019-10-08T01:44:08.416Z Reads: 112

```
Thanks. There not being a load was my next guess, which Fungineers confirmed. Will try with the wheel tonight. Bit hesitant though, with the issues I am experiencing.

So your PID is not bound to any limit in the firmware?
<br />
Is the PID value equal to *pitch x P + gyro rate of change x D*?

I think when I filmed the second video I may have had motor scale at 95%. This would mean the max duty (I believe) would be 85.5%. Anyway, if I can't fix it it's no biggie to me. It's a flipsky 4.12 FYI.

Thanks for your help.
```

---
## \#359 Posted by: Fosterqc Posted at: 2019-10-08T03:26:56.770Z Reads: 109

```
Could try contacting Pei Pei scooter, I assume we make up some amount of the customers for it. 

Could also take one apart and looks at the stator or whatever. Would be interested to see.
```

---
## \#360 Posted by: SwarleyAUS Posted at: 2019-10-08T08:24:16.001Z Reads: 111

```
Sweet. With a closed control loop the board responds predictably. Is anyone using the I in PID though? In a onewheel application I would expect to only use P&D...
```

---
## \#361 Posted by: NuRxG Posted at: 2019-10-08T08:43:05.478Z Reads: 107

```
on previous firmware iterations ive used I term, but with the onboard vesc firmware, adding any I has only made it unstable for me.
```

---
## \#362 Posted by: Jopj Posted at: 2019-10-08T14:55:15.385Z Reads: 110

```
I use a pretty heavy I term in my firmware, and find it very useful when climbing hills. Without it, a nose down attitude from neutral is needed to drive the motor which is a bit hairy with the already reduced front ground clearance on hills.
```

---
## \#363 Posted by: Jopj Posted at: 2019-10-08T14:56:19.732Z Reads: 107

```
I didn't have any luck in getting specs out of them when I was buying the motor :frowning:
```

---
## \#364 Posted by: Remieknaapen Posted at: 2019-10-08T18:25:03.531Z Reads: 111

```
What settings are you running on your onewheel, could you make a screenshot?

My board is working but the motor is making this horrible sound arround the balance point. Like it's constantly vibrating because it wants to keep the board balanced. Any idea what that couls be? Motor runs fine during setup. Bearings are stil good

Could be that my sensor is mounted to soft (double sided foam tape)?
```

---
## \#365 Posted by: Jopj Posted at: 2019-10-08T18:40:12.514Z Reads: 105

```
I use homebrew software running on a separate processor from the vesc, so my settings won't be comparable to the vesc app, atleast not directly. I use kp = 6.0, ki = 0.05,  kd = 7.0; with a pid evaluated at 100hz, with madgwick filter input that's running at 4khz and 0.1 beta.

I also get a sort of buzzing jitter around zero if I have too much d-term, but it's good at higher speed. Maybe I'll work in a speed-dependent d-term.. Try with only a low p-term, it'll be bad for control but will help finding out the cause. Could be reacting to the motor cogging at low speed, it causes quick acceleration spikes that would show up in the d-term output.
```

---
## \#366 Posted by: SwarleyAUS Posted at: 2019-10-08T21:44:17.363Z Reads: 101

```
What I might suggest is doing something like take in the accelerometer Z value and if more than 9.8g (ie going up a hill) increase the sensitivity, ie P gain, of the board. This is what I coded up for my board but did not test. Will go back to this w/ESP32 controller if I need to.
```

---
## \#367 Posted by: Jopj Posted at: 2019-10-08T22:15:29.869Z Reads: 104

```
I don't think that's a good way to do it. Accelerometer won't tell you if you are going up a hill (ideally it'll read exact same as while stopped when moving up at a steady state), and if there's room to increase P without oscillations, then why not increase it across the board. More P will make you need less nose drop per motor amps, but integrator will get you the required amps with ~zero nose drop once you get going. It works great.
What I'm looking at is adjusting the board neutral angle based on motor current and motor speed change. High current without corresponding speed change = hill, likewise negative current = downhill.
```

---
## \#368 Posted by: NuRxG Posted at: 2019-10-08T22:18:42.151Z Reads: 109

```
1g = 9.8m/s perhaps that is why it didn't work.

having more P gain up hills isn't what you want, you'd want to adjust adjust the setpoint angle to elevate the nose. However its not as simple as it seems. Any time you accelerate the nose is down a bit and you move forward, this already gives you more than 1g accelerating on flat. Also the G forces measured going up a hill are not constant, youd only have increased G when accelerating, when traveling up a hill at a constant 10 mph you'd still be 1G of downforce. 

I do plan on adding elevated nose option to the VESC, it will likely be in the next feature set when i get around to doing a next feature set. Its just gonna be directional nose elevation with smooth transitions from flat to elevated.
```

---
## \#369 Posted by: Jopj Posted at: 2019-10-08T22:26:33.668Z Reads: 110

```
We have the same idea :smiley: How do you plan on choosing when to raise the nose from whatever default value it's configured for normal riding? Some kind of external control or sensing the need from motor current and speed? I only have the latter option since my hardware lacks a radio of any kind.
```

---
## \#370 Posted by: Jopj Posted at: 2019-10-08T22:37:57.514Z Reads: 116

```
![P_20191008_183741_vHDR_On|670x500](upload://tzjCQw44mdLmW648r3ks0XbzfmV.jpeg)
Wanted to put a bit of paint on it just because.
![P_20191008_194051_vHDR_On|670x500](upload://9ImI92Xwh337pUWjgKTmnPQT49y.jpeg)
Didn't turn out perfect, but I like having the sensor positions visually marked. The griptape is showing some wear as the miles start accumulating, but hopefully it'll hold up :no_mouth:
```

---
## \#371 Posted by: SwarleyAUS Posted at: 2019-10-08T22:40:03.875Z Reads: 112

```
Which hub motor are you using? What wattage? Torque-y enough?
```

---
## \#372 Posted by: Jopj Posted at: 2019-10-08T22:45:31.156Z Reads: 115

```
I'm using the usual phub-188. Spec is 600W but I run it with 1kW peaks and it doesn't even get warm (short balance peaks :smirk:) Lack of power at speed is my biggest issue right now, I think even the "24V" phub is actually the same as the 60V one so my 10s pack has to low voltage, I ran out of duty cycle before anyhing else. I'll test with a 12s pack cobbled from RC plane batteries to see if that's enough, I really think this motor wants more voltage.

(edit) the problem is the low KV and not enough voltage to push current through it, motor itself seems solid and I've never gotten it more than slightly lukewarm
```

---
## \#373 Posted by: NuRxG Posted at: 2019-10-08T23:11:58.252Z Reads: 116

```
It will be another config option with a use configurable angle, then it will be activated above some non configurable erpm, and it will be direction based on the motor direction. It already has all the tiltback code for smooth angle changes, so it will probably happen at the configured tiltback speed.

Im on the fence about adding features that require the motor position tracking and wheel size to be accurately configured. But it would be cool to be able to offer drive changes based on exact speeds. Perhaps a stiffer ride feel above 10mph, or nose up activated at exactly 3mph, etc.
```

---
## \#375 Posted by: SwarleyAUS Posted at: 2019-10-09T11:45:17.873Z Reads: 117

```
Final ride for the night with the setup complete:

https://www.youtube.com/watch?v=JgYlhUdbRRY&feature=youtu.be&fbclid=IwAR3Vz-aSWtoBWz0I2iCQYgn3fFmMN_sf-liZ5XtNfwaczIJLAKS0O40Ekks

P gain: 17<br />
D gain: 300<br />
Beta: 0.01<br />
Pitch cutoff: 15 degrees (why it threw me off)

I think I still need more D? Would like it as buttery as possible! Chain drive isn't helping with efficiency and power delivery - not to mention I'm running 24V.
```

---
## \#376 Posted by: Jopj Posted at: 2019-10-09T14:17:46.932Z Reads: 119

```
Quick ride on the Redstar with some new program improvements and added rollers so I won't go flying if the nose digs in. I'll stiffen the control up in the future, but it's very comfortable now.

https://www.youtube.com/watch?v=PoC1mRiQK3Q
```

---
## \#377 Posted by: SwarleyAUS Posted at: 2019-10-09T22:05:17.764Z Reads: 113

```
Looks awesome! So rock solid compared to mine. Think I need to go to a phub as well... better torque delivery is what I need I guess to get a smoother ride. 

Care to share your settings?
```

---
## \#378 Posted by: Jopj Posted at: 2019-10-10T05:19:43.380Z Reads: 112

```
It's a diy control board no vesc-compatible settings, i posted the pid and filter parameters a few messages back. What is your motor? It's very likely that the phub will have less torgue than your current setup, being a low power hub motor. With a chain drive, backlash will be the worse issue, that will throw off pids easily. Does your motor have sensors? If you do end up with the phub, use a high voltage. The 42v my pack gives when full is too low.
```

---
## \#379 Posted by: SwarleyAUS Posted at: 2019-10-10T05:45:59.499Z Reads: 113

```
Ah that's right, yeah that's what I was doing but having problems with software and ESP32 hardware. Will try this for now but may go back to ESP32 when a new one arrives so I can get telemetry via bluetooth (which was working quite well). I have learnt more about the VESC through this process so hopefully I can eliminate my bugs if I do.

Motor is a sensored 6384 with 10t drive sprocket chained to 60t wheel sprocket. So there should be about maybe 10Nm at the wheel? The mechanical linkage in my setup does not help with 'smoothness'. I wodner if the phub has a planetary system or direct drive like the hypercore motor. Dang even at 42V!? It doesn't look like torque is lacking on yours... How fast can you go? Hitting max erpm?
```

---
## \#380 Posted by: Fosterqc Posted at: 2019-10-10T05:55:12.324Z Reads: 118

```
Phub 188 is definitely a non geared standard hub motor. 

Geared would be cool, but at that point just use a actual gear drive and a large low KV normal inrunner or outrunner. I think you could reverse mount the motor inside the wheel hub of a normal go kart tire. If you found one with a lot of space that would be cool.

Lmao maybe a airless tire so it could be significantly thinner than a pneumatic tire near the rim offering lots of space for motors and gearboxes inside the wheel area.
```

---
## \#381 Posted by: Jopj Posted at: 2019-10-10T06:09:19.650Z Reads: 122

```
[quote="SwarleyAUS, post:379, topic:80129"]
Motor is a sensored 6384 with 10t drive sprocket chained to 60t wheel sprocket
[/quote]

Then you definitely can have way more power and torque than I do with the Phub-188 as long as you have large enough current limits in VESC!  I suggest you add an idler or move the mount around to minimize backlash, or better yet go to a belt drive. I'd say especially with the latter that your drive would be a lot better than the phub. My max speed is only around 16 kph, and torque is lacking whenever there's quick accelerations, curbs or stuff like that. Not because of lack of current, but because the motor simply won't draw more, needs more voltage than 42.
```

---
## \#382 Posted by: Remieknaapen Posted at: 2019-10-10T19:52:05.526Z Reads: 128

```
Just wanted to share with you some pictures and specs of my Onewheel build.
It's still a work in progress, some parts need to be reprinted because they are damaged and some parts do need some redesigning. Also the footpads are just for testing, i plan on making some nice curved pads from wood or also 3d printed.

My setup is:
- Phub-188 36V
- 12s2p Samsung Q30
- FOCBOX with MPU09250 and Vesc balance software
- flipsky anto spark switch
- WS2812 led strip for front and tail light, powered with 5v from the FOCBOX and controlled by a teensy 3.2.
- lots of 3d printed parts
- aluminium U-profile 20x40x20mm and 3mm thick 
- XLR charge plug
- Diy velostat footpad sensors.

Here are some pictures of the build. Once I'm a bit more confident riding the board I will try to upload a video of the board in action!

3D printing battery box:
![IMG_20190710_075252|666x500](upload://dl00GnrxIe0DXL71Wwjp9yID2CX.jpeg) !

Programming and testing the WS2812 led strip:
![IMG-20190712-WA0017|690x388](upload://2sKJ6wiMrnYdgSUHw4IW5uURKAD.jpeg)

Velostat footpad:
 ![IMG-20190808-WA0006|690x388](upload://eGCEaCN7wn6UWrCIWMsWVR8cV0h.jpeg) 

Test fitting all the parts:
![IMG-20190809-WA0005|690x388](upload://cOHIHKnXaVJohkbquR3Ttg6NNBe.jpeg) 

Power button and XLR charge plug
![2|666x500](upload://qDrTTQfff586HsXaMygRYikCjug.jpeg) 

Front light:
![3|666x500](upload://cIl8tzUqxjSEgjC61elmaYIJFe6.jpeg)

Tail light:
![1|666x500](upload://q9gHg13wEaMCPYRnvFtntCqcRlm.jpeg)
```

---
## \#383 Posted by: zorglups Posted at: 2019-10-10T20:44:16.525Z Reads: 118

```
Whaouw !!! Proficiat from Belgium !!!!!
```

---
## \#384 Posted by: Hamont Posted at: 2019-10-10T21:18:37.684Z Reads: 121

```
Hey everyone, I am planning a one-wheel build. Parts ordered so far:


PeiPei hub motor 600W 48V

Queen Battery 6.8 Ah 26800 cells 14s1p

Chinese BMS (Changelin Powers Store)

Chinese Vesc clone 


Anyone have experience mounting a force sensitive resistor between a wooden deck and grip tape? Whats the consensus on reliable foot sensors?
```

---
## \#385 Posted by: s.white432 Posted at: 2019-10-10T21:21:08.905Z Reads: 113

```
Very nice build! I'm keen to see it in action.

Does 12S seem powerful/torquey enough? Jopj mentioned that 10S wasn't sufficient in his opinion.
```

---
## \#386 Posted by: s.white432 Posted at: 2019-10-10T21:23:08.858Z Reads: 109

```
Most people seem to use diy velostat sensors. See video from Fungineers https://youtu.be/Nx0Q9rcH_sI
```

---
## \#387 Posted by: Jopj Posted at: 2019-10-10T22:01:01.153Z Reads: 112

```
My velostat sensors are between griptape and aluminum and have worked great so far. I did glue them to the aluminum to help take some load. I guess if there's enough griptape-baseplate contact it should be fine with the grip taking most of the shear loads. Time will tell. Which vesc clone are you using that can handle 14vs?
```

---
## \#388 Posted by: Jopj Posted at: 2019-10-10T22:04:00.680Z Reads: 116

```
Looks great! Please report how you feel about the 12s pack and the phub, i'm also planning to go there with 12s3p vtc5a pack hoping that it's enough. Measured my speed at 80% duty cycle with "24v" phub and the current 10s, only 14 kph :frowning: Needs moar volts.
```

---
## \#389 Posted by: Surfer Posted at: 2019-10-10T22:33:31.721Z Reads: 111

```
Maybe interesting to check the motor/kv of the phub, to know if it's a torquey motor or more on faster side, that option is available in vesc tool.
```

---
## \#390 Posted by: Hamont Posted at: 2019-10-10T22:36:30.359Z Reads: 111

```
I can't link the AliExpress item, but it's called HGLRC Flipsky ESC.


Seems to use 60V FETs, not sure about the DC link. If I charge to 58V, I should be good, yeah?
```

---
## \#391 Posted by: Surfer Posted at: 2019-10-10T22:46:38.747Z Reads: 114

```
Nope, don't ask me how I know!
Vesc hight voltage cut off 57v cant be changed
Charging to 55 volts worked for me.

#Todaytailnose
```

---
## \#392 Posted by: Jopj Posted at: 2019-10-10T22:49:08.275Z Reads: 111

```
Even 13s is super hairy on those standard vescs, there needs to be headroom for all the spikes that happen. People used to routinely kill theirs at 12s before the designs were improved..
```

---
## \#393 Posted by: Jopj Posted at: 2019-10-10T22:51:40.741Z Reads: 111

```
Is it? Cool, I didn't know. I'll surely try to find that option. Although it most likely needs pole count, which I don't know.. By my calculations mine is around 10 kv
```

---
## \#394 Posted by: Hamont Posted at: 2019-10-11T00:25:34.432Z Reads: 113

```
I'll see what happens with mine, it was cheap enough that blowing it up wouldn't be the end of the world.


Alternatively I could use an ASI BAC500 which I have lying around for something else.
```

---
## \#395 Posted by: Fungineers Posted at: 2019-10-14T11:04:37.254Z Reads: 115

```
these sensors worked well with Arduino, but didnt work with the vesc balance app. 
The Balance app is more of an on/off type, whereas on the arduino i could tweek the analog input to exactly what I liked. 
I ended up making footpad sensors like @NuRxG (copper tape- velostat-spacer-velostat- copper), but it didnt work either. They were 'always off'. 
Frustrated with the arts and craft stuff, I ordered the tiny square FSRs, and Im using those now. The only issue with these is that these are too sensitive! So much that if I wrap the griptape too tight, it is on. 
However, the DIY footpads worked for a lot of people so give that a shot. Build them like @NuRxG
```

---
## \#396 Posted by: Fungineers Posted at: 2019-10-14T11:39:42.715Z Reads: 115

```
Ride this morning. Didn't end well haha. 

https://www.instagram.com/p/B3lVu9yD2pH/?igshid=7o46o49rgz9i
```

---
## \#397 Posted by: Jopj Posted at: 2019-10-14T20:07:20.054Z Reads: 114

```
Ouch! Any idea why that happened? I noticed in the vesc code that there's a thing called "overspeed cutoff", which disarms the motor if the duty cycle is too high. Isn't that dangerous, whenever the motor is driven to full power it'll cut out? I know that behaviour would have ended up with me on the ground many times when I ran out of duty cycle with my 10s pack, so I instead just have it beep and do it's best to keep up.
```

---
## \#398 Posted by: Jopj Posted at: 2019-10-14T20:25:37.294Z Reads: 117

```
Practicing those tighter turns where you get up on the edge of the tire. These things can be quite maneuverable! I added an extra check in the code that prevents the motor from disarming during those turns when the speed is low enough and the weight comes off a footpad. It'll now only disarm with one footpad if also the roll angle is low enough, meaning no tire-edge turns are being done

https://youtu.be/hNCafMnXcKI
```

---
## \#399 Posted by: Jopj Posted at: 2019-10-14T20:41:59.302Z Reads: 119

```
Have you tested your velostat sensors to find out how much pullup they require? I used a potentiometer in series with them (vcc -> pot edge -> pot wiper ->sensor ->ground)  and read the voltage from the potentiometer-connected sensor with an Arduino. That way I could spin the pot to find out how much pullup I need so that transitions between pressed and not pressed are the largest, and happen at the right pressure. The sensor I made was pretty low resistance, and I used a pullup of 60 or so ohms.![P_20190928_162825_vHDR_On|670x500](upload://50Isiuiwb4KzKidBrMoEPg2h0Rr.jpeg)
```

---
## \#400 Posted by: Khurtana Posted at: 2019-10-14T22:22:03.700Z Reads: 114

```
I believe Onewheel uses a 36v battery pack and a 750w motor. So, 10s2P.  I think the new peipei motor you’re linked would be a good equivalent.
```

---
## \#401 Posted by: Jopj Posted at: 2019-10-14T22:25:30.973Z Reads: 113

```
Yes, it could be. In my case though the power handling of the motor isn't the problem, it just has too low KV for a 10s pack to be able to get good power out of it. And mine is the lowest voltage version which should have the highest KV, if there's any difference at all..
```

---
## \#402 Posted by: NuRxG Posted at: 2019-10-14T23:11:31.141Z Reads: 110

```
onewheel v1 & plus both use the same battery its is LiFePo4 15 or 16s (i forget) 1p of the a123 systems cells. The xr is higher voltage, but im not sure what cells and chemistry.
```

---
## \#403 Posted by: veebee Posted at: 2019-10-14T23:41:03.198Z Reads: 113

```
XR uses Samsung 18650 30q in 15s2p.
```

---
## \#404 Posted by: Khurtana Posted at: 2019-10-15T04:09:59.328Z Reads: 107

```
I really don’t understand the voltages mentioned by PeiPei and no discussion with them gives me understanding.  I think all the motors are the same 24/36/48v etc.  The different wattages MAY be indicative of different units but I’m not sure.  Anyone know mandarin?
```

---
## \#405 Posted by: Fungineers Posted at: 2019-10-15T05:37:28.880Z Reads: 104

```
Mine were around 50kohms! (did some crude trial and error testing). Maybe Ill make another one and do some more testing since I dont like the FSRs (too sensitive).
```

---
## \#406 Posted by: Khurtana Posted at: 2019-10-15T05:39:33.999Z Reads: 99

```
50kohms?  You sure that wasn't a pull down?
```

---
## \#407 Posted by: Fungineers Posted at: 2019-10-15T05:45:37.018Z Reads: 106

```
When you say 'overspeed cutoff', do you mean 'cutoff duty cycle'? If thats what you mean, then you are right, once the motor reaches 0.90 Duty, it shuts off and sends the rider flying. I talked to Mitch, and it seems the vesc can do only max 0.75 duty so  0.9 is safe. The best is obviously to just set it to 1.0 (thats what I do) so that this never kicks in. 
If you are talking about another overspeed cutoff I want to know about that!

As to 'what happened in the end?' question: 
It looks like the P and D settings affect the motor more than I realized! If D is too high, the motor cogs and twitches randomly at low speeds, nothing significant, but it feels like it loses power for a split second, and then regains it. Now when you go faster, that split second becomes significant, and by the time motor regains control, you are already on the ground. lol.
So, tldr: I adjusted my D settings (around 100-120) and the ride was much smoother. No cogging at low speeds, and no nosedives at high speeds. 

Would love to hear if anyone else had this issue?
```

---
## \#408 Posted by: Jopj Posted at: 2019-10-15T10:53:36.114Z Reads: 108

```
That's the overspeed cutoff I was talking about. Vesc can do 0.95 duty cycle. In the code it starts pushback earlier, maybe that was the 0.75. In my code I start pushback at 0.8 but keep the motor engaged above that, when it reaches 0.95 it can no longer balance, but atleast there's a chance for the rider to lean back and bring the duty cycle down.
The D term basically reacts to the change of error. If it's unfiltered, high D will cause very high output spikes when input spikes, like when the motor cogs or anything not-smooth happens. Have you checked your vesc log for errors after those losses of control? Maybe it hit the overcurrent cutoff or something due to too aggressive control?
```

---
## \#409 Posted by: NuRxG Posted at: 2019-10-15T18:28:36.381Z Reads: 112

```
I think it has been said before, but ill re-say it, since this feature seems to be quite controversial lol!

It is optional, you can turn it off, and in fact if you have foot sensors you should turn it off. 

However on an euc which doesn't have foot sensors and will accelerate on their own if not perfectly balanced, it is critical to have some safety mechanism to stop them from riding off at max speed.

It is enabled by default, there are a lot of extra safety steps enabled by default, for example P/I/D are all 0. All of these safeties are there to prevent your motor from instantly spooling up to max speed when you first enable the balance app, and sending your setup through a wall. Self balancing vehicles are pretty dangerous, and I made a best effort to prevent injuries.

Perhaps right now when it is just a handful of smart builders making wheels everyone is smart enough to put it in a safe position during setup, but i know that wont always be the case.

I do however think it would be very beneficial to add a time delay, perhaps 1 or 2 seconds to the duty cycle cutoff. I intend to do this eventually, but after the initial release, I've been focusing on other projects and just getting out and riding for a while, it is open source, so you're all welcome to implement it if you wish, but none of you are man enough to ride an EUC anyways :crazy_face:
```

---
## \#410 Posted by: Detonatedfrost Posted at: 2019-10-16T01:39:33.032Z Reads: 113

```
Been following and this tripped me up because its labeled RX/TX on some VESC's so I'll clarify for us special needs folk...  
SCL  from  MPU  to  TX(SCL)  on  VESC..........................
SDA  from  MPU  to  RX(SDA)  on  VESC
```

---
## \#411 Posted by: Fungineers Posted at: 2019-10-16T10:42:57.717Z Reads: 112

```
I will ride your EUC while doing a handstand Mitch :stuck_out_tongue: 

Thanks for clarifying this!
I personally prefer to have tiltback on my OW. Its like..a connection..like the board is talking to me.
```

---
## \#412 Posted by: Fungineers Posted at: 2019-10-16T10:49:15.796Z Reads: 116

```
Now that people are riding the boards, I think we can move beyond the basic construction, and take it one step further. I would love to see someone implement front and back lights on the vesc. 
Probably one of these pins: PWM, Temp, CAN.
I would have tried to do it myself but Im kinda...dumb with this stuff.
@NuRxG is too busy riding eucs, lol
@Jopj did you try to do this?   
anyone else?
```

---
## \#413 Posted by: Squab Posted at: 2019-10-16T11:11:55.420Z Reads: 115

```
![image|690x445,50%](upload://kkiqnqTJPutWApI3XcShd7WRzmE.png) 
I disagree
```

---
## \#414 Posted by: Jopj Posted at: 2019-10-16T12:16:11.984Z Reads: 108

```
Yes, I'm going to, but as I'm using my homebrew control board instead of VESC it's not directly transferable there. I have my eyes on full-side-length ws2812 strips sometime in the future, I modified the Teensy octows library to drive only a few pins so that I can use them here. I already kind of have lights, not the sort that'll let you see, but RGB indicators and a bargraph on the front, all PWM'd of course :slight_smile:
```

---
## \#415 Posted by: Giga Posted at: 2019-10-16T12:54:45.759Z Reads: 108

```
[quote="Fungineers, post:412, topic:80129"]
Now that people are riding the boards, I think we can move beyond the basic construction, and take it one step further. I would love to see someone implement front and back lights on the vesc. Probably one of these pins: PWM, Temp, CAN.
[/quote]

It is already implemented in the nondefault WS2811 firmwares. 
Though you have to change the pin, since it is at the sensor port at the moment. Also I would not use the CAN ports. One day there will be a nice CAN BMS with tolerable dimensions which you want to wire up via CAN. 
IMO one of the ADCs or the Servo port should be sacrificed.
```

---
## \#416 Posted by: Fungineers Posted at: 2019-10-16T13:41:10.221Z Reads: 102

```
Yes but in the ws firmware they don't change direction do they?
```

---
## \#417 Posted by: Byngham Posted at: 2019-10-16T15:17:37.247Z Reads: 101

```
I'd specifically asked the folks at Trampa before ordering a Vesc 6+.  The guy that responded back said that 13S would be fine.  Jopj, do you think it was bad advice, or is the Vesc 6+ an example of the hardware after the designs were improved?
```

---
## \#418 Posted by: NuRxG Posted at: 2019-10-16T16:00:07.109Z Reads: 100

```
Honestly seems like a ton of work, and ugly code to get leds working onboard the vesc, I'm skeptical it would get merged. What is the benefit anyways? Seems trivial to wire up leds to an arduino.
```

---
## \#419 Posted by: Jopj Posted at: 2019-10-16T17:13:39.368Z Reads: 106

```
Yes, the ones with the most problems were the older 4.12 designs. The current, official vesc6 is certainly one of the robust ones. The limiting factor is the DRV chip that's theoretically OK for 60V, but in practice even with lower battery voltage there will be spikes which can exceed that and cause damage. The vesc6 should be ok anyway, but when in doubt it's always good to add extra capacitors to the VESC input to help deal with the spikes, I use 5x 100V 1000uF caps on my scooter for that purpose since it had space to mount those.
```

---
## \#420 Posted by: Fungineers Posted at: 2019-10-16T17:42:21.435Z Reads: 105

```
An arduino and ANOTHER mpu? And powered from the vesc? Vesc wont like that I have experience lol. So a buck converter..ahh that is more cumbersome isnt it?
```

---
## \#421 Posted by: NuRxG Posted at: 2019-10-16T17:55:57.028Z Reads: 112

```
Perhaps you can use something like this?
https://www.sparkfun.com/products/14001
```

---
## \#422 Posted by: Jopj Posted at: 2019-10-16T18:52:21.224Z Reads: 114

```
You can easily power the arduinos and IMU's from the VESC, but depending on how many LED's you want a buck could be a good idea. The VESC regulator is good for 0.5-1.5A depending on model, the 1.5A one would let you drive ~18 WS2812 LEDs with peace of mind. Overstressing that regulator isn't a good idea since that will cause the rider to eat asphalt.
```

---
## \#423 Posted by: Jopj Posted at: 2019-10-16T18:55:58.704Z Reads: 113

```
If you are looking at a microcontroller to drive LED's I'd suggest the Teensy line, the 3.2 is nice and small + very good for driving WS2812 leds. There are readymade [libraries](https://www.pjrc.com/teensy/td_libs_OctoWS2811.html) for them that'll drive 8 strips in parallell without blocking your code, or [single](https://www.pjrc.com/non-blocking-ws2812-led-library/) strips with UART hardware
```

---
## \#424 Posted by: Detonatedfrost Posted at: 2019-10-17T00:44:27.478Z Reads: 113

```
1st Thanks for everyone's effort on this project.  I'm stoked about it.  
2nd  I could use a little advice.   For 2 days I'm trying to get a Maytech superfoc 6.8 to receive/show data from the MPU6050.  I've read pretty much this whole thread and watched NuRxG's video.  I believe I got all the obvious stuff covered.  I'm assuming I don't need a sensored motor connected to see live data?  
Thanks
```

---
## \#425 Posted by: Detonatedfrost Posted at: 2019-10-17T01:22:00.931Z Reads: 111

```
Are any of you familiar with Betaflight for FPV.  Its the most popular interface for FPV drones.  It has fairly  extensive LED programing.  The main reason for integration would be to automate lighting based on what the board is doing.  Some extra channels on our remotes would also be nice to trigger different modes.   At some point I'd like to have the balance app set up as a mode that could be triggered on my skateboard for "wheelie mode"   I have not seen it done on anything yet...  "Digital Wheelies" :stuck_out_tongue_closed_eyes::stuck_out_tongue_closed_eyes:
```

---
## \#426 Posted by: Detonatedfrost Posted at: 2019-10-17T02:56:20.697Z Reads: 110

```
Maytech is saying I can’t connect gyro to IC.  I can only use Uart... 🤦‍♂️..
```

---
## \#427 Posted by: NuRxG Posted at: 2019-10-17T17:49:06.682Z Reads: 106

```
Ive setup betaflight quads with leds, I wasn't into it tbh, i could have a different color for arm modes but I never really found it all that useful. I wanted to do animated sequences, and i don't believe it is possible with betaflight.
```

---
## \#428 Posted by: XtremeRacing Posted at: 2019-10-17T18:36:04.830Z Reads: 110

```
It’s not a bad Idea want switch directions without facing the other directions the dark. It might come in handy want to test your skills in a tight space have to backup but there isn’t enough room to turn your body around so you have to ride switch. If your anything like me you might have to think skinny thoughts to fit in the first place. 

Go nuts and add the beep, beep, beep that heavy machinery makes when it is backing up. I’d do it just to see people’s reactions when they turn around expecting to see a backhoe instead of a onewheel.

If you don’t mind using you phone to turn on the lights you can control your lights with an esp32 for cheap with built in BT. I might use one to control flashing RGB leds to back of the board so I don’t get mowed down at night. I saw a cyclist with hot pink flasher that Ray Charles still couldn’t miss.  Another idea is to add a pressure switch kick plate toward the back of the board to swop front and rear lights.
```

---
## \#429 Posted by: XtremeRacing Posted at: 2019-10-17T20:55:17.662Z Reads: 109

```
I am looking at the same 800w motor. I'm also considering peipei’s scooter motor. You can get it configured up to 1200 W it has a 12 inch rim and takes tires I can get at a local tire shop pretty easily. I live in Phoenix AZ were temps will get to 115-118°F during the summer. I'm hoping motor is rated for higher wattage will come with thicker gauge wires hopefully prevent overheating. 
[1200w 12" Wheel](https://www.peipeiscooter.com/60v-1200w-1brushless-dc-wheel-hub-motor-for-halley-electric-motor-phub-146.html)

If they will actually configure the voltage. I'm thinking 36V. I'm planning on little bit different battery set up utilizing 24V kobalt batteries I've got a ton of them and I have a got a few different Ideas on how to config and charging. considering I doubt I'm going to find a BMS to that will work for my setup. (actually 22.2V). 2S4P What do you think?
```

---
## \#430 Posted by: BayneSolo Posted at: 2019-10-17T20:56:04.456Z Reads: 108

```
Hey yall, so I'm pretty much finished my DIY onewheel and I'm just in the "Everythings connected why the fuck won't this work properly" stages of the build.

I am doing a hybrid build between salvaging motors from a self balancing scooter and a vesc based build, so it means I'm running 2 motors. 

What's the best way of hooking 2 vesc's up to one IMU?? I've tried direct wiring it (with power from both and with power from one and only signal to the other) and also I have tried the CANBUS but either through my newness or it just not wanting to work, can't seem to get both vescs to play ball. 

Any suggestions?

Edit: I've now also tried the XDA and XCL pins into the 2nd vesc which enables them but disables the SDA and SCL pins :( not really sure what other options there are without breaking it out to an arduino.
```

---
## \#431 Posted by: XtremeRacing Posted at: 2019-10-17T21:09:59.125Z Reads: 99

```
NuRxG I think I found your next motor. [11" 5000w](https://www.peipeiscooter.com/11-inch-11inch-5000w-fast-speed-double-axles-bldc-brushless-no-gear-hub-wheel-motor-with-tyre-fit-disc-brake-phub-11nm.html):sweat_smile: You'll need a proton pack to power it. :ghost: :scream:[I ain't afraid of no ghost.](https://www.youtube.com/watch?v=VWb1z6ZwUoY)
```

---
## \#432 Posted by: NuRxG Posted at: 2019-10-17T21:24:09.928Z Reads: 100

```
If there is a next motor for me i will be [this beast](https://www.ebay.com/itm/Leili-12000w-72v-Electric-Bike-Ebike-Fat-Tire-Regular-Tire-Conversion-Kit-MOTOR/123888689254?_trkparms=aid%3D111001%26algo%3DREC.SEED%26ao%3D1%26asc%3D20160908105057%26meid%3D849486a5cc534b729649e7a4374d53ea%26pid%3D100675%26rk%3D1%26rkt%3D15%26sd%3D123888689254%26itm%3D123888689254%26pmt%3D0%26noa%3D1%26pg%3D2380057&_trksid=p2380057.c100675.m4236&_trkparms=pageci%3A2d824712-f124-11e9-8c93-74dbd180426d%7Cparentrq%3Adb99720a16d0aa6a35496ca1fff4d4d6%7Ciid%3A1) powered by [a 75/300](https://www.trampaboards.com/single-vesc-75v-300a-in-cnc-t6-silicone-sealed-aluminum-box--the-most-powerful-vedder-electronic-speed-controller-ever-p-26284.html) I want to set a single wheeled land speed record lol!

P.S. if anyone wants to buy me this motor :innocent:...
```

---
## \#433 Posted by: XtremeRacing Posted at: 2019-10-17T21:38:00.075Z Reads: 100

```
That reminds more of a big wheel then a one wheel. It'd be like trying to balancing 12000w unicycle. :rofl: I'd like to see someone ride it on a tight rope. I've actually flirted with the idea of using an alternator from a F150 that I have lying around. My only hold up is the trip to the emergency room that would surely follow. :grimacing: My copay is way to high for that.
```

---
## \#434 Posted by: XtremeRacing Posted at: 2019-10-17T21:46:25.825Z Reads: 100

```
@NuRxG this is my first build using a VESC. I'm not a coder. I was hoping not to have to drop $250 on a 6+. Do you know of a good, less expensive option that isn’t going to be a coding nightmare. If the 6+ is the only way to go without having to tweak the code to much I'll drop the extra coin.
```

---
## \#435 Posted by: NuRxG Posted at: 2019-10-17T21:52:22.562Z Reads: 103

```
I don't understand your question, what does codeing have to do with anything? All vescs run the same code.

regardless you should get a 6+ from trampa, it is the best, and the only option that will allow you to use bluetooth. It's not really all that expensive if you compare the specs other ESCs.
```

---
## \#436 Posted by: XtremeRacing Posted at: 2019-10-17T22:05:36.005Z Reads: 96

```
I'm not all that formulator with vescs. I've done some basic Arduino builds, very basic. I was thinking it was comparable having to tweak Arduino code. I guess I'm going to buy a 6+. I figured I'd have to go that way but I wanted to check. Thanks.
```

---
## \#437 Posted by: XtremeRacing Posted at: 2019-10-17T22:12:56.863Z Reads: 97

```
Has anyone tried the peipei's  [phub-146 1200w 12" motor?](https://www.peipeiscooter.com/60v-1200w-1brushless-dc-wheel-hub-motor-for-halley-electric-motor-phub-146.html)? I'm really think that is the way that I want to go.
```

---
## \#438 Posted by: XtremeRacing Posted at: 2019-10-17T22:25:34.293Z Reads: 102

```
I've got an unorthodox idea for my battery system.  I am wondering if anyone have tried anything similar or has suggestions on how to best implement it. 

I've got a ton of Kobalt 24V lithium ion batteries that I picked up for cheap. Kobalt calls them 24V but they have 6 Samsung 18650 cells in them so they are actually 22.2V, regardless they were $10 for 1.5ah 22.2v battery packs so I’m not too upset about their creative marketing. 

I use the batteries for a lot of different things.  I prefer not to cannibalize them. My idea is to 3D print sleds to mount the batteries to and wire the 22.2V kobalt packs in series-parallel to whatever voltage of motor I decide to get. Probably the 12” 1200w @ 36V. If I get that I’d probably go with 2S4P I'd like to be able to charge the batteries either in the onewheel or pull them out and charge them on the original Kobalt charger. I am not sure if I can find a BMS that will work with the 22.2 V series-parallel packs to whatever voltage I decide to get set up probably 44.4V. My other options are to cannibalize a Kobalt charger and wire up a relays to charge each battery pack sequentially utilizing the BMS already on the batteries or wiring connectors to each cell on the battery packs bypassing the Kobalt BMS. Each cell will charge independently use a separate charge controller. That seems like a lot of work. I have 20+ batteries and I'd like to be able to swap them out when needed. That’s a whole lot of soldering.
```

---
## \#439 Posted by: Detonatedfrost Posted at: 2019-10-17T22:29:37.707Z Reads: 99

```
Yes I agree and you can always split receiver or other output to an arduino or better yet esp32 and have it all without cluttering the VESC...
```

---
## \#440 Posted by: Detonatedfrost Posted at: 2019-10-17T23:54:16.522Z Reads: 107

```
Hey Squab this is the PDF of the vesc 6 from the VESC page with an external 9150. Its opposite of your pic.  I’m thinking SCL = RX on one side but TX on the other but that still doesn't explain why your 4.7 pic shows Rx/scl on the vesc but the vesc 6 shows Tx/scl on the vesc..   I wouldn’t think reversing these would be damaging but it sure will trip up a bunch of people if they don’t know to try reversing if it doesn’t work.   🤷‍♂️
![image|374x500](upload://7SCfuVyugHiDyDlpAjmwxZB4xEK.jpeg)
```

---
## \#441 Posted by: Detonatedfrost Posted at: 2019-10-18T10:44:53.705Z Reads: 103

```
I use Makita on almost everything I build with 3d printed mounts.  So convenient..
```

---
## \#442 Posted by: Jopj Posted at: 2019-10-18T13:06:24.448Z Reads: 105

```
Maybe hook the IMU into one vesc, then the other vesc to the first one as a CAN slave, so it'll drive it's motor with the same current as the first one. This assumes your motors are similar enough that driving them with same current is a good idea.

Of course, you can do the balancing code on a microcontroller, which then drives whatever amount of vescs with whatever settings they have, but it's less plug and play.
```

---
## \#443 Posted by: mikenyc Posted at: 2019-10-18T13:53:59.477Z Reads: 101

```
any chance we get can start moving this thread to the esk8 news site?
```

---
## \#444 Posted by: NuRxG Posted at: 2019-10-18T15:55:39.413Z Reads: 97

```
Was considering starting a thread there for the onboard balance app in the vesc, but felt conceited.

It might be helpful to split this into a few threads tho kinda confusing with all the different controllers. and HW builds can be its own topic.
```

---
## \#445 Posted by: mikenyc Posted at: 2019-10-18T16:07:06.266Z Reads: 94

```
would be a shame if all of the info on this thread disappears when/if the forum gets shut down
```

---
## \#446 Posted by: XtremeRacing Posted at: 2019-10-18T16:58:02.294Z Reads: 93

```
What motor and voltage set up did you go with? Did you add a BMS and charging port on the board or do you remove the batteries for charging?
```

---
## \#447 Posted by: XtremeRacing Posted at: 2019-10-18T17:09:40.156Z Reads: 95

```
You shouldn't feel conceited. I find the more specific the tread the easier it is find the info that you need. It be great if someone came up with a way to you could sort the the how to tips separate form the rest of the posts but still have a quick way to reference the corresponding posts.
```

---
## \#448 Posted by: XtremeRacing Posted at: 2019-10-18T17:48:04.632Z Reads: 94

```
I just ordered the [phub-146 500-1200w motor.](https://www.peipeiscooter.com/60v-1200w-1brushless-dc-wheel-hub-motor-for-halley-electric-motor-phub-146.html) I figured it is worth the addition cost for a 1200w motor that comes with a tire I can get locally. They specify it as custom configurable from 500-1200w but it didn't give me the option choose the watts / volts when I ordered. So I'll have to send them an email telling I want 36v 1200w. That seems like the best config for me. I ordered directly from PEI's web site shipping was a whole lot cheaper then ordering it from [Alliexpress](https://www.aliexpress.com/item/32784296273.html?spm=a2g0o.productlist.0.0.75a6172aq3YdNk&algo_pvid=695e1865-7535-4c22-b24f-ed9a030f00d8&algo_expid=695e1865-7535-4c22-b24f-ed9a030f00d8-0&btsid=738f21c3-5a32-4252-b42b-e724f8b3b948&ws_ab_test=searchweb0_0,searchweb201602_4,searchweb201603_55)
```

---
## \#449 Posted by: Squab Posted at: 2019-10-18T18:53:36.079Z Reads: 94

```
First of all, tubular's vesc is 4.12 Flipscy's FSESC, not VESC 6. If you look at a schematic for VESC 4.12 you'll see that it's Rx/Tx ports are, in fact, flipt. ![image|214x115,100%](upload://obdyunLkFJmEzyywjgWhlZ3oAqg.png) 
Second, no, it wouldn't be damaging to STM, in my line of work through me goes so many burned up STM32's and most of them damaged by uneducated (or careless) workers who feed ~36V on Rx/Tx or freq. ports.
```

---
## \#450 Posted by: BayneSolo Posted at: 2019-10-18T22:04:27.500Z Reads: 92

```
Thanks for the tip, I've tried doing the CAN slave route but I can't get it to work. Whenever the balance app is enabled on the master, I get a firmware warning and it disconnects when trying to forward CAN.

I've ordered a i2c multiplexer to see if that fixes the address issue otherwise I might chuck it on an arduino and see if that works.
```

---
## \#451 Posted by: NuRxG Posted at: 2019-10-18T22:13:22.155Z Reads: 89

```
What is the firmware warning?
```

---
## \#452 Posted by: Jopj Posted at: 2019-10-18T22:18:02.323Z Reads: 92

```
Hooking up two vescs to the same imu won't work without lots of modifications to the code. They'll be both trying to control the imu and read data without regard to what the other is doing, you would need a mechanism to basically say "hey I'm talking with the IMU please don't go on the bus". You'd need to code multimaster support to the VESC. I can't help you with that but I'm sure CAN slave is the way to go, it's made exactly for what you want to do - just somehow to get it working with the balance app.

If you mean the XDA and XCL on the MPU, those are pins for connecting slave sensors like magnetometers to the MPU, the MPU is the master in that case, it won't talk to the vesc through those pins.
```

---
## \#453 Posted by: BayneSolo Posted at: 2019-10-18T22:29:59.110Z Reads: 101

```
![vesc|574x500](upload://yvcZgrkntIGEtavzLiIPM3pBWeF.png) 

And if I dont get a warning, I dont get any data from the IMU.
```

---
## \#454 Posted by: BayneSolo Posted at: 2019-10-18T22:32:30.115Z Reads: 94

```
Interesting, thanks for explaining it out. This whole i2c business is new to me so trying to wrap my head around its functionality.
```

---
## \#455 Posted by: BayneSolo Posted at: 2019-10-20T01:25:30.980Z Reads: 90

```
I have managed to get the master and slave hooked up correctly and its properly functioning. The biggest problem has been my ignorance on how the canbus functions (wrapping my head around forwarding etc in the app).

So now the problem is how to get the IMU data sent to the slave esc. I might have a go at hacking some code together but if someone has some better guidance on implementing that into the existing balance app then feel free to show me the way.
```

---
## \#456 Posted by: Jopj Posted at: 2019-10-20T01:38:40.405Z Reads: 87

```
I don't think you need to send IMU data. If the VESC with the IMU connected runs the balance app, it'll have some current it wants to drive the motor with. Just send that current command to the other VESC. Just like in normal dual motor mode, the receiver is connected to one VESC which passes the current command value to the other.
```

---
## \#457 Posted by: BayneSolo Posted at: 2019-10-20T01:40:12.349Z Reads: 84

```
Oh ok, that sounds a bit simpler then! Is there some command to enable current commands on the can?
```

---
## \#458 Posted by: Jopj Posted at: 2019-10-20T01:51:53.110Z Reads: 91

```
Yes

Some of the other apps such as ADC have the option of selecting "multiple vescs over can" which does just what you want, send the motor drive current command to the slave VESC.

I'm not very familiar with writing code for the VESC, but it should be possible to look through the source how the current command data packet is sent in those apps, most likely it's an oneliner or something close. They are the exact same packets I use with UART, just sent over CAN instead.
```

---
## \#459 Posted by: BayneSolo Posted at: 2019-10-20T01:52:42.367Z Reads: 87

```
boom! thanks for the guidance, I will have a dig and report back the findings :)
```

---
## \#460 Posted by: Jopj Posted at: 2019-10-20T01:56:17.082Z Reads: 89

```
It's done like this in the ADC app: comm_can_set_current(msg->id, current);

It needs this include in the app source file: #include "comm_can.h"

There are some checks it makes before doing that, which I don't know anything about. But that's how the current is set, in the end.
```

---
## \#461 Posted by: Jopj Posted at: 2019-10-20T01:59:11.216Z Reads: 91

```
I think it's reading through a list of all CAN IDs it has received, and sends that message to all of those IDs. This way no matter how many vescs there are, it'll send the command to all of them as long as they are sending something that has their IDs in it, most likely the "can status" stuff that can be enabled in vesc tool.

For a simple test you can set your slave vesc to some number and just send the current command to that ID.
```

---
## \#462 Posted by: BayneSolo Posted at: 2019-10-20T03:01:39.598Z Reads: 90

```
I've hardcoded in the commands where I believe they are supposed to be. Can someone [take a quick look](https://drive.google.com/file/d/1KW4CXU2ICZ8zQlZllKoAzJeXYK78U_u4/view?usp=sharing) at it and also compile it? I'm a bit stuck with setting up my compilers.

(I'm using 4.12 hardware)

Edit: I managed to find a linux vm and get it to compile. 

SUCCESS! I have it sending the signals over the CANBUS. It's not pretty right now and I think it needs tweaking but now that I know that I can do it, I'm so excited!!

Edit 2: Turns out the code works fine, I just had my motor config messed up. (Pro tip: Remove the CANBUS wire when doing the motor config wizard on motors that are physically connected ;) )
```

---
## \#463 Posted by: Fungineers Posted at: 2019-10-20T05:45:44.092Z Reads: 90

```
Has anyone been able to top 15km/h (10mph for the freedom eagles) on the phub-147/phub-188?
```

---
## \#464 Posted by: XtremeRacing Posted at: 2019-10-20T08:30:07.832Z Reads: 97

```
I’m working on my one wheel design while I am waiting for my motor to be shipped. I’m curious to find out what are dimensions and weight of people’s builds?
```

---
## \#465 Posted by: BayneSolo Posted at: 2019-10-20T09:03:05.932Z Reads: 96

```
![OneWheel%20Front|523x500](upload://AmiiRi8lG1JeaRadMZC9Dg1Q1Ht.png) ![OneWheel|690x292](upload://qVlb2UPMgseaqeq9ps3VBNEHj8z.png) 

I can't tell ya how heavy it is but its definitely not lite :joy:
```

---
## \#466 Posted by: NuRxG Posted at: 2019-10-20T09:36:23.481Z Reads: 93

```
Awesome that you figured it out.  It would be nice if you can get code to scan the bus for vescs on app start and write the current to all of the vescs, and submit a PR, so i don't have to do it :smiley:  Im sure other people will want to use this feature.
```

---
## \#467 Posted by: BayneSolo Posted at: 2019-10-20T09:49:30.972Z Reads: 94

```
haha maybe a little later, I'm coming up on final exams but after that I could have a crack.
```

---
## \#468 Posted by: Fosterqc Posted at: 2019-10-20T10:00:54.867Z Reads: 96

```
What do you all think of the larger wide ish hub motors that peipei sells?

https://peiscooter.com/13-inch-13x6-50-6-wide-tyre-double-axle-brushless-gearless-dc-scooter-hub-wheel-motor-can-with-disc-brake-phub-167g.html

https://peiscooter.com/15-inch-15x6-00-6-wide-tyre-hally-hub-motor-strong-power-bldc-phub-174.html

https://peiscooter.com/15inch-15-inch-15x6-00-6-tire-bldc-double-shafts-brushless-no-gear-dc-hub-lawn-mower-motor-for-scooter-diy-with-tire-phub-210.html

Funny tread
https://peiscooter.com/13-inch-13inch-13x6-50-6-wide-tyre-brushless-gearless-dc-hub-wheel-motor-for-many-diy.html
```

---
## \#469 Posted by: Jopj Posted at: 2019-10-20T13:49:26.336Z Reads: 96

```
Mine's a bit smaller, but quite heavy too since it's all metal and the rear segment is chock full of battery with scarcely a cubic centimeter to spare.

![dim|690x259](upload://A1kSaw6bM98rEX4313WZrlTnYGF.png) 

![dim2|690x392](upload://od6iFR55XN9KVBR4bXYlY66359B.png)
```

---
## \#470 Posted by: Jopj Posted at: 2019-10-20T14:05:48.253Z Reads: 97

```
What's your speed on the phub-188? What "voltage" version are you using? Since you are asking about 15 kmh, I'm thinking either you have the exact same one as me since you also had a 10s pack iirc. If you ordered any other voltage than 24, it supports my feeling that they're all the same. Very close to my 16 kmh, and I push the duty cycle a bit higher than the defaults in the balance app.
```

---
## \#471 Posted by: Fungineers Posted at: 2019-10-20T14:45:24.220Z Reads: 92

```
Well mystery solved.
I run 36V version with a 10S pack, and yes, Ive hit 16kmh before nosediving lol. 
Are you running 10s?
Still waiting for @Remieknaapen to run his 36V with 12S at full speed to confirm 16 is indeed topspeed.
```

---
## \#472 Posted by: Jopj Posted at: 2019-10-20T15:13:17.635Z Reads: 91

```
Yep, running 10s. On a 12s pack it'll go 20% faster, so around 19 kph then.
```

---
## \#473 Posted by: NuRxG Posted at: 2019-10-20T16:54:17.763Z Reads: 91

```
I have that last one but i never built a frame for it.
```

---
## \#474 Posted by: Fosterqc Posted at: 2019-10-20T18:48:15.099Z Reads: 92

```
Oh cool! Do you also have a phub 188? 
If so how do they compare? Same gauge wire?

They are pretty similarly priced, I've been comparing all their larger models and some are rated for higher voltage like 74v and some are rated for 1000W. 

I don't know if they have terrible documentation on purpose, or they don't think people want to see it...
```

---
## \#475 Posted by: XtremeRacing Posted at: 2019-10-20T19:20:31.122Z Reads: 90

```
I looked at larger wheels. My biggest hesitation was the wider foot placement because of the diameter of the tire. I ordered a 12" rim with a tire diameter of 430mm. I'm 6' tall. I don't think any wider would be comfortable for me.
```

---
## \#476 Posted by: XtremeRacing Posted at: 2019-10-20T19:49:40.499Z Reads: 91

```
My understanding is that most vescs can't handle more 60v.

In theory the lower voltage motor should be built to handle more amps at the rated watts.

I went with 36v 1200w motor. 1200w / 36v = 33.33 amps. A 72v motor will only need winds and leads able to handle half of that, 16.67 amps. It looks like if you order a phub-188 PeiPei ships the exact same motor weather you specify the 36v or 48v options. I’m not sure if that is the case for other motors. Since people have been able to over volt the PeiPei motors without them burning up or even getting hot I ordered the 36V and plan run a 12s  44.4v battery pack.
```

---
## \#477 Posted by: Jopj Posted at: 2019-10-20T20:01:24.386Z Reads: 86

```
The 24V version looks to be the same as the 36 and 48V ones as well. So I think I'm actually undervolting mine so to speak :no_mouth:
```

---
## \#478 Posted by: XtremeRacing Posted at: 2019-10-20T20:23:14.468Z Reads: 93

```
I watched your video on the motor. I agree with you the wires seem fairly light gauge for the current draw of the application. If they are pure copper they might be close. If the wires are CCA or aluminum they defiantly look like they are under rated. Since shielding thickness varies it’s hard to tell gauge without measure the copper if the wires aren’t marked. Are there any markings indicating the wire gauge?

I’m not sure if it will help or not. You might consider replacing the current leads with thicker gauge wire. The wire resistance might be limiting the current that the motor can draw effecting your max speed.
```

---
## \#479 Posted by: XtremeRacing Posted at: 2019-10-20T20:43:52.830Z Reads: 90

```
Thanks for the drawings they are in line with what I was thinking.
```

---
## \#480 Posted by: XtremeRacing Posted at: 2019-10-20T20:51:23.882Z Reads: 91

```
Does anyone known what the actual current draw of phub-188 is at full load maxing out the voltage with out burning up your vesc? [In other words how loud is it when you turn it up to 11?](https://www.youtube.com/watch?v=4xgx4k83zzc)
```

---
## \#481 Posted by: Jopj Posted at: 2019-10-20T22:40:43.885Z Reads: 89

```
The VESC is in no danger with this motor.I managed to get it to briefly draw 30A when stalled against a curb, but once it gets moving you'd really need more voltage to be able to push it. The higher the speed, the lower the current it can draw, and due to the low kV it really drops off fast.
```

---
## \#482 Posted by: XtremeRacing Posted at: 2019-10-21T02:05:41.747Z Reads: 87

```
I’m planning out my build. Since this is my first build any input, ideas or suggestions would me much appreciated. I ordered a 12” 1200w wheel which will require a decent size battery. I’m planning a 12s4p 18650 system. I’m wondering if 12s is going to be enough voltage to really get it moving. If I go any bigger will I risk damaging the vesc? NuRxG mentioned using capacitors to protect against voltage spikes. If I use capacitors as overvolt protection how close can I get to the vesc 6+ max of 60v before I risk burning it up? Is a 14 or 15s battery pack asking for trouble?
```

---
## \#483 Posted by: Fosterqc Posted at: 2019-10-21T02:06:44.536Z Reads: 89

```
I recommend you check out the thread on the superior forum about the 84v FOCer. That's what I want to use with a PEIPEI job motor, or if I decide to go belt/gear drive I would still use the 84v FOCer for better prefomace at all RPMs.
```

---
## \#484 Posted by: XtremeRacing Posted at: 2019-10-21T02:08:21.418Z Reads: 98

```
I do some metal fabrication. I have a welder, metal break and several other tools.  I want to make my onewheel as lightweight as possible while still having plenty of power to push my 200+ pounds uphill. My goal is to keep it under 33lb (15kg) I’d like it to be under 30lb (13.5kg) but that might be wishful thinking. 

I’m not sure how much weight the larger wheel and extra batteries will add. PeiPei doesn’t have the weight of the motor in the specs.  I’m planning on offsetting the extra weight somewhat with a unibody design. The deck will be bent to form the rails making it one piece.  That way I can use a whole lot thinner gauge aluminum. That should cut down on weight a little. I've got some thin aluminum diamond plate laying around, It’s about 0.01” or 2.5mm, converted to the world’s standard measurement. One that makes sense. I live in a county that still thinks that dividing the base unit of measurement by 12 is a good idea. I digress. 2.5mm aluminum should be rigid enough once I break a.k.a. bend it. I think I can get away with 11g (3.5mm) 2”x3” (50x75mm) steel plates for the axle mounts. 

The axle is pretty long on the 12” wheel, 340mm (13-3/8”ish). I might cut it down to so it’s not so wide. The width of the rim is 208mm. The total width of my rails shouldn’t add more than 1” (25mm) I think I can keep the total width of the board to 10” 250mm which seems to be pretty standard. Total length probably between 28-32” (710-810mm) that way hopefully everything will fit.
```

---
## \#485 Posted by: XtremeRacing Posted at: 2019-10-21T02:18:41.654Z Reads: 95

```
:thinking: Just when I was thinking I had one thing decided. I was going to go with a 6+. :smirk: Now I have to check out the FOCer 84v. :sweat_smile: Thanks for the heads up. :smiley:
```

---
## \#486 Posted by: Fosterqc Posted at: 2019-10-21T03:57:42.135Z Reads: 91

```
When you look at the thread you will see my interest, I'm trying to be at the front of the line to purchase.

Making a high voltage system sounds really fun.
```

---
## \#487 Posted by: Fosterqc Posted at: 2019-10-21T04:07:52.904Z Reads: 91

```
Peipei is so random with their documentation...

That 12" 1200W motor you linked has a photo of a screen with the CAD model and dimensions, why for just this one product?!?
```

---
## \#488 Posted by: doomy Posted at: 2019-10-21T10:40:58.662Z Reads: 91

```
I'm also planning on building a onewheel. If going with the phub188 motor i will use the a200s vesc. With that i should be able to go with a 16s pack.

http://teamtriforceuk.com/a200s-v2-2/
```

---
## \#489 Posted by: NuRxG Posted at: 2019-10-22T10:09:14.418Z Reads: 97

```
Wires look identical to me. Cant really say much more beyond that, i haven't used it, and i dont have a motor testing setup.

IMO all the numbers from china can be disregarded, just run any motor at the max voltage & watts your esc can handle.
```

---
## \#490 Posted by: Fungineers Posted at: 2019-10-22T17:20:55.207Z Reads: 98

```
lol. why you have to be callous all the time, Mitch. 
If you want to have the maximum amount of fun, follow this guy's advice (I do).
If your plan is to preserve the motor long term, running higher than rated watts (600W) could result in overheating the motor (since the coverplate is plastic, you will not feel the heat if you place your hand over the wheel cover. The heat is "trapped" in the wheel; this is the reason OneWheel now has a metal casing for the wheel covers).
If it is overheated for long, and repeatedly, the adhesive between the windings can (will) melt, and so will the adhesive holding the magnets to the hub. After this, you trash the wheel and order the 1200W motor :smiley:
```

---
## \#491 Posted by: Surfer Posted at: 2019-10-22T17:51:04.824Z Reads: 96

```
I will follow his advice about running it close to the max, and I will add the option to install a NTC thermistor (1$) to the motor windings connected to the vesc and keep the temp under control. Just the only important thing to know when you buy the thermistor is to known is 10K and the beta value to adjust your temp setting in vesc tool.
I used this and has been always perfect readings:

€ 0,62  10%OFF | 3950 NTC 10K Precision Epoxy Thermistor Temperature Sensor
https://s.click.aliexpress.com/e/e5eAMrfoJ
```

---
## \#492 Posted by: XtremeRacing Posted at: 2019-10-23T17:11:43.210Z Reads: 95

```
Some people are swapping out bearings on the there Onewheel XRs ether because of wear, play or because some of bearings that future motion puts or cheapo $5 bearings.

Bearings can effect the how smooth the ride is, speed, and motor life. Play in the bearing can cause the magnets to rub together as the motor turns causing damage. When I get my motor, the order status is still processing.:face_with_raised_eyebrow: 

I’ll probably test the factory bearings then swap them out to higher quality bearings to compare ride quality. I think the onewheel XR’s axle shaft is a lot wider diameter then PeiPei’s so I’ll I’m not sure the actual part #   bearings will work. SKF, NSK, Burris are some of the brands people are using. 

@Fungineers swapping bearings might get you a little more speed.
```

---
## \#493 Posted by: XtremeRacing Posted at: 2019-10-23T17:16:32.802Z Reads: 94

```
Unfortunately the new ones won't ship until December and the FOCers are still in development. :roll_eyes: Patients is not one of my virtues. I think I'll go with the 6+ for now. I should be able to get some speed put of it.
```

---
## \#494 Posted by: doomy Posted at: 2019-10-23T17:47:55.520Z Reads: 93

```
i just orderd the pcbs and soldered the a200s myself. it was quite the challenge and i managed to burn a few mosfets and a power board. i got one working now tough.
```

---
## \#495 Posted by: XtremeRacing Posted at: 2019-10-23T18:24:52.954Z Reads: 93

```
I don't know if I'm ready for that. Let me know how well it works.
```

---
## \#496 Posted by: doomy Posted at: 2019-10-24T06:54:38.672Z Reads: 90

```
Maybe you could try the cheap FOCer, you will get some soldering skills, its damn cheap (i built 5pcs for under 100$) and i run it on 13s all the time.
```

---
## \#497 Posted by: Byngham Posted at: 2019-10-24T14:32:51.082Z Reads: 94

```
I'm having the same sort if issue that Fungineers experienced in building the foot pads.  I've discovered that I can get the foot pad to be recognized as closed by pressing extremely hard in a couple of specific spots on the pads I made.  For the rest of the pad, it doesn't seem to matter how hard I press, I'm still not getting the switch recognized in the VESC software as being pressed.

I'm wondering if the pads that I built may have too much resistance.  Can anyone tell me what resistance the VESC expects to see in order to consider the switch closed?  I haven't been able to find that information anywhere.

Thanks everyone!
```

---
## \#498 Posted by: Jopj Posted at: 2019-10-24T14:40:26.181Z Reads: 92

```
The bearings on my phub seem solid so far, no weird noises and the motor is stable. If the bearings are bad enough that their friction has any noticeable effect on top speed, they'd get extremely hot very fast, and most certainly could be heard.
```

---
## \#499 Posted by: Jopj Posted at: 2019-10-24T14:42:43.411Z Reads: 91

```
I suggest testing the pads individually to see that they work. Arduino or anything that reads analog values + potentiometer is all that's needed. I'm pretty sure that there needs to be an external pulldown or pullup resistor, since the resistance of this type of pad is pretty low. Any internal pullup the vesc can manage won't be enough, those are in the range of tens of kOhm whereas with my pads I use ~60 ohms as pulldown.
```

---
## \#500 Posted by: Fungineers Posted at: 2019-10-24T15:00:13.383Z Reads: 94

```
I would have loved to conduct more experiments, but I couldnt be bothered. Maybe you can do it for us. 
1. Measure the resistance of your footpads.
2. Measure increasing resistances connected to the vesc, until you find the one that doesnt turn the vesc on. 
If 1 is > 2, then you know your problem. If not, check your connections. 

Also, let us all know whats 1 and 2 :slight_smile:
```

---
## \#501 Posted by: Byngham Posted at: 2019-10-24T15:05:06.340Z Reads: 96

```
I don't mind testing to see what mine read.  Should be able to do that before the weekend.  

I was just hoping there might be someone who could tell me "if you're not able to get the pad to return less than X ohms, the VESC software not going to believe the switch is closed...."
```

---
## \#502 Posted by: NuRxG Posted at: 2019-10-24T17:17:51.605Z Reads: 98

```
On velostat sensors pressing a small point often wont reduce the resistance as much as pressing a large area. Try actually stepping on it, rather than poking very hard with a finger. Cant promise it will help, but it's worth a try.

Also another interesting sensor alternative worth noting is that [car seat sensors](https://www.ebay.com/itm/Universal-Car-Seat-Pressure-Sensor-Safety-Belt-Warning-Pad-Occupied-Seated-Alarm/113707619731?_trkparms=aid%3D111001%26algo%3DREC.SEED%26ao%3D1%26asc%3D20160908105057%26meid%3D538d2ec0efec4ebdaf4837f51377f701%26pid%3D100675%26rk%3D3%26rkt%3D15%26sd%3D292894374147%26itm%3D113707619731%26pmt%3D1%26noa%3D1%26pg%3D2380057&_trksid=p2380057.c100675.m4236&_trkparms=pageci%3A109d33f8-f682-11e9-87a1-74dbd180afaf%7Cparentrq%3Afec55a3616d0a4b7b7150876fff7511f%7Ciid%3A1) are super cheap and cover a large area. Not sure how practical they are for fitting 2 on a single footpad, but the price is hard to beat.
```

---
## \#503 Posted by: Byngham Posted at: 2019-10-24T21:54:53.424Z Reads: 97

```
I like the way you think there.  I've got a couple of car seatbelt pressure sensors on the way, and will try them out.  Found one that was something like 7" x 3", with another 3" tail extending before it connects to wires.  We'll see how they work out.

I'll also see how the velostat works with stepping on it.  We'd been afraid to step on it, since we've not gotten off the bench yet.  Can certainly try setting it up on blocks on the floor, and step on the sensors without fear of having it take off on us.  Thanks for the advice.
```

---
## \#504 Posted by: BayneSolo Posted at: 2019-10-25T06:48:55.010Z Reads: 96

```
Anyone with vesc flashing experience, can you take a look at this? Happened to my master vesc while riding.

https://vesc-project.com/node/1412
```

---
## \#505 Posted by: Sindre Posted at: 2019-10-25T09:18:25.199Z Reads: 101

```
Hi Bayne, use the stlink utility to perform an mass erase. It would give good pointers if something is wrong with the mcu. https://www.st.com/en/development-tools/stsw-link004.html
```

---
## \#506 Posted by: Groovr Posted at: 2019-10-25T09:33:33.045Z Reads: 103

```
Hi all,

Have anyone had a look at the PHUB-144 hub motor? I was searching for a hub motor for my project and found it. As the original onewheel uses tires that are 11.5x6.00-6 it seams like using this hub motor should enable the use of the same tires. My main concern is that it looks quite bulky on the wire side.

(I am not allowed to post links but if you search for PHUB-144 on peipei scooter you will find it)
```

---
## \#507 Posted by: BayneSolo Posted at: 2019-10-25T09:45:30.893Z Reads: 98

```
I'm unable to mass erase, it says that the device is protected and that its unable to erase. I thinking the mcu is gone, I've ordered a new one but will continue to mess around with trying to get it working.
```

---
## \#508 Posted by: Surfer Posted at: 2019-10-25T10:37:34.911Z Reads: 97

```
Sometimes the MCU can hang, try to use reset pin 7 to ground for reset.
```

---
## \#509 Posted by: Fosterqc Posted at: 2019-10-25T15:52:22.610Z Reads: 102

```
Yeah another person was asking about it.

https://www.peipeiscooter.com/mini-halley-motor-48v-60v-brushless-dc-wheel-hub-motor-450w-phub-144.html

Probably would be able to compare and contrast between the specs of the phub188 if pepe decided to actually give you the stupid specifications.
```

---
## \#510 Posted by: Groovr Posted at: 2019-10-25T16:34:00.854Z Reads: 96

```
Looks like the phub-174 is the same with a fitted tire. But specifications are scares, even the different images on the product page does not line up.
```

---
## \#511 Posted by: BayneSolo Posted at: 2019-10-25T21:49:58.985Z Reads: 95

```
Reset pin 7 on the st link to ground on the vesc??
```

---
## \#512 Posted by: Surfer Posted at: 2019-10-26T19:37:08.957Z Reads: 99

```
Sorry mate, I droped the post like it's hot.
![44049020-7dd052ea-9f22-11e8-82e1-610df77df32f|625x417](upload://6siSh0d23rJmblU69yAt3QU3xTZ.png) 
I did have same or similar problem, I couldn't flash because protected memory or sometimes can't connect to the target, this worked for me I hope to you too,
The thing is to short pin 7 of the st32 to ground on vesc, while connecting for flash, I haven't succeed with openocd, but it worked well with a cheap STlink.
```

---
## \#513 Posted by: XtremeRacing Posted at: 2019-10-26T22:58:52.939Z Reads: 91

```
I have some soldering experience but I'm not overly confident in my surface mount skills. Maybe I'll get a heat gun and give it a shot. Which cheap FOCer do you think I should get?
```

---
## \#514 Posted by: XtremeRacing Posted at: 2019-10-27T00:52:14.822Z Reads: 94

```
My order status was still processing on in my Pei account so I emailed Pei about the order status. 

Pei’s Response, 

“After your payment.We have arranged the production,Now still not finish.We try to be quickly.
Because the weight of this motor wheel is nearly 18kgs,So we will delivery by UPS or Fedex special line.It will not be fast,in general need 18 days.And you don’t need pay any customs duties.” :astonished:

I guess my goal of keeping the board under 15kg is out the window…I figured the tire would be steel belted and the larger motor would add weight, but damn. Maybe I should have gone with the phub-238. :disappointed:

On the bright anyone trying to steal will wind up with one hell of a hernia when they try and pick it up.  

Her English isn’t great.I guess you don’t need spaces after punctuation after all.Maybe she meant lb instead kg.I doubt it.Fingers crossed.
```

---
## \#515 Posted by: BayneSolo Posted at: 2019-10-27T02:11:41.914Z Reads: 90

```
Unfortunately that doesn't work, at least with my raspberry pi setup. I think the next route to try is getting an actual st link.
```

---
## \#516 Posted by: doomy Posted at: 2019-10-27T06:44:04.800Z Reads: 91

```
The last version with the hole under the DRV chip for easy soldering. There is a thread with more info over at esk8 news. Yeah it works best with the heat gun, soldered the a200s control board this way with ease.
```

---
## \#517 Posted by: XtremeRacing Posted at: 2019-10-27T19:56:46.325Z Reads: 94

```
I've been looking at [Shaman's cheap FOCer github page.](https://github.com/shamansystems/Cheap-FOCer) I think I might give it a shot. I have several projects in mind that I think it will work well for. While I do have some basic electronics experience my knowledge of FOC in practically nonexistent. I don’t think I’ll have a problem using the cheap FOCer on an ebike. I don’t know how to integrate everything needed use NuRxG’s balancing function. The cheap FOCer is based on VESC 4.12. I read somewhere that trying to flash VESCs to newer firmware can brick them. What firmware are you using? Have you used the balancing function of the vesc-tool directly with the cheap FOCer you built?
```

---
## \#518 Posted by: Fungineers Posted at: 2019-10-28T10:28:41.975Z Reads: 90

```
If your mcu is being detected by the stlink software, then 99% its a good mcu and can be fixed. Dont waste that good mcu.
Also, you dont need to reset it using hardware, there is a RST pin on the vesc on the same connector that you can connect to RST on the stlink. 
Once done, try to 'connect under reset'. Once done, erase the whole chip and flash the bootloader on it. 
Good luck!
```

---
## \#519 Posted by: Groovr Posted at: 2019-10-28T12:44:01.462Z Reads: 90

```
One small thing I wish someone had told me. If you get a cheap knock off st-link from ebay, verify the pinout of the st-link. It took me two weeks of pulling my hair before I found a forum where someone pointed it out. The printed pinout on the case was not the same pinout as on the circuit board, once connected according to the circuit board I could connect and reprogram.
```

---
## \#520 Posted by: XtremeRacing Posted at: 2019-10-28T15:58:49.908Z Reads: 93

```
There is some great info in this thread it is really helping me plan out my board. 

:thinking: I’m curious what people’s think about their completed builds. What components they used, how they preform, what people like, what they, and what they would change on a future build.
```

---
## \#521 Posted by: Groovr Posted at: 2019-10-28T16:21:42.126Z Reads: 95

```
I built mine with parts from a hover board inspired by ZbLaB.

Not using iron for the frame. Next will be Aluminum. The choice made it a lot heavier but I could not source aluminum locally.
Using a proper controller. I'm waiting for a Vesc 6+ in the mail so have sorted that. The hoverboard controller with a custom and very much hacked firmware works but a long way from ideal.
And a better hub motor than the two hoverboard motors bolted together. Getting the right balance and to get the motors to work in parallel was not the easiest of tasks and are still not fully ok.

So the short answer, everything but the griptape and the paint. :smiley:
```

---
## \#522 Posted by: BayneSolo Posted at: 2019-10-28T21:26:06.248Z Reads: 92

```
Interesting that you had balance problems with the two hoverboard motors. How did you connect them? I personally went that route with two Vesc 4.12's and havent had any problems (Other than a vesc shitting the bed but thats a different story :joy:)

I connected my two motors with a 3d printed spacer, with m6 threaded rod to connect to two outer bells and also some thinner rod just in the spacer, balance wasn't an issue at all.
```

---
## \#523 Posted by: Groovr Posted at: 2019-10-28T21:49:00.821Z Reads: 99

```
To get them lined up and running smooth was a problem at first. I ended up having one axle loose and connect power to both on the opposite winding. Let’s just say that solved the issue quite violently, the loose one kicked in place and I bolted it down. Now they run smooth. Took a while before I got the idea to let the windings “self align” that way.

And they are both connected in parallel on the same motor output. This free up a lot of port and clock cycles to do other stuff :smile: basically half of the controller functions removed (gyro reading/hall reading).
```

---
## \#524 Posted by: BayneSolo Posted at: 2019-10-28T22:04:46.483Z Reads: 101

```
Interesting, so you have one esc controlling two motors?
```

---
## \#525 Posted by: NuRxG Posted at: 2019-10-28T22:18:28.119Z Reads: 105

```
I haven't seen anyone talking about this so i thought id share. Looks pretty cool, but at the same time i don't think I'm ready to spend 600$ on one.

https://www.ebmakers.com/collections/x-esc/products/100a-200a-based-on-vesc6-high-power-esc
```

---
## \#526 Posted by: Groovr Posted at: 2019-10-29T06:07:12.619Z Reads: 102

```
Yes, it will cut the resistans for the windings in half but as long as the output FETs can take the power output and the magnets/windings are aligned it works quite well.
```

---
## \#527 Posted by: doomy Posted at: 2019-10-29T13:12:33.423Z Reads: 99

```
I'm using the newest offical 4.12 firmware on it, ackmaniak works also.

Did not try with MPU yet..
```

---
## \#528 Posted by: NuRxG Posted at: 2019-10-30T09:50:12.430Z Reads: 100

```
Woah, there is a 400v vesc out there.

http://www.powerdesigns.ca/
```

---
## \#529 Posted by: Fosterqc Posted at: 2019-10-31T01:07:51.329Z Reads: 101

```
I forgot to post this like 5 times, but I'd really like to see a diy OW build with a real hypercore motor (preferably with 16S+) 
![Screenshot_20191029-163026_Facebook|281x500](upload://kf4QPX1pFb1keycHckDqB9WEhPO.jpeg) 

This guy's selling them for almost reasonable prices (these are brand new tho getting a deal on a parted out broken one would be cash)

I really want to know how interior the peipei motor probably is.

Last point is that you could probably get a way more baller hub motor from China for that money... So it doesn't quite make sense to buy a hypercore motor new.

Thoughts on this?
```

---
## \#530 Posted by: NuRxG Posted at: 2019-11-01T03:12:42.324Z Reads: 99

```
Not my build, but here ya go!
![IMG_20190929_152437|666x500](upload://aQl88nk9pSWpQIJzOhJ57b0jLOl.jpeg)
```

---
## \#531 Posted by: time Posted at: 2019-11-02T01:14:28.467Z Reads: 96

```
I know everyone's setups are different, but I'm curious what settings others have set in the VESC Tool Balance App (well those who are using it).  Could some of you who have completed your builds share them?
```

---
## \#532 Posted by: SwarleyAUS Posted at: 2019-11-04T01:01:29.298Z Reads: 97

```
These are my settings:

![image|690x431](upload://c5I4bKnOLT4K7lXWwFFtMpu4wPl.png) 

Questions for @NuRxG though around some issues I am having:
- When I turn on the board sometimes it's not getting IMU data, any idea why (using MPU6050)? Rebooting the VESC through VESCtool fixes it, but out in the field I sometimes have to remove and reapply power 3 or more times! Could be a connection issue though, I will look into this.
- Is there any limit on the range of the PIDs? There seems to be no difference in setting the D to 100 or 500.
- Because I have my MPU6050 upside down, I have a 180 degree offset applied to the roll axis. Sometimes however the Balance app IMU data will seemingly lose this offset and appear rolled by 180 degrees as oppose to 0 as seen below. I think this is playing into the issue in my first question... any idea why on this too? I think it is occurring after I release the footswitch.

![image|690x431,100%](upload://5IN7mGbsGZnZRliTwIFQp161JD5.png)
```

---
## \#533 Posted by: time Posted at: 2019-11-04T04:15:24.420Z Reads: 95

```
Thanks! I'm just starting to play around with the tuning and it's proving to be...challenging.
I'll definitely give yours a try.


For anyone who is putting off building one because you don't think yours would turn out nearly as good as the others on here (seriously, you guys are amazing!), I would like to lower the bar.
Presenting my "WoodWheel":

![woodwheel|690x335](upload://h7C6jFN97IvkR1o4sdUu0TZQglm.jpeg) 

Eventually I'll get the body machined and all nice, but for now all I had was scrap wood (and a little bit of aluminum).  If you look closely you'll notice the high quality float plates as well lol.
```

---
## \#534 Posted by: SwarleyAUS Posted at: 2019-11-04T05:04:30.374Z Reads: 94

```
Mines no less a woodwheel than yours! Wood is good... Absorbs vibrations better! ![15728436972605151647258173117444|666x500](upload://2ZF2hsayuptN3nGDD1U2pQGAak5.jpeg) 

In the process of changing my rails to 50x25 aluminium and adding covers underneath ATM tho
```

---
## \#535 Posted by: NuRxG Posted at: 2019-11-04T07:48:50.975Z Reads: 92

```
I know you wanna raise your board for ground clearance, but i believe if you lower your rails below the mounting holes, it will balance better. (try both and draw your own conclusions tho)
```

---
## \#536 Posted by: NuRxG Posted at: 2019-11-04T08:06:52.119Z Reads: 100

```
I've seen the imu occasionally not have the right orientation on a bootup, but that hasn't happened to me in a long time, don't think I've seen it on the latest code base. It also only happened on a boot.

Ive never seen the imu need a few reboots to work. I hope it is a wiring issue. 

There is a series of things that need to happen in a specific order, to get everything right, such as load app config, config imu, read settings and apply offsets, modification of madgwick parameters for quick initial setup, then restoration of config parameters, and then the balance app can start. If the imu is not connected or is getting connected late, it may be throwing things off. 

The imu code shouldn't have anything to do with the balance code, they're 2 unrelated parts. The balance app just reads values from the imu "app". It isn't controlling the imu or changing anything. That doesn't mean any part of the code is bug free.

But in general i have not seen these issues. I'm mainly using internal imu.


I didn't code any upper limits on the PID values, however if your chain has some play, i can see how that would diminish the effects of the D value. More so gut feeling and intuition than mathematically so don't ask me to back this claim up :-P

Sorry im not more helpful, you're the first person to report this imu connection issue, and i haven't seen it myself. If multiple people are experiencing it, and there are exact reproduction steps, I'll be happy to fix it.
```

---
## \#537 Posted by: SwarleyAUS Posted at: 2019-11-04T09:15:22.385Z Reads: 90

```
Cheers for the response and a bit of a look behind the curtains =)
```

---
## \#538 Posted by: time Posted at: 2019-11-05T02:52:54.715Z Reads: 96

```
I'm loving the chain drive! It looks really clean.  I can't wait to see how it looks after the change.

@NuRxG Sadly the board only sits so high because when I attempted to mount the wheel's axle straight to the wood rail I was using it snapped in half haha.
Instead of taking the time to do it right I decided to make a separate mount that the rail would sit on top of.  Ironically having it that high worked out best as the wood I used made my board super thick...

Definitely is the plan to mount lower in my rebuild now that I know all the parts work.
```

---
## \#539 Posted by: Pierrotds Posted at: 2019-11-06T16:42:17.193Z Reads: 95

```
Hi guys, I'm planning to start to build my own onewheel to soon so I'm joining the thread.

So I'm starting to make my plans on fusion 360 and I would need your help. 
First of all I'm gonna like mainly everybody gonna use the peiscooter hub but I'm still wondering how I'm gonna be attaching it to the aluminum profiles in a secure way. Do you guys have some ideas ? 
Next, what do you guys think is the best voltage for the board ? I think 12/13s could allow a good speed ? And if you have some good batteries to recommend me it could be awesome !
And finally,  it's more of a software idea I had. If I'm following correctly the speed is linear to the angle of the board ? Wouldn't it be a good idea to try to make it exponential to the angle ? It would allow the board to be faster with less angle ? I'm mainly speaking tu @NuRxG (And thanks for the amazing job of implementing the balance into the vesc project !) do you think it could be possible and interesting ? 

Thanks for the help !
```

---
## \#540 Posted by: NuRxG Posted at: 2019-11-06T18:32:42.175Z Reads: 100

```
I don't need to justify my maths to nobody!
 
![giphy|320x275](upload://27NORPhTduOPqQGWhJpmY197psg.gif) 


Seriously tho, make a build, try the software. If you think you can improve it, go for it, its open source. I would love for it to work better. 

Im not a mathematician and PID is the go to for basic control loops. LQR seems like another good option for more tuneability. To me it just sounds like you're trying solve a problem that doesn't exist before you even attempt to see if it exists. Then tagging me and expecting me to somehow defend my system that works fine vs some other hypothetical system I've never tried is just unfair to me. I get that you're new and excited and trying to help, but I'm in over my head, and just trying to make sure there are no bugs that result in deaths :skull_and_crossbones:  . 

You're not the first person without a build or ever trying to run self balancing code that has suggested things, so I'm a bit jaded/over it. Sorry for the rudeish response, but it is simply unreasonable for me to code and then test every idea that everyone has, or mathematically prove the same. I think exponential is a great idea for you to try! However firmness is more limited by the sensor fusion math than the pid math, and also **not a problem**. My EUC is incredibly firm (that doesn't mean exponential won't be better, go for it).
```

---
## \#541 Posted by: SwarleyAUS Posted at: 2019-11-08T05:40:46.607Z Reads: 94

```
I bought two of these to try out. They will need to be cut to size at about 250x300mm each. Resistance wise they are great though... 

Open circuit resistance: >200k ohms<br>
With 30kg applied to half of the pad area: <30ohms<br>
With 30kg applied to the whole pad: <20ohms

15-20ohms seems to be about the minimum resistance at about 50kg. There's about 5-10 ohms delta between the two pads I bought.
```

---
## \#542 Posted by: kossojan Posted at: 2019-11-10T00:22:08.243Z Reads: 93

```
Hi
am am also building one, unfortunatly i can't post image or links...

The biggest challenge was communication with PeipeiScooter. First no responses, then wrong tracking numbers, excuses and so on, but after 6 weeks, i received the motor.

To mount the motor i designed a small metal plate and had it laser cut out of 5mm steel. It was actually very affordable, one plate costs arround 6€ including shipping.
It is designed to fit into the slots of a 30x60 alumunium extrusion, but will later be cut to cut a 40mm thick walled aluminium tube. 
@Pierrotds: 
I will cut a 32mm hole into the 40mm beam for the axle and the nut. My plate will bolt  inside the frame to hold the motor. The plate itself will get M6 internal threads and the screws bolt the plate to the inner wall of the frame. The holes on the outside are 10mm (to fit the screw caps) and the inner wall will have 6.2mm holes (for the screws to go through). 


For the first tests i used a wooden frame and the following items:
Flipsky 4.12 VESC
MPU6050 Breakoutboard
Button with long cable as foot switch replacement
9S2P  INR18650-15Q (high current battery from a robotic lawnmower, was extremly cheap)

First rides:
-link removed-

It works surprisingly well, but i believe the 9S battery's voltage is too low to get a realiable balancing at higher speeds. So the final board will get a 12S2P battery.

My next step is building an aluminium frame out of 40x20x3mm hollow tube and 40x10mm bar stock.
```

---
## \#543 Posted by: Fosterqc Posted at: 2019-11-10T07:46:27.095Z Reads: 98

```
I like to sort their AliExpress page new to old to see what the person writing their posts is up to...

US $149.00 | 10inch 10*6.0-5.5 tire BLDC brushless gearless electric scooter hub drive wheel phub-510
https://s.click.aliexpress.com/e/oz7Xp4pi
![20191109_233849|314x500](upload://lHZmjvM3SWC8GU8YVm9BzkGdf1a.jpeg) 

Seem to be getting better at posting specs. I mean look at all those numbers! Diagram for this one too.

Looks like it would be cool for a larger Funwheel.
```

---
## \#544 Posted by: Pierrotds Posted at: 2019-11-10T16:15:06.787Z Reads: 95

```
I found those ones on aliexpress I was planning to use 2 of them for the left sensor and 2 others for the right sensor but its more expensive. Looking forward to see how it is going to be for yours.

https://www.aliexpress.com/item/32955734979.html?spm=a2g0o.detail.1000014.28.11a9169fjB3DuN&gps-id=pcDetailBottomMoreOtherSeller&scm=1007.13338.141932.0&scm_id=1007.13338.141932.0&scm-url=1007.13338.141932.0&pvid=ed29eb6e-cdee-419e-82fa-fe60ef900929
```

---
## \#545 Posted by: Fungineers Posted at: 2019-11-11T18:26:00.595Z Reads: 94

```
A large funwheel sounds like..fun, but needs a larger wallet too :frowning:
```

---
## \#546 Posted by: Fungineers Posted at: 2019-11-11T18:27:05.682Z Reads: 91

```
These work but are very sensitive...also very expensive as you said. Not worth it imo
```

---
## \#547 Posted by: Fungineers Posted at: 2019-11-11T18:29:44.132Z Reads: 90

```
To everyone who is planning to buy a peihub or is in the process, peihub will claim that it is going to send the wheel through UPS expedited (which costs a fortune), but often times, they end up sending through aramex slow mail. I disputed this and was able to get a $20 refund since they didnt send as per the service I paid for, and it was late. 
Buy yourself some footpads. Lol.
```

---
## \#548 Posted by: Fosterqc Posted at: 2019-11-11T20:25:03.656Z Reads: 87

```
Yeah they're up to some funky stuff and I don't like them very much.
```

---
## \#549 Posted by: NuRxG Posted at: 2019-11-12T03:28:32.800Z Reads: 91

```
When i ordered my motor from pei, they never shipped it, and eventually i got a refund after a month or two. Instead i ordered the same motor from a different seller.
```

---
## \#550 Posted by: Pierrotds Posted at: 2019-11-12T06:01:11.472Z Reads: 90

```
Did you bought it from aliexpress or from the pei website ?
```

---
## \#551 Posted by: Fungineers Posted at: 2019-11-12T06:12:45.605Z Reads: 87

```
Aliexpress, since I dont trust them to order directly. With Ali, at least refund is guaranteed in case of no-receive.
```

---
## \#552 Posted by: Jordicious Posted at: 2019-11-12T20:11:48.392Z Reads: 89

```
Wow, I honestly never would've expected a DIY OW to be even possible.

Massive respect to you sir.
```

---
## \#553 Posted by: beherit Posted at: 2019-11-15T23:13:22.938Z Reads: 86

```
I **love** seeing these, keep 'em posted!

It'd be nice to have a different term for DIY OneWheels, since its a brand and all.
```

---
## \#554 Posted by: Groovr Posted at: 2019-11-16T07:37:14.387Z Reads: 88

```
What seller did you end up using?
```

---
## \#555 Posted by: NuRxG Posted at: 2019-11-16T19:56:14.108Z Reads: 91

```
https://www.aliexpress.com/item/32817514024.html?spm=a2g0s.9042311.0.0.6fe14c4d4NoAVP
```

---
## \#556 Posted by: Pierrotds Posted at: 2019-11-17T19:52:37.647Z Reads: 87

```
And compared to the pei wheel what do you think ? Better or worse or the same ?
```

---
## \#557 Posted by: NuRxG Posted at: 2019-11-17T20:42:11.145Z Reads: 87

```
i only have one. But it looks like the same thing, i have no reason to suspect its not coming from the same factory.
```

---
## \#558 Posted by: Pierrotds Posted at: 2019-11-17T21:02:44.718Z Reads: 85

```
Yeah looks to me exactly the same. Still looking for another option otherwise I will go for the peiscooter one I think
```

---
## \#559 Posted by: Remieknaapen Posted at: 2019-11-18T21:08:55.977Z Reads: 88

```
Guys, i have got my board up and running!
I'm using 12s2p at the moment. Top speed is 19Km. Range is still hard to figure out because of the low temperatures here. But i guess somewhere between 10 to 18Km. All up weight of the board is 9.8Kg.

I made a small video for you as well, let me know what you think of it!

https://youtu.be/00XBdZNgJ3c
```

---
## \#560 Posted by: s.white432 Posted at: 2019-11-18T22:10:13.391Z Reads: 86

```
Very nice! I'd be keen to see more details around its components and construction. How does it perform on inclines?
```

---
## \#561 Posted by: Surfer Posted at: 2019-11-18T22:20:50.901Z Reads: 86

```
I still have to post my settings but just I saw that you have this springy effect too, i set confidence decay to 0 and it was really noticeable riding improvement even in bumpy roads.
```

---
## \#562 Posted by: Byngham Posted at: 2019-11-18T22:36:49.112Z Reads: 89

```
It's been a while since I was able to work on the project.  Life happens.

I got in the car seat sensors like NuRxG posted about (actually what I got were [these on Amazon](https://www.amazon.com/dp/B07JK9M7YR/ref=cm_sw_em_r_mt_dp_U_SVX0DbAVQEWVF) ).  They were pretty easy to search for, and that particular model were a size that I could fit two side by side on my foot pad.

Hooked them up to my Vesc, and they work perfectly first try.  Thanks NuRxG!!
```

---
## \#563 Posted by: Byngham Posted at: 2019-11-18T22:44:32.518Z Reads: 88

```
Now that my foot sensors are working, I've run into another problem.  When I try to test out the unit, I step on the footpads, the motor starts to spin up, and within a half second the vesc shuts down.  I've managed to reproduce the issue while connected to a laptop, and in the Debug Console we're getting this error:

![image|690x87](upload://bTRn85bHmtnTN2mxa8ZG6VGFKGy.png) 

Any ideas?
```

---
## \#564 Posted by: Fungineers Posted at: 2019-11-19T03:30:02.639Z Reads: 87

```
Set your duty cycle cutoff to 1.0 in the Balance App.
```

---
## \#565 Posted by: Fungineers Posted at: 2019-11-19T03:35:04.202Z Reads: 87

```
Im disappointed..because the video is only 1 min long.
I think we all need more footage of the Monowheel in action. 
Also I think that's the fastest the phub188 has gone. 
Great job, and waiting for more board closeups and ride videos.
```

---
## \#566 Posted by: Remieknaapen Posted at: 2019-11-19T09:03:25.136Z Reads: 86

```
It does handle inclines pretty good! In the video on 0.30s I'm going uphill on a 10 degree angle.

@Surfer, I gave it a quick go yesterday evening and it really does make a improvement. Was only able to test it inside because of the bad weather over here. Can't wait to ride it outside again.
```

---
## \#567 Posted by: NuRxG Posted at: 2019-11-19T18:38:11.746Z Reads: 85

```
Are you using BLDC or FOC? If BLDC try FOC?
```

---
## \#568 Posted by: Fosterqc Posted at: 2019-11-19T21:42:06.223Z Reads: 83

```
16Kv will do that to you.

It's really funny how all these Phub Funwheels look like OW pints if you don't look closely. Definitely looks great!

I like it.
```

---
## \#569 Posted by: Byngham Posted at: 2019-11-19T22:45:03.453Z Reads: 80

```
@Fungineers -- The duty cycle setting had been at 0.9.  I thought I'd had issues trying to set it to 1.0 previously, but it seemed to take this time around.  Unfortunately, it didn't change the behaviour.  I'm still having my vesc shutdown after about a 1/2 second of trying to power up the motor (with the motor up on blocks).

@NuRxG -- The vesc is setup for FOC.  I had the vesc re-sense the hall sensors and such, but that also didn't improve things any.

Is it possible that something's just gone wrong with my vesc, and it needs to be replaced?
```

---
## \#570 Posted by: NuRxG Posted at: 2019-11-19T23:24:25.606Z Reads: 81

```
Does this only happen with the balance app or can it be reproduced with other control methods?

Maybe we should take this to DM
```

---
## \#571 Posted by: Fungineers Posted at: 2019-11-20T04:29:40.239Z Reads: 81

```
I dont suspect anything wrong with the VESC. 
I would just put it on the ground and ride it and see if that makes a difference.
```

---
## \#572 Posted by: Remieknaapen Posted at: 2019-11-20T11:05:01.228Z Reads: 77

```
What do you mean by 16kv will do that for you. Get more speed?

 I'm thinking about opening up the phub188 to see if i can rewind it or change it from star to delta config to gain more speed (factor 1,7 if i'm correct).
```

---
## \#573 Posted by: Fosterqc Posted at: 2019-11-20T23:09:48.460Z Reads: 79

```
Low Kv = high torque = good fast hill climbing

Buuut crappy top speed unless you have a very high Voltage setup. I actually like that the Phub is low Kv you could run it on 100V and it would be awesome I think.
```

---
## \#574 Posted by: Fungineers Posted at: 2019-11-21T07:37:43.825Z Reads: 79

```
I would like to know from people using the MPU6500. 
How has your experience been? 
Has someone tried both MPU6500 and MPU9250. Perhaps @NuRxG. Any noticeable  difference?
```

---
## \#575 Posted by: Pierrotds Posted at: 2019-11-21T11:12:43.036Z Reads: 80

```
I have mpu6500 but I can't make it work with the vesc. The software only accepts the 9X50 I think and I don't know how tu make it work so I bought a 9250 in the end.
```

---
## \#576 Posted by: SwarleyAUS Posted at: 2019-11-21T21:44:44.280Z Reads: 81

```
Yes it doesn't seem there is a way to 'test' the VESC & balance app without a load, ie if it is not on the ground it will switch to 'Dead' mode quickly. I would love to change this, particularly for novices & testing settings. I don't see any need for the board to go to this 'Dead' mode if it not on the ground...
```

---
## \#577 Posted by: SwarleyAUS Posted at: 2019-11-21T21:46:30.334Z Reads: 75

```
I will have tried both soon. Think my current 6050 has died. Hoping my power up issues whereby the board gets stuck on 'Calibrating' will be resolved by changing to the 9250.
```

---
## \#578 Posted by: SwarleyAUS Posted at: 2019-11-21T21:47:55.483Z Reads: 77

```
6050 was working for me (intermittently). Maybe you were having the issue I am which is that sometimes you need to reboot the VESC a few times for it to get good comms with the IMU
```

---
## \#579 Posted by: Fosterqc Posted at: 2019-11-21T22:03:05.168Z Reads: 77

```
Let's see the guts :upside_down_face:
```

---
## \#580 Posted by: Pierrotds Posted at: 2019-11-22T17:46:56.813Z Reads: 77

```
How have you made it word with ? Vesc tool only shows for 9X50 or I'm crazy ?
```

---
## \#581 Posted by: Pierrotds Posted at: 2019-11-24T11:24:03.133Z Reads: 82

```
Just found this wheel looks like it goes up to 800W could be interesting. Anyone has already tried it ? I know peiscooter sells it to but this one gives us more information on the sizes.
https://www.aliexpress.com/item/33009640417.html?spm=a2g0o.detail.1000060.1.77d846f8WdY9lG&gps-id=pcDetailBottomMoreThisSeller&scm=1007.13339.146401.0&scm_id=1007.13339.146401.0&scm-url=1007.13339.146401.0&pvid=5fbd5902-25ae-4757-8ca8-f549508e1d9d
```

---
## \#582 Posted by: SwarleyAUS Posted at: 2019-11-24T22:17:59.033Z Reads: 79

```
It uses the same protocol, so MPU6050 should work when you choose MPU925X
```

---
## \#583 Posted by: Pierrotds Posted at: 2019-11-25T09:26:27.197Z Reads: 79

```
Yeah I found what wasn't working thanks !
```

---
## \#584 Posted by: NuRxG Posted at: 2019-11-26T21:17:21.333Z Reads: 79

```
I have that motor with a diferent tire but ive never tried it. too lazy :sleeping:
```

---
## \#585 Posted by: clumsylyric Posted at: 2019-11-27T02:22:31.726Z Reads: 78

```
What do the P I D values for the balance app do? I'm using a VESC and MPU 6050 based on @Fungineers build with pei pei 36v 600W motor. I don't know how to use the VESC Tool so could somebody with a similar setup reply with their settings? I've been trying but nothing seems to work.
Thanks!
```

---
## \#586 Posted by: jwhite Posted at: 2019-11-27T02:53:16.853Z Reads: 78

```
Hi all! I just began working on my own diy onewheel and I was just wondering what type of VESC y'all would would recommend, as well as any other tips or suggestions for building? Thanks!
```

---
## \#587 Posted by: SwarleyAUS Posted at: 2019-11-27T03:32:53.374Z Reads: 82

```
PID intro: https://www.youtube.com/watch?v=wkfEZmsQqiA

In short:<br>
P or Proportional gain affects how much corrective action a system applies when not at the set point, at an instantaneous point in time.<br>
I or Integral gain affects how much corrective action a system applies when not at the set point, for a consistent period of time.<br>
D or Derivate gain affects how much corrective action a system applies when not at the set point, based on the current rate of deviation from the set point.

Hopefully my explanations are correct!

These are my settings.

![image|690x431](upload://5IN7mGbsGZnZRliTwIFQp161JD5.png)
```

---
## \#588 Posted by: clumsylyric Posted at: 2019-11-27T04:05:28.577Z Reads: 76

```
Thanks! Currently work on my onewheel. With your settings I got it kind of working. Still too jerky
```

---
## \#589 Posted by: SwarleyAUS Posted at: 2019-11-27T04:45:25.821Z Reads: 75

```
You may will need to 'null' any noise of offsets on the IMU page of the tool too. Start with increasing P gain until it is enough to correct and correct firmly, then add D gain to smooth.
```

---
## \#590 Posted by: webst Posted at: 2019-11-27T05:27:38.437Z Reads: 75

```
Probably VESC6+ as it has built in IMU, problem is that original 1W runs on 18S LiFePo4 which gives around 58V. You’ll need 14S with regular LiIon to reach similar speed while VESC’s max is 12S which limits max speed to around 19kmh with popular chinese wheel people use.
```

---
## \#591 Posted by: Fosterqc Posted at: 2019-11-27T05:40:57.415Z Reads: 71

```
You mean 16S lifepo4 58.4 yeah.

Secretly hoping my battery in my V1 Onewheel dies so I'm forced to upgrade it.
```

---
## \#592 Posted by: webst Posted at: 2019-11-27T05:48:08.622Z Reads: 74

```
I quickly calculated with nominal voltage. You’re right.

[quote="Fosterqc, post:591, topic:80129"]
Secretly hoping my battery in my V1 Onewheel dies so I’m forced to upgrade it.
[/quote]

Well, it won’t happen soon though with that chemistry unless you help somehow.
```

---
## \#593 Posted by: Squab Posted at: 2019-11-27T07:24:39.511Z Reads: 79

```
Firstly, if you are using phub-188 wheel, then PID constants Swarley gave are not for you.
Try P = 7-10 and D = 120-160, jerkiness should go away mostly. 
Secondly, if you'r VESC is Flipscy FSESC 4.12 then jerkiness would never go away completely, right now I'm in the process of figuring out what causes such a big difference in behavior (ie what chinesium bull they did in components to Vedder design)
```

---
## \#594 Posted by: NuRxG Posted at: 2019-11-27T08:33:45.386Z Reads: 78

```
fsesc 6.6 is even worse :expressionless:
```

---
## \#595 Posted by: Fungineers Posted at: 2019-11-27T16:09:43.078Z Reads: 78

```
My range test of the 10S Samsung 25R battery. 
https://youtu.be/_ANnb3Uvrao
```

---
## \#596 Posted by: Fungineers Posted at: 2019-11-27T16:10:17.325Z Reads: 74

```
Still riding daily and loving it. No problems yet :slight_smile:
```

---
## \#597 Posted by: clumsylyric Posted at: 2019-11-27T18:44:00.976Z Reads: 76

```
Thank you very much, just what I needed
```

---
## \#598 Posted by: clumsylyric Posted at: 2019-11-27T18:46:46.649Z Reads: 78

```
Just got my MPU+VESC working but I ran into another problem. When I connect footpads (Car seat ones) My switch Value can be detected as 1 or 0 but it doesn't work. State is always Fault when I have footpads wired. Any suggestions?
```

---
## \#599 Posted by: NuRxG Posted at: 2019-11-28T07:56:14.419Z Reads: 75

```
Need a switch value of 2 to exit fault. Gotta wire 2 switches, or one switch to two pins.
```

---
## \#600 Posted by: 702vegas Posted at: 2019-11-28T08:20:49.592Z Reads: 76

```
would it be possible to use brains from an EUC to make a one wheel?
```

---
## \#601 Posted by: webst Posted at: 2019-11-28T09:52:29.554Z Reads: 80

```
https://youtu.be/0dq-1kT_1OI
```

---
## \#602 Posted by: webst Posted at: 2019-11-29T08:11:57.115Z Reads: 77

```
General question. What is real life advantage of using 16S in such a device over 12S? Won’t using higher KV higher nominal power motor suffice?  Maybe @b264 could shed some light.
```

---
## \#603 Posted by: esk888 Posted at: 2019-11-29T14:06:00.794Z Reads: 78

```
I am working on a one wheel board but can't find a suitable wheel.
```

---
## \#604 Posted by: NuRxG Posted at: 2019-11-29T14:07:30.168Z Reads: 82

```
A higher KV motor would be fine, however as i understand it, higher voltage will run a little more efficiently and cause less heat. The real issue is that without spending a ton of money we really only have access to lower voltage controllers and low kv motors. So were stuck going slow.

I do own a ninebot z10, which is 16s with a top speed around 30mph, so even at 12s that motor would have a fairly acceptable top speed. It gets fine range for its battery, and i have no issues with it. I did burn up my first controller but burning up controllers is pretty common on higher voltage models too.

There is also the leili ebike motors that are pretty high KV as well. But all the wide "onewheel" like motors we gwt from peipei are low KV. So far i haven't seen anyone re-wind one yet.
```

---
## \#605 Posted by: ZbLaB Posted at: 2019-11-30T21:29:13.433Z Reads: 83

```
Hi, I was reading this topic, but olny now I decided to post my onewheels here.

About one year ago I made my first onewheel clone based on components from cheap chinese hoverboard. I discovered simple hack and share this online - many builders decided do try make their own boards based on this concept, so now there are about 30+ boards like mine spreaded on whole world :slight_smile:

Youtube video about that was posted by webst couple posts earlier.

Now, when NuRxG shared their own vesc solution it is good moment to do it once again - but better. 

General dimensions was taken from Pint, but my board is litte bit wider. Main frame have only 4 elements - very easy to cut from 18 mm plywood by simple CNC router. Today I've finished frame and wiring. Foot sensor is made of seat sensor from Audi - it will be hidden under grip tape soon. I'm still waiting for BMS from China to finish 12s2p battery. Vesc with IMU and Mitch firmware was tested on my prototype board, you can find that on my IG and FB - it works well, so there souldn't be any problems. 

Detais you can find on my fb page: facebook.com/zblab or on instagram: instagram.com/zblab - unfortunetly this forum tells that I'm not allowed to post links and pictures. 

Thanks in advance for you opinion. 
regards,
ZbLaB
```

---
## \#606 Posted by: NuRxG Posted at: 2019-11-30T22:15:18.863Z Reads: 84

```
Here are the links he cant post :smiley:

https://www.instagram.com/p/B5gFJr4B8aK/?igshid=tq6xrv6xbaub

https://www.facebook.com/141274539380494/posts/1335214609986475?sfns=mo

I guess because he is a new user.
```

---
## \#607 Posted by: webst Posted at: 2019-12-01T22:39:25.088Z Reads: 73

```
Impressive, would you mind sharing link to the wheel that you used?
```

---
## \#608 Posted by: Fosterqc Posted at: 2019-12-02T01:30:22.544Z Reads: 73

```
Sure looks like the Phub-188 or other from 

Peipeiscooter

@ZbLaB fantastic work with the routing. I really like the USB extension to the vesc. Looks very well thought out.
Would you share your plans or designs with us?
```

---
## \#609 Posted by: Fosterqc Posted at: 2019-12-02T01:31:43.109Z Reads: 75

```
What's your budget?

What size diameter do you want?

What voltage you gonna run?
```

---
## \#610 Posted by: webst Posted at: 2019-12-02T07:46:28.345Z Reads: 74

```
[Phub-44](https://s.click.aliexpress.com/e/43KAsAOWP) looks ideal (size wise) but underpowered and sold in a lot of 10. If we were about to buy more there should be no problem to have it customised. @ZbLaB will you be able to compare it to original ow and estimate parameters like KV knowing that 12S should be maximum?
```

---
## \#611 Posted by: Remieknaapen Posted at: 2019-12-02T09:13:29.834Z Reads: 75

```
I made some changes to my onewheel last week. I took the plunge and opened up the phub-188 to see the inert. My goal was to see how it's winded and connected inside. I will post some pictures of the inside of the hubmotor next time.

What i find out is that the motor is star winded. Re configuring this to a delta winding makes the KV 1,7x greater. The stock KV of the Phub-188 is 10. Meaning winding it to delta we would get a KV of 17. Downside is that the torque gets divided by 1,7. Since to torque of the stock Phub-188 is pretty high this shouldn't be a problem. So I changed the winding from star to delta. Result is that my top speed on 12s increased from max. 19kmh to a steady 21Kmh. I still had powered left and in theory I should be able to reach a speed of +-30Kmh with this setup. Since I didn't wear any protection I was afraid to go faster. 

I will post some details about this mod once I have tested it some more.
```

---
## \#612 Posted by: Surfer Posted at: 2019-12-02T14:03:01.826Z Reads: 75

```
Maybe is worth to wait a bit for the vesc FOCer is up to 20s and it has a IMU built in.
Beta units are assembled as we speak.
![IMG_20190906_220003|250x500](upload://gXgDvVlMfBlnSE5OGb5fbnziOo4.jpeg) ![IMG_20190906_220820|250x500](upload://rvEgKEmYEh2kkM30FIvhyQE18tY.jpeg)
```

---
## \#613 Posted by: NuRxG Posted at: 2019-12-02T19:31:30.749Z Reads: 73

```
How complex is this rewiring? Did you toss all the original copper, or did you just unwind and rewind the original wires? Did you have cut or solder anything? Was it all glued together?
```

---
## \#614 Posted by: webst Posted at: 2019-12-02T23:45:23.734Z Reads: 74

```
Thanks for the pictures, OW shaft is really beefier compared to all the Phubs. 

Is there any BMS comparable to DieBieMS for more than 12S? Also what about BT modules, will FOCer work with metr?
```

---
## \#615 Posted by: NuRxG Posted at: 2019-12-03T01:53:48.679Z Reads: 76

```
I did some self edumacating, it seems changing from star to delta is just modifying the terminating ends, no actual rewinding required.

I'm gonna open mine up and give it a looky look.
```

---
## \#616 Posted by: NuRxG Posted at: 2019-12-03T06:39:17.441Z Reads: 76

```
A buddy has that motor and he says it is super weak and underpowered.
```

---
## \#617 Posted by: webst Posted at: 2019-12-03T07:28:58.930Z Reads: 77

```
You mean Phub-44? It looks like I’d have to reconsider moving higher than 12S with this build.
```

---
## \#618 Posted by: Remieknaapen Posted at: 2019-12-03T09:11:32.041Z Reads: 79

```
It is pretty easy actually!

The side covers of the Phub-188 are held in place by the 8 screws and some silicon kit.
I gave the axle a gentle tap to 'brake' the silicon kit loose from one of the side cover plates.

Configuring it from start to delta took some tinkering but in the end it's really easy.
I didn't have to remove any of the windings, all I did was resolder the start and end of each winding of the motor. Currently all 3 ends of the windings are soldered together. The 3 starting points of the windings go to the vesc. When opening up the motor and looking from the top to the starts and ends of these windings you can see there are 6 small bundles of wires coming out of the stator. reading them counterclockwise gives E1, E2, E3, S1, S2, S3 (E=End, S=Start). All you need to do is connect S1 to E2, S2 to E3 and S3 to E1. These 3 individual connections each need to be connected to 1 of the 3 wires from the vesc. I will try to make a small schematic drawing if someone is interested in it.

Some pictures of the motor. Build wuality is pretty good, Windings look reasonable. Only thing I noticed is that the shaft of the Phub188 is made from really soft steel. Will see how it will handle after a while. 
![IMG_20191123_141021|666x500](upload://K0zoAkIGTSkmzL7Uu8AzKdoO5V.jpeg) ![IMG_20191123_141143|666x500](upload://4UoGv3m5Ls1cPPOL8tJuwmroeDz.jpeg) ![IMG_20191123_141349|666x500](upload://a71hioJySA1vWdaMJw2y8qFl2Of.jpeg)
```

---
## \#619 Posted by: Remieknaapen Posted at: 2019-12-03T09:39:17.488Z Reads: 78

```
Can you tel by looking at the original onewheel hubmotor if it's delta or star connected ?
```

---
## \#620 Posted by: webst Posted at: 2019-12-03T10:07:47.893Z Reads: 78

```
[quote="Remieknaapen, post:618, topic:80129"]
Only thing I noticed is that the shaft of the Phub188 is made from really soft steel
[/quote]

That shouldn't really matter that much I suppose, the forces are not that large. BTW: Looking at those wires OW motor looks like much lower KV and Phub188 is already around KV10. That gives high torque while going slow while 16S allows for high speed. Am I right?
```

---
## \#621 Posted by: Surfer Posted at: 2019-12-03T10:20:59.822Z Reads: 79

```
> That shouldn’t really matter that much I suppose, the forces are not that large.

I think you right, the ow motor shaft is aluminium.
@Remieknaapen i don't have a plan to open it soon, I will keep it in mind for next time
```

---
## \#622 Posted by: Remieknaapen Posted at: 2019-12-03T12:21:09.282Z Reads: 80

```
Can't really say much about the windings, they look pretty simulair to me. Beside that the kv also depends on stator size, magnets and a few more things. I do think that the kv of the onewheel motor is +-10kv, same as the phub-188. Running it on 15 or 16s and using a tire with a diameter of 290mm makes it go 30kph.
```

---
## \#623 Posted by: NuRxG Posted at: 2019-12-03T18:05:38.131Z Reads: 80

```
onewheel motor unloaded goes almost 30mph much faster than kph. tiltback is at 16mph, but i ride with friends going 22mph on onewheels all the time.
```

---
## \#624 Posted by: Remieknaapen Posted at: 2019-12-04T11:52:34.028Z Reads: 82

```
According to my calculations my modified phub-188 does about 24mph unloaded. Not really comparable with the xr. But looks like i will be able to reach pint speed. Also my board in dimensions, weigth and range is more comparable with the Pint then the Xr.
```

---
## \#625 Posted by: clumsylyric Posted at: 2019-12-06T16:35:13.239Z Reads: 79

```
I just got my onewheel fully working and had a day of testing. I turn it on the next day (No changes at all) and it has some weird behavior. When I tilt forward it takes a little while to respond and jerks all of a sudden. Same for tilting back. Seems like the PID output doesn't match my pitch output for some reason. Am I right that this is the case? Or is there another problem?

Thanks!
```

---
## \#626 Posted by: Surfer Posted at: 2019-12-06T19:16:08.166Z Reads: 79

```
Maybe your gyro drifted and needs recalibration?
```

---
## \#627 Posted by: Fosterqc Posted at: 2019-12-08T06:22:03.795Z Reads: 81

```
![Screenshot_20191207-222013_Lite|281x500](upload://c0DhYFj0MA00lKpLoTI6gLuAyP6.jpeg) 


Another XR motor with is Vega going for $490
And a v1 motor got sold for $175
```

---
## \#628 Posted by: aidnani Posted at: 2019-12-10T01:19:23.833Z Reads: 78

```
https://www.youtube.com/watch?v=tQ0S2yHSg_8

I thought I'd share my progress! I now have a working prototype. I'm using an ESP32, a VESC, and a steel frame made of 1inch square tubing. I've also got a mobile app which connects with bluetooth for tuning the PID loop. My end goal is to implement digital shaping, just like the actual OneWheel!

![screenshot_20190710-221306_onewheel-1-2|292x489](upload://aXPh6JqGW5t1bHqTSrD1kY5Vo5n.jpeg)
```

---
## \#629 Posted by: Remieknaapen Posted at: 2019-12-10T13:54:34.150Z Reads: 76

```
Looks Good! Can you tell us a bit more about what components you are using?
And it looks like you have some kind of remote or maybe a trigger in your hand to activate the board am i right?
```

---
## \#630 Posted by: aidnani Posted at: 2019-12-10T22:42:08.849Z Reads: 76

```
Thanks! So the thing in my hand is actually just an on/off switch. This current version doesn't have any weight sensor pads, so I just needed some way to enable and disable the motor. The next version should have those pads, and will eliminate that switch. 

I've got a blog post here with all the details. The one in this post is an older version with a different wheel, but my current version is almost exactly the same, just with the wider wheel.

https://akashidnani.com/2019/07/21/building-my-own-onewheel/
```

---
## \#631 Posted by: aidnani Posted at: 2019-12-10T22:43:59.416Z Reads: 75

```
I can hardly tell the difference between that and the actual OneWheel. Nice! Do you have details on how you constructed the frame?
```

---
## \#632 Posted by: Khurtana Posted at: 2019-12-14T23:28:58.555Z Reads: 73

```
What wheel is your new one?  Do you have a link?
```

---
## \#633 Posted by: Pierrotds Posted at: 2019-12-16T14:44:49.442Z Reads: 74

```
Hi guys I'm trying to configure my IMU. I think I did everything right but when I'm looking at the graph of angles it's seems that the axis are drifting away from there original position. My gyro is pretty much centered and my accelerometer to. Do somebody knows what to do ? Thanks !

 ![Annotation%202019-12-16%20154314|690x146](upload://8kOTTAp5xhCyUkWVxcsEXcYqzYc.png)
```

---
## \#634 Posted by: Remieknaapen Posted at: 2019-12-16T15:29:02.205Z Reads: 71

```
Did you correct all the axis of the MPU? I only centered the axis that is used for balancing the board. I did try to correct and center all axis at first but that also resulted in a lot of drifting.
```

---
## \#635 Posted by: Pierrotds Posted at: 2019-12-16T16:09:57.841Z Reads: 71

```
Fine thanks it's working better now ! Other little problem I think is that I can't make the motor spin properly. When I'm uploading the app data on the vesc the motors makes a spin but later nothing more. Even when the imu is flat it doesn't make the motor spin in either direction. Any ideas ? Thanks again
```

---
## \#636 Posted by: Remieknaapen Posted at: 2019-12-16T21:14:41.473Z Reads: 71

```
That's probably because there is no load on the motor. Set your cutoff duty cycle to 1 and the wheel should keep spinning untill you let go the footpad sensors or shut it of if you don't have any sensors yet. Just be carefull!
```

---
## \#637 Posted by: Pierrotds Posted at: 2019-12-18T07:26:44.334Z Reads: 70

```
Seems to work a little bit better thanks ! I think I need to have the peihub motor to do real test. So I'll wait
```

---
## \#638 Posted by: aidnani Posted at: 2019-12-18T10:44:09.857Z Reads: 73

```
Updated blog post on my version. Lots of build details for those of you who are curious! 

I'm hoping for the next version to do aluminum rails, along with 3d printed bumpers and footpads, like @Remieknaapen has done. I'll also probably be be removing the ESP32, and using the VESC balance app. 

https://medium.com/@aidnanidev/building-my-own-onewheel-4eebeaa60fc?sk=558232ac564193a4eeb3a081801cea02
```

---
## \#639 Posted by: jwhite Posted at: 2019-12-20T05:07:02.439Z Reads: 73

```
So I just started the assembly of my own onewheel, now that all my parts have finally arrived, and I'm a little confused. The vesc I'm using has 6 wires for the hall effect sensors, but the motor I'm using (phub 188) only has 5 hall effect wires? What do I do with the extra wire coming from the vesc?? Thanks!
```

---
## \#640 Posted by: Remieknaapen Posted at: 2019-12-20T08:30:49.654Z Reads: 76

```
The Vecs has a Temp. sensor input connection. The phub 188 doesn't have a temp sensor so you don't need to connect anything to the vesc temp. Sensor input.

For the other connections; Red wire from the phub 188 is 5v, Black wire is ground, and the other three wires are the hall signal wires and can be wired randomly to the vesc hall ports.
```

---
## \#641 Posted by: NuRxG Posted at: 2019-12-21T05:17:09.073Z Reads: 73

```
Hey guys I started a telegram chat room for real time talking about diy self balancing stuff.

https://t.me/joinchat/JP0KNxbguWM5KhHrT5_CYA
```

---
## \#642 Posted by: ZbLaB Posted at: 2019-12-26T11:46:02.986Z Reads: 72

```
Today I made range test on my vesc onewheel.
I have about 95 kg, there is about 6*C outside (quite cold).
I made 10,5 km and my 6000 mAh 12s2p sony vtc6 battery still performs but I had enough :). Voltage dropped from 50,4 to 44,6V so there was some juice left.
Max speed achieved was 22 km/h. 
I think that in summer it will be able to reach about 18-20 km with me.

Here is small video about my board:
https://youtu.be/J2WR75qj_28
```

---
## \#643 Posted by: ZbLaB Posted at: 2019-12-26T11:53:10.959Z Reads: 72

```
And some pictures:
https://www.instagram.com/p/B6f2Q9ABpKz/

https://www.instagram.com/p/B6WDSwbhgh7/
```

---
## \#644 Posted by: RevolutionAire Posted at: 2019-12-31T05:26:13.071Z Reads: 69

```
Hi everyone,

Amazing builds.
Could anyone post some details of how you are attaching the wheel axles to the side rails.
I’ve never seen an actual OW so I’m unable to reverse engineer it and the pictures posted don’t quite show that detail.

Thanks.
```

---
## \#645 Posted by: Fosterqc Posted at: 2019-12-31T05:36:52.936Z Reads: 67

```
It is a round dead axle with two flats. So it's kind of 0 shaped. Some peipei hub motors include metal plates if you order the right one, that can be bolted to aluminum rails.
```

---
## \#646 Posted by: annihil8ted Posted at: 2020-01-03T20:29:08.588Z Reads: 64

```
Ayyy UCI! That's my alma matter. haha is that APS?
```

---
## \#647 Posted by: annihil8ted Posted at: 2020-01-03T20:30:48.210Z Reads: 63

```
I know it's been stated before but would y'all mind also documenting some of the valuable info here on the other forum? The frequent forum outages are slightly concerning :sweat_smile:
```

---
## \#648 Posted by: miniOW Posted at: 2020-01-04T03:54:40.455Z Reads: 65

```
Getting the parts to build my onewheel using the shell of the v1 onewheel. Its a 500W motor attached to a 16s LiFePO4 battery pack.
Sourcing the phub-181 1kW since it will fit my Burris onewheel tyre (11x6-6), and the vesc 75/300 to play with.

Will first try getting the new motor to work with the V1 controller to see what happens, then the v1 motor with vesc.

All the past work on this is inspirational.
```

---
## \#649 Posted by: Fosterqc Posted at: 2020-01-04T20:58:43.415Z Reads: 66

```
Uhhhhhhh the Peipei motor with the Onewheel V1 controller? 

Wouldn't it need to be configured for the motor? Hall sensor parameters and such. 


I have a V1 Onewheel too. The moment it breaks I'm going to start tinkering with it but it's a tank. 

I think am interested upgrade would be 16S3P lifepo4 18650s. Slightly larger but can have capacity up to 4.5Ah, and it should work well with all the stock components.
```

---
## \#650 Posted by: miniOW Posted at: 2020-01-05T00:25:01.843Z Reads: 65

```
tbh, was going to assess the motor when I get it, suss out the wiring so voltages and sensors are at least connected correctly and see how it goes.
```

---
## \#651 Posted by: Surfer Posted at: 2020-01-05T19:08:27.673Z Reads: 64

```
I did mod my ow+ to 14s3p with Samsung 30q and it fits inside of the battery box, that's 9 amps and gives around 35km, maybe is interesting instead lifepo4, still using same ow original charger.
```

---
## \#653 Posted by: miniOW Posted at: 2020-01-05T22:46:28.311Z Reads: 64

```
Thats awesome. I thought there would be issues going to a 14s on the onewheel BMS but looks like its fine. Also, how did you fit 42 18650s into the same housing?
```

---
## \#654 Posted by: Fosterqc Posted at: 2020-01-05T23:15:46.886Z Reads: 65

```
I think they take the OW BMS out. 

They are switching from 16S1P lifepo4 26650 to 14S3P li-ion 18650. 

It is possible because there is some extra room under the battery that is normally for protection but most modded Onewheels have float plates over this weak point.
My v1 battery I checked when I got it used, someone has been in there before me.
![20191005_133214|666x500](upload://uy5j4V4jQGUK7z7fjeM0CpwzWgy.jpeg)
Pic I couldn't find before (WARNING FIRE PRONE BATTERY CHILDREN AVERT YOUR EYES)
![FB_IMG_15783527238459046|375x500](upload://elHz6uM0dPWZsjTHAlyLxcZrrtI.jpeg)
```

---
## \#655 Posted by: mikenyc Posted at: 2020-01-06T02:30:05.779Z Reads: 66

```
https://www.youtube.com/watch?v=ojM8FEeXLoQ&feature=youtu.be&fbclid=IwAR0-aoUGVLRgvXANLhvdt8hVXZmw2-LY_LRMi9oX6HfPaA4wa6R-kY_wj8s
```

---
## \#656 Posted by: Surfer Posted at: 2020-01-06T14:46:23.053Z Reads: 65

```
Thanks buddy, I left my post unfinished. :slight_smile:
```

---
## \#657 Posted by: Fosterqc Posted at: 2020-01-06T23:22:13.609Z Reads: 63

```
I'm supprised at how well it worked. Definitely would want to see more on how it rides.
```

---
## \#658 Posted by: miniOW Posted at: 2020-01-07T09:18:51.269Z Reads: 63

```
Might be worth finding a spare XR battery box to give you a bit more space to work with.
```

---
## \#659 Posted by: Fosterqc Posted at: 2020-01-07T09:31:40.515Z Reads: 66

```
I'm not sure if the xr battery box fits the V1. I would just make the V1 box taller as I mentioned before.

I am talking to someone who makes rails that is working on a custom XR battery box.
```

---
## \#660 Posted by: Fosterqc Posted at: 2020-01-07T23:40:39.498Z Reads: 67

```
![20200107_153731|661x499](upload://zdkZXRvitgvR5s9OlzMoIQXs5GF.jpeg) 

There is another one up for $500 that has ceramic bearings and Burris treaded.
```

---
## \#661 Posted by: veebee Posted at: 2020-01-09T00:51:31.505Z Reads: 68

```
[I recently modded my stock XR pack.](https://imgur.com/a/HsfPIs2) Took it from 15s2p of VTC6 to 15s2p of Sanyo 20700b.

I had to mill some relief in the pack, but everything is working with the standard controller/BMS. I'm getting about 19-20 miles on a charge, up from about 14-15. Only problem is the app doesn't really know my SOC anymore. A full drain/charge helped a ton but it's still about 10% off. Not a big deal.

The XR pack should fit the V1 frame, but you will have to use XR bumpers with it. Dimensionally the rails haven't changed from V1->XR from what I can tell, and I've swapped a lot of parts.
```

---
## \#662 Posted by: Fosterqc Posted at: 2020-01-10T11:48:10.368Z Reads: 67

```
[quote="veebee, post:661, topic:80129"]
The XR pack should fit the V1 frame, but you will have to use XR bumpers with it. Dimensionally the rails haven’t changed from V1->XR from what I can tell, and I’ve swapped a lot of parts.
[/quote]

Thanks for the info! 
Haven't seen this in all my research.
```

---
## \#663 Posted by: Surfer Posted at: 2020-01-10T14:53:44.654Z Reads: 63

```
Really nice mod!! I believe is not possible to fit 21700 cells right?
```

---
## \#664 Posted by: veebee Posted at: 2020-01-10T15:59:19.258Z Reads: 65

```
@Fosterqc  The OW modder community isn’t very mature yet. Lotta people think installing a new footpad is a mod. I can do a side by side dimension check on the rails to be sure if you’d like.

@Surfer I don’t think so. You’d have to thin out the bottom of the pan even more, which I wouldn’t be super comfortable with even with the float plates there. I think 15s3p of VTC6 would fit, though which is what I plan on trying next.
```

---
## \#665 Posted by: jwhite Posted at: 2020-01-10T18:18:41.413Z Reads: 62

```
Hi all, I've just finished building my onewheel, and now I'm working on programming it... however, no matter what code I use I cannot get the arduino to spin the wheel. I'm wondering if there is a problem with how my arduino and vesc are connected? Any thoughts?
```

---
## \#666 Posted by: Surfer Posted at: 2020-01-10T19:14:56.296Z Reads: 65

```
I did fit 14s3p in a plus, if I was able to fit 15s3p in a xr I will go and buy a XR strait away.
If you find the time to confirm it, that would be awesome, but I'm pretty sure I will have to wait 😁
Thanks for you quality post and reply 🤙🤙
```

---
## \#667 Posted by: miniOW Posted at: 2020-01-10T23:09:03.840Z Reads: 63

```
you reckon a 14s3p will fit the XR housing with little to no milling?
```

---
## \#668 Posted by: veebee Posted at: 2020-01-11T00:31:47.383Z Reads: 66

```
@miniOW I've laid it out, and 14s3p fits perfectly with no modifications, although that's with no fishpaper/tape/shrink-tube/foam etc. Problem is the XR won't work without the BMS and the BMS is a 15s BMS, so you need those extra cells if you want it to run. If you're just using the housing for a plus then you're good to go.
```

---
## \#669 Posted by: miniOW Posted at: 2020-01-11T01:03:04.602Z Reads: 66

```
yeah, plan to use it for the custom build with vesc 75, v1 shell and ranger/ego kit. Ego batteries are 14s so will work well together.
```

---
## \#670 Posted by: aidnani Posted at: 2020-01-12T05:59:52.882Z Reads: 66

```
Zot zot! It's the ARC parking structure :)
```

---
## \#671 Posted by: milan89 Posted at: 2020-01-14T19:40:52.724Z Reads: 61

```
Hello, can you help me please? Im building my first DIY OneWheel. Its my first project with VESC (FSESC 4.12) regulator. Im using HUB wheel similar to phub-188 but VESC Tool keep recognizing it like sensorless. How should I config it in VESC Tool? My VESC also does not save engine settings from wizard.
```

---
## \#672 Posted by: SwarleyAUS Posted at: 2020-01-14T21:21:20.342Z Reads: 63

```
How many small wires come from the motor?
How have you got them connected to the VESC?

You can run the FOC Wizard or Other Motor Wizard (and choose BLDC), depending on whether you want to run in FOC or BLDC mode. FOC is not advised for high kv motors.
```

---
## \#673 Posted by: milan89 Posted at: 2020-01-14T22:13:18.547Z Reads: 65

```
There are five small wires. Red (5V), Black(GND), Yellow(Ha), Blue(Hc) and Green(Hb). 
But if I plug them all in as described, it doesn't work. On multimeter there is nothing change too. Is it possible that the engine has been damaged? Or I could burn the sensors?
```

---
## \#674 Posted by: SwarleyAUS Posted at: 2020-01-14T22:46:34.564Z Reads: 65

```
So you've got them plugged into the VESC as per this?

https://cdn.shopify.com/s/files/1/0011/4039/1996/files/06_be544658-0682-45ea-8461-9ecee8e482f2_2048x2048.jpg?v=1541572579

Doubtful you could burn the sensors if you plugged them into the #1 connector. Does the motor work in sensorless mode?
```

---
## \#675 Posted by: milan89 Posted at: 2020-01-14T22:59:18.017Z Reads: 62

```
Yes, I connected them exactly like this. The motor spin in sensorless mode. I can perform motor wizard, 
but the parameters are not saved when I disconnect the computer. In "balance" screen I can see "State: Running", but motor is stopped.
```

---
## \#676 Posted by: SwarleyAUS Posted at: 2020-01-14T23:09:25.409Z Reads: 62

```
Are you getting a "MC configuration Update" message in the bottom right hand corner of the VescTool when you complete setup i nthe wizard?

Follow these instructions if you haven't already: https://vesc-project.com/node/938

Sounds like a dud VESC.
```

---
## \#677 Posted by: Fosterqc Posted at: 2020-01-14T23:32:05.583Z Reads: 61

```
came here to say people could not get the fsesc 4.12 to work in this application

[quote="NuRxG, post:253, topic:80129"]
Switching from flipsky 4.11 to Focbox, when i lean hard it actually moves instead of just making whining noise and nose diving.
[/quote]

.
```

---
## \#678 Posted by: milan89 Posted at: 2020-01-14T23:45:15.901Z Reads: 57

```
Thank you for your answers. The solution of not running motor when it in state "Running" was that I didn't set PID in Balance screen. Tomorrow I will try set it in sensorless mode and maybe disassembly that motor to look on Hall sensors.

Thank you again ;-)
```

---
## \#679 Posted by: SwarleyAUS Posted at: 2020-01-14T23:45:47.816Z Reads: 60

```
I certainly experience these issues, but my 4.12 works more often than not and I cannot justify spending AU$400 on an ESC
```

---
## \#680 Posted by: Fosterqc Posted at: 2020-01-14T23:47:44.643Z Reads: 60

```
Are you interested in the 84v cheap FOCer @shaman is working on?
```

---
## \#681 Posted by: SwarleyAUS Posted at: 2020-01-15T01:20:26.428Z Reads: 59

```
Whats better about it?
```

---
## \#682 Posted by: Marshallin Posted at: 2020-01-15T11:31:11.943Z Reads: 62

```
Hello, can I use onewheel+ motor with VESC ? I cannot find motor I would like from china.
```

---
## \#683 Posted by: Fosterqc Posted at: 2020-01-15T15:27:09.680Z Reads: 60

```
Haha guess who's Onewheel finally broke? Yours maybe?

Well mine did. 
I'm planning on selling the controller and battery if it's good (-fried BMS)

Then, yes using a VESC to control it. 
I've actually been trying to convince people in this thread to buy used Onewheel motors off the Facebook group, instead of from Pee pee who is overall not a good store I think. 

I'm planning on using the 84V Cheap FOCer (thread on the superior esk8 community forum) 

If be interested to hear what VESC you wanted to use?
```

---
## \#684 Posted by: MysticalDork Posted at: 2020-01-15T23:08:18.058Z Reads: 57

```
It can go up to 84V, as opposed to 50V which is what most other vescs are limited to. Since the Peihubs have such a low KV, higher voltage will allow higher top speeds.
```

---
## \#685 Posted by: SwarleyAUS Posted at: 2020-01-15T23:46:46.675Z Reads: 57

```
Ah ok, I'm running 24V at the moment into a 120kv 6384 motor, rather than a hub motor. Is it based off the Focbox? If so, as NuRxG recommends Focboxes then maybe. Is the Focbox based off the VESC 6 like the FOCer V2 is?
```

---
## \#686 Posted by: Fosterqc Posted at: 2020-01-16T01:32:39.581Z Reads: 60

```
FOCBOX is 4.12 based but good with high currents. 

The cheap FOCer 2 84V is based on VESC 6 and will also have a built in gyro imu unlike 90% of other vesc available.

And given the name with some work yourself the cost per unit should be far less than $200 USD
```

---
## \#687 Posted by: MysticalDork Posted at: 2020-01-16T01:37:55.222Z Reads: 61

```
The FOCer lineup are all engineered from scratch based on the vesc6.x platform, whereas the focbox is based on the vesc4.x platform. Since you're using a regular outrunner you have less need for a high system voltage. There are quite a few 6.x based ESCs that may be more suited to your specific build.
```

---
## \#688 Posted by: Eamon Posted at: 2020-01-20T17:51:06.802Z Reads: 57

```
hey, i'm building a one wheel, could we have the 3D printing files? Your board looks amazing btw. thanks!
```

---
## \#689 Posted by: Remieknaapen Posted at: 2020-01-21T13:57:38.953Z Reads: 62

```
Not for know, the parts still need some redesigning. If I'm going to share them I think I also need some kind of manual and parts list. Because it takes more then just the 3d files to build it. Don't have time at the moment to do all of that.
```

---
## \#690 Posted by: milan89 Posted at: 2020-01-21T18:38:33.099Z Reads: 64

```
Hey guys, I would like to thank you for help about week ago. My prototype is working now. It was due to defect hall sensors in motor. So I changed that and now its in run! There is a picture of my early prototype
![MK891066|690x459](upload://1ATnBUTMFgDjIf5ITH5VQgW7UYc.jpeg) 

But Im working on better looking chassis:
![MK891074|690x459](upload://bZMU0vuJGKS6RuEKiRpIzbnvwdF.jpeg)
```

---
## \#691 Posted by: Groovr Posted at: 2020-01-23T20:22:12.548Z Reads: 59

```
That new frame looks awesome :slight_smile:
```

---
## \#692 Posted by: edumerc Posted at: 2020-01-24T02:02:23.834Z Reads: 57

```

Very cool prototype, I may be weird but I really like the thin steel rails, do you have any video on how it rides? The new frame looks awesome, like factory made, is it cnc machined?
```

---
## \#693 Posted by: UnspecifiedId Posted at: 2020-01-24T03:52:02.035Z Reads: 57

```
Fantastic work and love the YouTube video. Are you able to share your CAD design file and 3d print/STLs with the community ?

Excellent, Excellent work.
```

---
## \#694 Posted by: MysticalDork Posted at: 2020-01-24T05:42:53.117Z Reads: 55

```
[quote="edumerc, post:692, topic:80129"]
is it cnc machined?
[/quote]
 If I had to guess, I'd say it's manually machined (or could be) for all the holes, and then all the frame members are welded together nicely.
```

---
## \#695 Posted by: Remieknaapen Posted at: 2020-01-24T13:58:07.631Z Reads: 53

```
Thanks for the compliment! 

Like I mentioned before. The parts still need some redesigning. If I’m going to share them I think I also need to write some kind of build manual and write down a parts list. Because it takes more then just the 3d files to build it.

I'm playing with the idea of doing that. Maybe I'll start writing stuff down and see where it goes.
```

---
## \#696 Posted by: Nick2204 Posted at: 2020-01-25T11:17:32.772Z Reads: 53

```
Did you ever get any further with the superfoc 6.8 ? I'm keen to give it a try as opposed to starting off with an older 4.12 variant, but onewheel balance functionality is one of my key interests.
If it needs some code tweaks or pin tracing to see where they've put the sda/scl pins I can give it a go.
```

---
## \#697 Posted by: jokostyle Posted at: 2020-01-25T14:43:28.777Z Reads: 52

```
Hello, can someone help me? I cannot run  a small sensorless motor to test if my 6050 work well.

I have not the gyro orientation tab in the vesc tool 2 free

I cannot send image or link, because I m new maybe.:blush:
```

---
## \#698 Posted by: maxdg99 Posted at: 2020-01-26T03:50:32.658Z Reads: 55

```
Hello all!  I recently became interested in building my own OneWheel, so I have read a good chunk of this thread.  This had lead me to have a few questions...

First off, it appears that one of the only sources of hub motors that would work for this build is from Pei Scooters.  As I have read in this forum, however, it seems that Pei Scooters is unreliable and the motor has a relatively low speed.  What do you all think about using a belt driven set up?  Do you think that a belt driven setup would be capable of self balancing?

Secondly, if I were to use a belt driven system, could I use a regular arduino motor controller as opposed to a VESC?  It would save a lot of cost, and I may not need FOC for this applications.

I think you all in advance for your help!  This forum has been very useful in my research!
```

---
## \#699 Posted by: MysticalDork Posted at: 2020-01-26T04:10:38.792Z Reads: 55

```
Re: belt drive, yes that will work. There are several people in this thread and elsewhere that have used chain to good success, and belts work the same.

Re: not using a vesc, it totally depends on how much effort you are willing to put into it, and how skilled of a programmer you are. It can absolutely be done, but assuming you value your time at $5/hour, you'll be able to afford several vescs by the time you're done.
```

---
## \#700 Posted by: maxdg99 Posted at: 2020-01-26T04:22:17.488Z Reads: 54

```
Thank you very much!  This is very helpful!  I may try a normal motor controller just for the heck of it because I am going to school for computer science, but I may just end up with a vesc.  Thanks again!
```

---
## \#701 Posted by: Seaka Posted at: 2020-01-26T23:55:21.864Z Reads: 57

```
Hello all,
Long time lurker, first time poster.
I had read this thread before Mitch wrote his self balance app for the VESC.
Just a question to anyone in the know, Would a Vesc mini 4.20 work for this project or is it that different in hardware to the 4.12 that it would be a problem?
Thanks all.
Seaka.
```

---
## \#702 Posted by: SwarleyAUS Posted at: 2020-01-27T10:54:46.816Z Reads: 56

```
Doing that now. Was previously running a chain drive but for the same gear ratio I can use smaller pulleys/sprockets and thus get better ground clearance. I find my 6384 brushless motor has plenty of torque @ approx 5:1 gearing:

https://youtu.be/JZM3uOjBaKc

It's not as clean a solution as a hub motor, in both senses of the word, but it works. I just hope there will be no more inefficiencies in the system than there was in my chain drive. Time will tell.

WIP ![IMG_20200116_213204|374x500](upload://z3ghCHOSnENBvSHdAXoL7RqcFBQ.jpeg)
```

---
## \#703 Posted by: SwarleyAUS Posted at: 2020-01-28T01:34:59.162Z Reads: 55

```
Have you downloaded the tool from here? https://vesc-project.com/node/17

You may need to update the firmware on your vesc, through vesctool, too.
```

---
## \#704 Posted by: jokostyle Posted at: 2020-01-28T18:07:14.491Z Reads: 51

```
Hi, yes I have yet updated my firmware through vesctool 2 free version.

I have 3.66 installed. ![image|690x388](upload://npwVjrxMKBoGtfdSX7XIuxzimE5.png) 

I dont understand how to set up the balance app, I will recheck tonight the video tutorial of NuRxG.

but I have not the gyro orintation tab, so I dont know if it is the roll or pitch axis which should drive the throttle of the wheel.
```

---
## \#705 Posted by: SwarleyAUS Posted at: 2020-01-28T20:10:37.376Z Reads: 47

```
XYZ, Accel and Gyro tabs are under IMU app
```

---
## \#706 Posted by: jokostyle Posted at: 2020-01-28T23:29:38.236Z Reads: 50

```
Yes I know and i have set some offsets.

I have try different things, and  set a deadzone of about 1 degree seems to work but the throttle curve seems to be too sensitive the motor go fast with a little angle.

when I put a strong angle to the imu 6050 , the state become dead and the motor doesn't rotate, I need to deplug the battery and replug the battery to  reboot the esc. Do you know which setting I should  modify to avoid this behavior ?
![image|690x388](upload://b7Mxlv1cCeIJS0gIPVxbJSFga4q.png)
```

---
## \#707 Posted by: SwarleyAUS Posted at: 2020-01-29T01:13:12.619Z Reads: 51

```
If you are testing the motor on the bench, with no load, then what you are seeing is expected behaviour. Without a load the motor will spool up quickly and go into 'dead' state because it cannot compensate for the tilt angle with the closed loop system being broken. This is an unfortunate limitation of the balance app. Would be good to have a test mode where the dead mode can be disabled.

Safe to say it is the pitch angle that drives the motor current.
```

---
## \#708 Posted by: maxdg99 Posted at: 2020-01-29T15:20:18.301Z Reads: 48

```
Has anyone had experience using a motor controller other than a VESC (diy or bought)?  Secondly, can anyone recommend a VESC that is 'good' at self-balancing (as I have read that some VESCs do not perform well) that is around $100?  Thanks in advance!
```

---
## \#709 Posted by: jokostyle Posted at: 2020-01-29T16:46:51.855Z Reads: 45

```
Hi !

Thanks SwarleyAUS for your explanations.
 I am charging the 18650 to make the real battery pack, I will test will the real motor and a load. 
I will try to make a 13S2P pack, but I fear that my fesc 4.12 blow with the voltage spikes despite if it is labeled 13S on it. 
I have see on the forum that the team triforce uk have made a strong esc but it is too expensive for me. I am looking on the uncle FOCer but I don't know how to make an esc and if it is compatible with the vesc software.
```

---
## \#710 Posted by: GroteGeert Posted at: 2020-01-29T19:18:45.732Z Reads: 44

```
Hi, 

Man what a mega story. I am new here and i am reading reading and.......... reading. My name is Geert and i am from the Netherlands. I did do a lot of stuff with ebikes, 10kw downhill bikes, racedrones and skateboards. I never had aspected that people brake the codes of the onewheel. Respect!!!!!!
Reading this forum has motivated me to build one.
```

---
## \#711 Posted by: GroteGeert Posted at: 2020-01-29T19:23:24.705Z Reads: 45

```
@Remieknaapen nice to see someone from or little country. Maybe you can help me to start this project.
```

---
## \#712 Posted by: MysticalDork Posted at: 2020-01-29T20:41:12.664Z Reads: 45

```
You haven't asked any questions yet, just made statements. Once you ask a specific question, then we will be able to answer it.

I will say that personally I wouldn't run 13s on any speed controller with a maximum safe input voltage of 60v, that's just too close to the limit. 12s is, in my opinion, the highest you should go.
```

---
## \#713 Posted by: jokostyle Posted at: 2020-01-29T21:35:43.475Z Reads: 49

```
on the label of the esc, it is write that it can manage 3 to 13S lipo, but when I see the other esc that are done to 12S I think that flipsky are maybe lying on the specs.

the capacitor on the esc are rated 63 volts and 13x4.2 will give 54.6 volts .

It give 8.4 volts headroom for the voltage spikes. I have yet buy a 13s daly bms, can I use it on a 12 pack ?

I want to have a good max speed, that's why I am interested to build 13 S pack.

A better esc with max voltage will be great, but the prices are insane, I am interested by  the FOCer 84V, but for now it is still in development and not supported by vesc tool for the moment.

I will make a 12S battery pack for the moment, it will avoid the esc to burn , you are right; thanks for the advice :+1:
```

---
## \#715 Posted by: MysticalDork Posted at: 2020-01-31T01:29:32.711Z Reads: 45

```
[quote="jokostyle, post:713, topic:80129"]
I have yet buy a 13s daly bms, can I use it on a 12 pack ?
[/quote]
No. Unless your BMS specifically states being able to handle multiple cell configurations, a 13s BMS is only suitable for a 13s battery, and you will need a 12s BMS for your 12s battery.
```

---
## \#716 Posted by: Giga Posted at: 2020-02-01T20:22:09.508Z Reads: 46

```
Thats not true for most bms. 

All BMS with processor on the PCB do use either a TI chip or LTC chip for cell monitoring. And for this chip you just have to look into the datasheet and can see which "cells" have to be shorted to work at other configurations. 

Even vendors show it: 

![image|390x500](upload://5XZcqS4xgOLTDm1FT49NPkUuumw.jpeg) 

Just keep attention when buying...
```

---
## \#717 Posted by: jokostyle Posted at: 2020-02-04T18:30:22.929Z Reads: 42

```
Hi, 

I have try to connect the bms, and it is not possible, the bms is in protection mode, the voltage at the output is 42.2 volts while the total voltage of the battery is 50.3 volts. I have made a test with one more cell  and I can hear a "clic" inside the bms and the output voltage is the same between the bms and the pack. I have yet ordered a 12s bms 60A.
```

---
## \#718 Posted by: NuRxG Posted at: 2020-02-05T23:00:23.892Z Reads: 39

```
If you set cutoff duty cycle to 1 it can freespin forever :slight_smile:
```

---
## \#719 Posted by: SwarleyAUS Posted at: 2020-02-05T23:21:01.618Z Reads: 39

```
As in it will not enter dead mode? Ah-ha! Cool, good to know!
```

---
## \#720 Posted by: Bobbyboulders Posted at: 2020-02-09T00:12:22.873Z Reads: 35

```
I have been following this thread for a while and I have had a couple of different unsuccessful iterations. I finally broke down and got a larger vesc, the trampa 75/300. That and some 80/20 aluminum extrusion, and a 16s3p pack. I'm just getting finished or trying to finish tuning the thing. The PID settings are a real drag. I've at least got it to where it's rideable. Thanks to everyone that has posted helpful information.
```

---
## \#721 Posted by: SwarleyAUS Posted at: 2020-02-09T00:25:17.108Z Reads: 35

```
I think the general rule is get the P value to a point where you have good acceleration but no oscillation and then increase D gain to smooth. Should speed tuning up a bit...
```

---
## \#722 Posted by: Remieknaapen Posted at: 2020-02-09T20:45:26.065Z Reads: 37

```
Show us some pictures of your build :slight_smile: What hubmotor are you using?
```

---
## \#723 Posted by: Seaka Posted at: 2020-02-10T02:48:19.200Z Reads: 36

```
I have ordered my P-hub188, its on the way, Ive worked out what im doing for the frame and deck, Im in the middle of building my battery (12s2p), ordered footpads but Im on the fence with my VESC.
It would be nice to just order a 75/300 but thats not in the cards for this build at least for the moment, Im looking at slightly more affordable hardware, what are peoples opinions on 4.12 hardware? I know  @NuRxG doesnt like the FS versions but others have had success using them, what else out there is good quality and affordable? 
I was Looking at the Maytech SuperFOC 6.8 (based on 6.0) or the Maker-X go-Foc SV6 or the Mini Foc Plus (Both based on 6.6), Has anyone had any experience with these brands?
They seem Like good value for dollar solutions but im new to VESCs so any advise or wisdom would be much appreciated.
Thanks.
Seaka
```

---
## \#724 Posted by: SwarleyAUS Posted at: 2020-02-10T03:31:57.305Z Reads: 37

```
I've had success with my Flipsky 4.12 unit. More success than not anyway. Had a decent crash but can't with any certainty put it down a fault of the VESC. Rode a real onewheel the other day and was surprised (read underwhelmed) by how similar in feel my board is/was to the real deal.
```

---
## \#725 Posted by: Ariehh Posted at: 2020-02-10T07:38:07.294Z Reads: 35

```
Hey I love reading this thread and the improvements everyone makes, but unfortunately this forum will probably go offline forever since Enertion's future doesn't look that bright. Would it be possible to carry the info and conversation over to the "other" forum?

Forum (dot) esk8 (dot) news
```

---
## \#726 Posted by: Fosterqc Posted at: 2020-02-10T08:30:09.187Z Reads: 35

```
I've  been lazily hoping someone was worried about this for me.
```

---
## \#727 Posted by: Ariehh Posted at: 2020-02-10T09:05:25.923Z Reads: 35

```
I made a thread on the "new" forum to continue this thread.
Please post all further info there to preserve all knowledge and info

[Here is a bit.ly link since this forum removes the forum (dot) esk8 (dot) news links](http://bit.ly/OnewheelBuildGuide)
```

---
## \#728 Posted by: Bionic24 Posted at: 2020-02-10T09:46:03.604Z Reads: 38

```
Hi Arjan,

I already made a post of my Onewheel on the other forum. But until now most knowledge on DIY Onewheels seems to be on this forum :).

Here are some pictures of my build. It is a Hoverboard conversion.

![a65d2c9fcee4e0ba994685161cdbf001088f7755_2_1035x582|690x388](upload://5BIUUF93R5tnYVAJxsP3xhJniKX.jpeg) ![axle-block|375x500](upload://tNHXUNpDO678AZmfUBOOf2WeUeW.jpeg) ![innertube|309x500](upload://lVU57Oio8nASbbce22ximo6YvwN.jpeg) ![motor%20allignment|690x388](upload://trCkNuwkVddj6dFHpV0X1803QAE.jpeg)
```

---
## \#729 Posted by: Ariehh Posted at: 2020-02-10T10:05:57.216Z Reads: 36

```
[quote="Bionic24, post:728, topic:80129"]
But until now most knowledge on DIY Onewheels seems to be on this forum :)
[/quote]


I know, but there is a very big chance that this forum will shut down soon (forever). That's why I'm suggesting to maybe share the info on both forums. I suggest you link your post to your build in the thread I made, as a first.
```

---
## \#730 Posted by: Giga Posted at: 2020-02-10T11:46:29.774Z Reads: 38

```
Well, just add it here: 

https://forum.esk8.news/t/project-noahs-ark/10219

or if it gets cut out:

https://[newforum]/t/project-noahs-ark/10219

https://[swen.8kse.murof]/t/project-noahs-ark/10219

some parts are backwards :slight_smile:
```

---
## \#731 Posted by: Bobbyboulders Posted at: 2020-02-10T14:20:52.734Z Reads: 38

```
![1581344342095499055037193981322|375x500](upload://gLfKPMKUdnpE5Uf0UHoCeahtR0p.jpeg)
```

---
## \#732 Posted by: Bobbyboulders Posted at: 2020-02-10T14:22:36.888Z Reads: 36

```
@Remieknaapen there you go.
```

---
## \#733 Posted by: NuRxG Posted at: 2020-02-10T19:30:16.967Z Reads: 34

```
That thing is MEGA!!!!!!
```

---
## \#734 Posted by: Bobbyboulders Posted at: 2020-02-11T02:55:02.646Z Reads: 33

```
@NuRxG yeah I wanted to ask you about the tires you have tried on your 8" hubs. Which one do you like the best? I want something a bit shorter and narrower than that 225/55/8
```

---
## \#735 Posted by: NuRxG Posted at: 2020-02-11T21:29:44.938Z Reads: 29

```
I don't have any 8" hubs, those are all the monsterwheel. the guy who built that isn't on here i don't think, but he is in the telegram chat i posted earlier.
```

---
## \#736 Posted by: vitormhenrique Posted at: 2020-02-12T20:45:33.341Z Reads: 23

```
do you guys know where can I find information on the onewheel motor wiring?
I maybe get their motor on my diy, china is pretyyyy slow sending stuff bc of the virus, so i might try to source locally, and use with my vesc!
```

---
## \#737 Posted by: Fosterqc Posted at: 2020-02-13T04:47:57.980Z Reads: 23

```
It seems like there are only a couple people who have looked into it enough to know the KV of all the OW motors. 


I don't know if you have to unwind a motor to tell how many turns/pairs were used but maybe you could tell without destroying it. 

![c0ce94830144940c536348df99affe24e238995a_2_500x1000|250x500](upload://nlGRwb2p6Bcuy82mr0cYxLEsvCS.jpeg)

(Pic to help illustrate my point)
```

---
## \#738 Posted by: MysticalDork Posted at: 2020-02-15T02:19:35.102Z Reads: 15

```
Those photos tell us nothing about the KV. 

Your best bet is to hook it up to a vesc and check the KV from the vesc software.
```

---
## \#739 Posted by: Fosterqc Posted at: 2020-02-15T10:48:49.424Z Reads: 13

```
[quote="MysticalDork, post:738, topic:80129"]
hook it up to a vesc and check the KV from the vesc software
[/quote]

wasn't aware that was a thing, Cool!

[quote="MysticalDork, post:738, topic:80129"]
Those photos tell us nothing about the KV
[/quote]

[quote="Fosterqc, post:737, topic:80129"]
maybe you could tell without destroying it.
[/quote]

[quote="Fosterqc, post:737, topic:80129"]
I don’t know
[/quote]
```

---
## \#740 Posted by: MysticalDork Posted at: 2020-02-15T10:50:58.422Z Reads: 13

```
Yeah, it's a thing. It's not 100% accurate, but usually within ~+/-10%. The latest version of vesc-tool with the implementation of HFI is far more accurate than the earlier versions which used a different method.
```

---
## \#741 Posted by: Giga Posted at: 2020-02-15T14:45:07.005Z Reads: 8

```
Lol, KV always has been super accurate. 
Just let the motor spin at max RPM, Note down the Voltage and the actual RPM and divide each other. Then divide the result by 0.95 (because of the maximum of 95% duty of the VESC). 
Tested with optical RPM-Meter and Encoder, error is below 1%
```

---
