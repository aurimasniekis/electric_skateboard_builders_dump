# Chrysos 6x6 &#124; Custom Deck/Mounts &#124; Caliber Trucks Cal II 50° &#124; SK3 6374 192kv &#124; 12s ( 2 x 6s ZIPPY 8000mAh ) &#124; VESC

### Replies: 20 Views: 2670

## \#1 Posted by: Dutch Posted at: 2016-06-17T17:26:07.259Z Reads: 188

```
**_My parts:_**
**[Motor:](http://www.hobbyking.com/hobbyking/store/__42024__Turnigy_Aerodrive_SK3_6374_192kv_Brushless_Outrunner_Motor_EU_Warehouse_.html)** SK3 6374 192kv
**[ESC:](product/vesc-the-best-electric-skateboard-esc/)** VESC from diyelectricskateboard
**[Battery:](http://www.hobbyking.com/hobbyking/store/__16228__ZIPPY_Flightmax_8000mAh_6S1P_30C.html)** 2x ZIPPY Flightmax 8000mAh 6S1P 30C
**Motor mount:** Custom aluminium mount
**Gearing:** 16/36T 15mm
**[Wheels:](https://www.amazon.com/gp/product/B01AZ2US8G/ref=ox_sc_act_title_1?ie=UTF8&psc=1&smid=A2DQMI7AS28KLN)** white 97mm Flywheels with custom gold rims. 
Does someone know if you can buy wheels in a set of 2 instead of 4 ?
**[Trucks](https://www.amazon.com/Caliber-Trucks-Cal-50%C2%B0-Longboard/dp/B014JWQ8M8/ref=sr_1_1?ie=UTF8&qid=1466442157&sr=8-1&keywords=Caliber+2+white+gold):** Caliber Trucks Cal II 50° White/Gold
**Receiver:** Arduino Nano with bluetooth.
**[Remote:](http://www.aliexpress.com/item/2016-VR-Box-VR-Case-Bluetooth-Remote-Controller-Wireless-Gamepad-Mini-Mouse-Joystick-for-iOS-Android/1000002023104.html?spm=2114.30010308.3.2.pVvAuz&ws_ab_test=searchweb201556_0,searchweb201602_4_10017_10040,searchweb201603_10&btsid=a64bb8be-247d-4389-bef3-95b3eebe4a0d)** Modified bluetooth controller
**Deck:** Custom Deck'with paintjob ( White board with gold racing stripes )
**Housing:** Custom housing made with a air vacuum former.



**For the motor mount and wheels:** (*A tip for the people who are interested in cheaper mounts.*)

I got a lot of aluminium at home, but i want a sturdy mount, that's why i am going with 8mm thickness atleast.
My X-Carve will not be-able to cut this i think or very slow.
I will also get custom mounts like [these](https://s-media-cache-ak0.pinimg.com/736x/35/31/9f/35319f180ca8c6c0fa3c9350128980cc.jpg) i absolutely loved the 6x6 design and will put these on the back with front-wheel drive.
And what i mean by making custom rims for the flywheels is [this](http://skateandannoy.com/wp-content/uploads/2008/05/spinner4.jpg). These will be made on the lathe and later on with the CNC.
I went to some companies to ask how much this would could me to do. They were all between $400-$700. I understand they have to config all the machines and stuff which makes it this expensive. But i though this can be done cheaper!

How i solved this is, i went to my local schools and one of them has tech classes and they have all kind of crazy machines. What i did is i went in and asked nicely how much it would cost if they could CNC the mounts for me if delivered the material and drawings myself.

What do you think ? FREE.
He told me he would make it a lesson for the kids there so they could understand the machines more and so he had some more materials for teaching. I was so happy when i heared this. But ofcourse i'm not going to be a jerk and let him actually do it free. Will definitely buy them a gift of some sort.
```

---
## \#2 Posted by: flatsp0t Posted at: 2016-06-17T17:35:15.905Z Reads: 163

```
[quote="Dutch, post:1, topic:4817"]
Thinking of going with 20/20.
[/quote]
:hushed:
This is a 1:1 Ratio.
If the rest of your setup could handle it(which it cant obviously), this led top a top speed of 70 kph even on 6s!!

Normal for this type of setup is 16/36.

To the VESC/Other ESC: there were enough threads on this, use the search function on it.
```

---
## \#3 Posted by: Dutch Posted at: 2016-06-17T18:00:29.862Z Reads: 156

```
Why can't the setup not handle a 1:1 ratio ? I'm new to this so i have no clue why it wouldn't

For the VESC/ESC i did some research and got to the conclusion a VESC is the best solution.Thank you for that.
```

---
## \#4 Posted by: flatsp0t Posted at: 2016-06-17T18:12:00.819Z Reads: 146

```
Because it has not enough torgue to get a human moving. this will cause extreme heat (high amp draw) and will burn out your motor.
```

---
## \#5 Posted by: sismeiro Posted at: 2016-06-17T18:31:00.530Z Reads: 148

```
Hi, to help you with the gear ratio calculations and how the components will work together use the following calculator: http://toddy616.blogspot.pt/2013/07/electric-skateboard-calculator.html

Just put the numbers and verify the output. One thing that you should take into account is the desired top speed you want and change the other values according like the gear ratio of the motor and wheel pulleys.
```

---
## \#6 Posted by: Dutch Posted at: 2016-06-17T18:41:50.383Z Reads: 147

```
So i got this for now.
I notcied the more kV on the motor the faster it goes, so wouldn't it be better to use one like 400kV for example ?
Same goes for the battery. Would 6s or 12s be better. I'm going with a single motor now, but i'm kinda OCD and would like to upgrade to add a second motor later on.
The goal for the top speed for racing would be around 40mph weighted if possible.

http://i.imgur.com/Xdqrp2d.png
```

---
## \#7 Posted by: Mikenopolis Posted at: 2016-06-17T20:42:55.433Z Reads: 131

```
@dutch "I'm part Asian so i'm a small guy actually haha" I'm not sure what this means, I'll full Asian standing 6'0" 200lbs
```

---
## \#8 Posted by: Dutch Posted at: 2016-06-17T21:33:56.185Z Reads: 121

```
@Mikenopolis nothing really, was just a small joke because most asian people are small ( not all iknow )
```

---
## \#9 Posted by: Luke Posted at: 2016-06-17T21:34:37.895Z Reads: 119

```
going 10 or 12 s will help you with top speed. someone will know what is the highest kv motor you can run on a 12 s I think its around 230-240. also larger wheels increase top speed and decrease torque, so consider going for a larger wheel (90, 97mm) instead of a 20/20 gear ratio
```

---
## \#10 Posted by: Dutch Posted at: 2016-06-17T21:36:02.451Z Reads: 120

```
Interesting, had no idea. Thank you!
```

---
## \#11 Posted by: 91Seconds Posted at: 2016-06-18T10:37:43.211Z Reads: 110

```
I saw this picture floating around recently 
<img src="/uploads/db1493/original/2X/1/1b1b8a2e0a290f8d4ef1a8c535b60551153d6085.png" width="396" height="268">

Not sure how much you know about electric motors but the way i understand it is that as the motor spins faster it produces "back mf" which is voltage opposing the power supply voltage making it spin.  at top speed the motor produces back mf equal to the voltage going through it and so cannot go any faster because the total voltage inside the motor is zero.  the amount of back mf it makes at different rpm is characterized by the kv rating where kv refers to _rpm/volt_

on the filp side of this is that the lower the kv, the more torque you get but lower top speed.

A higher voltage of battery will translate 1:1 with higher electrical to speed which is why people are running torqueier motors (lower kv) at higher voltages to get the same speed.  this also has the advantage of getting the same power with lower amps.  _Power=Volts*Amps_

Amps kill boards, amps are hot, your motor doesnt like them, your ESC doesnt like them, and your batteries dont like them. 

With a high kv you'll get lots of rpm per volt but low torque and more or your journey will occur in the high amp range.  For example if you have aboard with an electrical top speed of 100km/h but you are travelling at 25 km/h you will be running on 25% effeciency with very hot motors.
The same board with an electrical top speed of 50km/h will run at double the efficiency and 2/3 the heat of the faster board.

I think it was @onloop who said something like "a dc motor is a hurgy little thing and when it has a load on it it will draw more amps until the load is balanced with the motor (which occurs when the motor reaches it's top electrical speed) and if that load never goes away (for example if you never get to 100km/h) the motor will continue to draw amps forever.   http://www.electric-skateboard.builders/t/beginners-guide-to-building-your-own-electric-skateboard-drivetrain/53   I think a common rule of thumb round here is to aim for 45km/h

Even if you either didnt care about the inefficiencies or actually planned on predominantly ride at 100km/h, there are limits on what motor kv can work with batteries which is well beyond the scope of my powers of explanation but a good thread can be found here http://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125 and a little bit of context is that electrical RPM is basically the frequency that the ESC needs to switch phases on the motor.  this is realted to the rpm and the number of pole pairs on the motor, most 63xx's have 14 poles and 7 pole pairs.  I'm sure it's all explained better on that thread anyway 

TL;DR
my increasing top speed you stretch out the graph and put yourself on the high amps, low efficiency side.

hope I've been helpful, this is the first time i've felt like i know enough to help someone.
```

---
## \#12 Posted by: ed713 Posted at: 2016-06-18T10:50:52.004Z Reads: 99

```
Duuuude! That post was really gosh darn informative. I think I understand the motors now, as opposed to just doing what everybody is doing. Thanks for the lesson :relaxed:
```

---
## \#13 Posted by: 91Seconds Posted at: 2016-06-18T10:53:25.330Z Reads: 105

```
I've been lurking round these forums not posting anything for a long time in case i was wrong or something so i think it did me well to finally share the knowledge i've gained.
```

---
## \#14 Posted by: Dutch Posted at: 2016-06-19T02:59:23.396Z Reads: 100

```
Thank you for that detailed post. Didn't know to much about the motors so that was very useful to lesrn from.

Also instead of making my own deck i think i actually just by one. Makes it a lot easier.

Saw these longboards at my local home depot for only $30. So that's a good and easy alternative i think. Only have to find some paris trucks and 97mm flywheels and i'm good.

It can hold 176lbs and it's 107 x 22,5 cm which is pretty good i think

<img src="/uploads/db1493/original/2X/0/0549f6728848f28fd30b1225d43480112d37f1d5.jpeg" width="424" height="424">
```

---
## \#15 Posted by: Dutch Posted at: 2016-06-20T19:00:55.907Z Reads: 91

```
Updated entire post with semi-final part list and moved it to builds.
Ordered most of the parts, have to find some of the rest tho.
```

---
## \#16 Posted by: Dutch Posted at: 2016-06-21T23:50:24.168Z Reads: 83

```
Does someone have a basic drawing/measurements of a motor mount ?
Trying to design one to send to the school but i don't have the parts in yet, so i have no clue what the measurements are.
```

---
## \#17 Posted by: ed713 Posted at: 2016-06-22T00:34:47.725Z Reads: 79

```
http://www.enertionboards.com/open-source-electric-skateboard-motor-mount/
```

---
## \#18 Posted by: Dutch Posted at: 2016-06-22T00:58:28.993Z Reads: 79

```
Thank you, must have looked over it while searching!
```

---
## \#19 Posted by: claudiofiore88 Posted at: 2016-06-22T01:36:19.999Z Reads: 79

```
@korryh posted an interesting motor mount design here.

 http://www.electric-skateboard.builders/t/where-do-i-find-post-your-answer-as-a-link/3120/15
```

---
## \#20 Posted by: Dutch Posted at: 2016-06-22T02:05:12.754Z Reads: 77

```
Not sure what the best place is to post this, but i found some cheap flywheels.

Most of the 97mm flywheels are around $100 in my country but found them on Amazon.
https://www.amazon.com/gp/product/B01AZ2US8G/ref=ox_sc_act_title_1?ie=UTF8&psc=1&smid=A2DQMI7AS28KLN

Bought 2 sets of 4 for only $53.98 and free shipping. Guess i have 2 spare wheels now for when i go 6x6.
```

---
