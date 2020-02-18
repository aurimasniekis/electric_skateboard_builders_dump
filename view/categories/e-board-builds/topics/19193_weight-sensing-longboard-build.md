# Weight sensing longboard build

### Replies: 76 Views: 6488

## \#1 Posted by: GIP_longboard Posted at: 2017-03-16T22:40:54.983Z Reads: 443

```
Hello guys,

My name is Lennert and i am part of a team of engineering students (We study mechanical engineering: robotics and mechatronics) assigned with the task to build an electric longboard.
We didn't get any specific tasks so we had to think of some original control ideas ourselves, here is what we came up with: (if you have any suggestions, leave them in the comments!)

- normal RC remote operation
- weight sensing operation
- maximum acceleration based on weight distribution (compensator with force setpoint on front truck)
- maximum deceleration based on weight distribution
- active speed wobble suppression
- torque vectoring curve assist
- alot more


We have currently designed all mechanical parts and are in the process of making them.

We are currently working on the weight sensing of the board.
You basically have 3 options here: strain gauges in a wheatstone bridge, load cells or force sensitive resistors.
We chose for the strain gauges approach since it doesn't require your feet to be on some kind of pads like the Zboard does, and integrates the sensors into your trucks.

To determine where to place the strain gauges we did an FEM simulation to determine the locations of maximum tension and compression.
<img src="/uploads/db1493/original/3X/9/4/94cf54d20969c7945d47a2b1b86f66664e67314a.png" width="690" height="429">
<img src="/uploads/db1493/original/3X/a/0/a00405b509d65f375ecd0fa5d81bf21ee8189a22.png" width="690" height="429">

We use a HX711 load cell amplifier and an arduino to read out the wheatstone bridge:
https://www.youtube.com/watch?v=SyRaMHRWb1A&lc=z13iv5mh0xizv5lyn04chjo5uuijd5mougk

As you can see, we have a good resolution. This data will have to be filtered using a LPF to filter out process noise such as bumps in the road. Measurement noise is pretty low.

We still have a lot to do, and i will update regularly :slight_smile:
```

---
## \#2 Posted by: Blasto Posted at: 2017-03-16T23:03:16.673Z Reads: 390

```
Sounds like a cool project, what university?
```

---
## \#3 Posted by: GIP_longboard Posted at: 2017-03-16T23:08:01.563Z Reads: 381

```
We study at KULeuven in Belgium. And yes, we probably got the most fun project of all students in our master :smiley:
```

---
## \#4 Posted by: TarzanHBK Posted at: 2017-03-17T11:24:58.399Z Reads: 357

```
sounds cool! 
If you go weight sensored, think about an proper algorithm to get rid of sudden acceleration or brakes when you go over stuff. I saw a dude playing around with that kind of thinks and he had an accident going over a rock - board accelerated due to high compression in the sensors and he does some cool aerial flips before the street catched him softly with his face ;)
```

---
## \#5 Posted by: Maxid Posted at: 2017-03-17T11:43:30.935Z Reads: 322

```
Won't carving also give wrong readings?
```

---
## \#6 Posted by: wmj259 Posted at: 2017-03-17T13:04:25.889Z Reads: 308

```
You could make it so the sensor is about the size of a foot versus a small circular pressure pad. 
And carving would somewhat cause a misrepresentation  so maybe the board would have to recognize what position or angle its at.
```

---
## \#7 Posted by: Mrmoonlight Posted at: 2017-03-17T18:30:35.479Z Reads: 293

```
I know if I'm carving hard at higher speeds, there's definitely an increase in pressure and not a time when I would want to accelerate or brake. Also, you would need some way to tell the difference between landing on your rear or front truck and leaning to brake or accelerate.
```

---
## \#8 Posted by: GIP_longboard Posted at: 2017-03-17T18:41:35.080Z Reads: 295

```
Yes, that's what i meant when i said low pass filtering (simple running average/weighted average or even more advanced LPF filters). We will filter out the high frequency noise such as bumps in the road so only the "slower" components of the signal will pass. A bumpy road will be a few Hz at least, and you choosing to go faster or slower will be very slow in comparison :slight_smile:
```

---
## \#9 Posted by: GIP_longboard Posted at: 2017-03-17T18:44:48.681Z Reads: 284

```
The sensors are built into the trucks, so we don't need any pads of some sort. Actually the trucks are part of the sensors this way.
```

---
## \#10 Posted by: GIP_longboard Posted at: 2017-03-17T18:45:51.985Z Reads: 283

```
How exactly would carving give me wrong readings ? could you explain :slight_smile: ? I appreciate the input!
```

---
## \#11 Posted by: GIP_longboard Posted at: 2017-03-17T19:12:58.234Z Reads: 301

```
Got some more done today:
cleaned up the trucks by wrapping them to protect the cables and especially the strain gauges.
Here is a picture of the strain gauges on the surface (this was our test piece, the rest of them are cleaner)
<img src="/uploads/db1493/original/3X/3/6/361d8568673d267a9cb7ad8ac8306564b02406b6.jpg" width="281" height="500">

Here they are protected, so the whole truck is one clean package:
<img src="/uploads/db1493/original/3X/5/e/5ed8691b243c8f8260fb86b34129856a9ed15a54.jpg" width="690" height="388">


We then applied known weight on the trucks so we can actually use the values coming from our wheatstone bridge. This is because the gauges have a +-5% tolerance so no 2 bridges are equal. We then solved a least squares problem to obtain sensor value in function of weight. After which we calculated the inverse so we can have weight in function of sensor value and interpolate between datapoints :slight_smile: 
<img src="/uploads/db1493/original/3X/0/2/02462d17f1741a7dd37a382a3c39e027915eeeb3.jpg" width="281" height="500">

So we can now measure the force/weight applied on the front and rear truck!
```

---
## \#12 Posted by: Maxid Posted at: 2017-03-17T19:21:47.444Z Reads: 280

```
What kind of reading will your sensor give you when you jump up from the board - that is what will happen when carving (just less severe)
```

---
## \#13 Posted by: GIP_longboard Posted at: 2017-03-17T19:36:40.237Z Reads: 280

```
I am not really familiar with longboards, so i even had to look up what this carving technique is exactly. But as i understand it's just fast turning while shifting your weight to the side ?
```

---
## \#14 Posted by: Maxid Posted at: 2017-03-17T23:51:23.362Z Reads: 269

```
You said it yourself - shifting weight. Since your sensor is basically just measuring weight this might be an issue. Also turning requires uneven distribution on the wheels (inner wheel gets pushed down harder) - can you filter this?
```

---
## \#15 Posted by: GIP_longboard Posted at: 2017-03-18T00:32:09.014Z Reads: 273

```
The sensor measures the deformation of the trucks. We will not be using any absolute values, only relative forces between the trucks will be considered (how much % of my weight is on the front/back). As long as both the front and rear trucks are loaded/bent asymmetrically, it should still be fine. But we will have to test this for sure :smile:  If this doesn't work, an accelerometer could be used to determine whether or not we are cornering (sideways G') and adjust readings accordingly. We could also use speed measurements of the wheels to determine this, since the outer wheels should be turning faster. Our professor wants the focus of the project in signal analysis and software/algorithms, and not so much on the mechanical design. Thanks for the insight!
```

---
## \#16 Posted by: Dornacht Posted at: 2017-03-18T03:09:43.116Z Reads: 254

```
Defenatly sounds like a fun project I would suggest a delay in the response from the sensors so that it takes out the outliers such as sudden rocks and body weight shifts and average it out to a gradual change that won't result in loss of control
```

---
## \#17 Posted by: bbq870 Posted at: 2017-03-18T06:24:35.768Z Reads: 253

```
by all means, really, with no offense to you and all my respect for your project: get a longboard and learn to skate first. even pushing a few days on the flat ground. it´s ok for the start.
then get a cheap e-board and see what they do, how they perform.

THEN think of improving these objects.

to me this sounds like somebody wants to make a revolution in F1-engines but doesn´t know about cars at all.
("I heard they are fast and people have fun with them...")

do you know what people use the kicktail for?
```

---
## \#18 Posted by: GIP_longboard Posted at: 2017-03-18T15:03:09.009Z Reads: 245

```
Yes, we will use digital low pass filtering to remove the bumps in the road etc. :slight_smile:
How exactly the weight distribution will control the speed of the board is yet unknown.
```

---
## \#19 Posted by: GIP_longboard Posted at: 2017-03-18T15:15:32.448Z Reads: 243

```
Well, we were assigned this project by the university, we are good engineering students.. but no pro skaters :smiley:
We also can't just buy a working board for this project, since it would kind of defeat the purpose of designing one as an exercise in engineering. I have to admit some experience on the board would help out a lot, but i personally don't expect is to be too difficult to learn. I will certainly consider riding it non motorized for some time to get the hang of it ;) Thanks for your input!
```

---
## \#20 Posted by: Mrmoonlight Posted at: 2017-03-18T17:48:05.962Z Reads: 243

```
Also something to think about is pushing and foot braking. Times when your weight is on a single foot mainly over your front truck. 

Basic scenario. You're stopped at an intersection in back of a car. Car makes a right and you need to move forward a few feet. You manually push with your back foot and balance your weight on your front until you want to stop, at which point you foot brake. 

There are quite a few situations where pushing comes into play on electrics. Sometimes it's a crowded intersection, other times it's when you're passing by a cop, or you just need to save on battery power. 

When it comes to pushing, keep in mind that most people push with their rear foot, but a few people are mongo where they push with their front foot balancing their weight over the rear truck.
```

---
## \#21 Posted by: DougM Posted at: 2017-03-18T17:54:05.691Z Reads: 213

```
You could very easily correlate weight sensing with acceleration statistics - for a given amount of power measure how quickly the board accelerates.  If you add an accelerometer and a tilt-pitch-roll sensor you would also know the attitude of the board as well as acceleration load on all axes.

Then filtering out bumps, rocks and carving loads would be pretty easy.

Wear a helmet when you are testing that board.
```

---
## \#22 Posted by: jmasta Posted at: 2017-03-18T18:08:52.677Z Reads: 207

```
Seems like a cool project!   I'm curious to see how your pressure activated control system works.  Wouldn't you have to de-weight the front to slow down though? That sounds a little sketchy to be honest.  You want to keep your weight over the front truck to maintain stability at higher speeds. Switching your weight distribution could initiate speed wobbles and/or loss of stability

_(Speaking as a 10+ year downhill rider and also a mechanical engineer)_
```

---
## \#23 Posted by: GIP_longboard Posted at: 2017-03-18T18:16:49.763Z Reads: 208

```
Yes, my idea was to build in something like a "launch control" mode, just not for drag racing purposes:
When the board accelerates too fast, your weight will shift back alot and the weight on the front trucks will decrease.
So we take a setpoint for front weight: if its too low (we are falling off), reduce the acceleration. If its too high (we can go faster), increase the acceleration. This could be done by an empirically tuned PID / writing down the differential equations in laplace domain (white box) / doing system identification (black box). There's alot that comes into play we are probably forgetting :D
```

---
## \#24 Posted by: GIP_longboard Posted at: 2017-03-18T18:22:57.917Z Reads: 208

```
Yes, we kind of wanted it to work like a segway, we will have to find out if it works on higher speeds as well. I was kinda thinking to use it as a more "inuitive" way to control the board at cruising speed. Since we will be driving the wheels separately, we were hoping to be able to also implement some sort of active speed wobble reduction controller. It's kind of early in the project to give you answers to these questions, i guess we will just have to find out :wink:
```

---
## \#25 Posted by: brakkeh Posted at: 2017-03-18T20:04:58.287Z Reads: 194

```
Hey guys, is this at GroupT in Leuven?
```

---
## \#26 Posted by: GIP_longboard Posted at: 2017-03-18T20:09:55.322Z Reads: 193

```
No, it is at campus Arenberg (which is like 5min of cycling from GroupT) , are you from Belgium :D ?
```

---
## \#27 Posted by: brakkeh Posted at: 2017-03-18T20:12:18.144Z Reads: 190

```
I'm a student at groupT :) 
I'm in my second year and i'm currently building an electric skateboard. Just have to wait for a few more parts and I can finally start :)
```

---
## \#28 Posted by: GIP_longboard Posted at: 2017-03-18T20:35:02.924Z Reads: 198

```
Ok, nice! Make sure to make a build thread. You can usually find us in the "FabLab" on our campus, where they have cnc laser cutters and 3D printers and other machinery, you only have to pay for the materials as a student of KU Leuven! I don't know if you've been there before ?
```

---
## \#29 Posted by: brakkeh Posted at: 2017-03-18T20:44:22.186Z Reads: 194

```
Ooh yes, i've never been in FabLab myself but we have used it in previous projects. 
Is it also possible to cnc carve the motor mount? I've called to FabLab before but they said they didn't work with metals..
Normally colleagues of my dad would do it at school but they are already four weeks late :s
```

---
## \#30 Posted by: lone_deranger Posted at: 2017-03-19T04:17:10.082Z Reads: 188

```
This has been successfully implemented before.
Have a read through; https://endless-sphere.com/forums/viewtopic.php?f=35&t=49557
```

---
## \#31 Posted by: GIP_longboard Posted at: 2017-03-19T13:54:30.361Z Reads: 186

```
They only do plastics and wood there, which is great for prototyping. There is also a CNC lathe and mill, but they kind of have problems getting it to run (they were working on it 2 weeks ago). I will ask them about it next time i'm there. Doen't groepT have their own cnc machinery ?
```

---
## \#32 Posted by: Kaden56 Posted at: 2017-03-19T20:33:14.492Z Reads: 177

```
Sounds like a fun project! What will you be using to compute everything? I saw you were using arduino's software is there going to be an arduino on board? Or a vesc? Or some other micro controller?
```

---
## \#33 Posted by: GIP_longboard Posted at: 2017-03-19T21:00:39.056Z Reads: 178

```
Yes, we will be using an arduino pro mini. For prototyping we are just using an uno and a breadboard, since they both use the ATMega328, we wont have to change any pins or functions in our code. We will be using vesc's as ESC, but we decided not to program to the STM32 directly, although they have plenty computing power left. Arduino is quicker, easier, cheaper (1$ from Ebay) and has way more online documentation and libraries. It is less powerful however, but it will be plenty for what we want to accomplish.
```

---
## \#34 Posted by: DougM Posted at: 2017-03-21T05:24:47.927Z Reads: 171

```
The only problem I see is that your rider is going to naturally react when those events occur which will change your sensor readings but more importantly, might cause your algorithm's to actually make a bad situation worse.  I would be mighty unhappy if my board reacted in an unpredictable way in a tense situation.

Still, from a research standpoint there's a lot to be learned here.  I would be interested to see intelligence that could make these boards safer.  For instance (you might have already mentioned this) active high-speed wobble suppression, some sort of system that optimizes braking for conditions, etc.
```

---
## \#35 Posted by: Lighthouse Posted at: 2017-03-22T19:55:25.212Z Reads: 166

```
Sensors could work on the trucks, but they would add an extra component to an eboard that is relatively consistent to a rider (same rider would likely maintain weight over boards lifetime). A different route you could take is to customize the riders experience. Boosted and Evolve boards allow you to change between settings but don't let you focus on specific tunes. You could make a motor control component that allows the rider to tune how fast they get to certain speeds and allow input of weight calibrations there. Another cool tune you could try would have trucks that automatically adjust to the speed of a rider. Tightening trucks allows some control of speed-wobble, but the faster you want to go, the tighter the trucks need to be and the less carving you can do. Trucks that adjusted to speed would be unprecedented. 
Sounds like a fun project
```

---
## \#36 Posted by: GIP_longboard Posted at: 2017-03-22T23:07:51.132Z Reads: 159

```
We will probably make an android app that allows the user full control over all calibration and control settings. So you could generate your own custom profiles. And i will think about the tightening trucks for speed wobble suppression, which is completely different to the software approach we had in mind ! I like the idea.
```

---
## \#37 Posted by: Hillso Posted at: 2017-03-31T18:36:18.495Z Reads: 159

```
Love your project!
can I use [this sensor](https://www.aliexpress.com/item/Free-Shipping-10PCS-BF350-3AA-BF350-Precision-resistive-strain-gauge-strain-gauge-for-the-pressure-sensor/1894156024.html?ws_ab_test=searchweb0_0,searchweb201602_0_10065_10068_10136_10137_10138_10060_10062_10141_10056_10055_10054_10059_123_10099_10103_10102_10096_10052_10144_10053_10050_10107_10142_10051_10143_10084_10083_10080_10082_10081_10110_10111_10112_10113_10114_10078_10079_10073_10070_10122_10123_10124,searchweb201603_0,afswitch_1,ppcSwitch_5,single_sort_0_default&btsid=59ec06ea-ff54-4de3-94ce-1eabc590d709&algo_expid=cb78978d-9b56-46e2-951d-765179bf5713-5&algo_pvid=cb78978d-9b56-46e2-951d-765179bf5713) to do the same thing?
```

---
## \#38 Posted by: GIP_longboard Posted at: 2017-03-31T22:27:20.080Z Reads: 176

```
Yes, you can use those strain gauges. Just connect 4 of them for full bridge or 2 for half bridge wheatstonebridge. Then use an amplifier circuit to amplify the signal, after which you can sample it using an ADC. The strain gauges you linked can stretch 2%, so depending on material (young's modulus) and geometry, you have to choose different strain gauges
```

---
## \#39 Posted by: GIP_longboard Posted at: 2017-03-31T22:28:01.057Z Reads: 179

```
first simple test today:
https://www.youtube.com/watch?v=5Al1JnHB7cA
```

---
## \#40 Posted by: DynamicLabs Posted at: 2017-04-01T04:37:39.968Z Reads: 183

```
Very cool project! It is great that this is being built in a research/university environment.  I hope that what ever you discover will trickle down to commercial use one day.

I'm curious as to what kind of sensors you plan to be using for wobble detection.  

We have played around with speed wobble suppression and torque vectoring on our board.  We use a 6 D.O.F. IMU to sense roll angle oscillations, and apply brakes to each wheel accordingly.  I'd like to share some of our insights with you, so hopefully you can come up with a better solution.

- The torque we were able to apply with our hub motors was not enough to totally suppress a speed wobble.  It definitely did help however!  If you want to model the system, I would think of it as an under damped oscillator being driven at natural frequency, with the brakes providing the damping.  So while the amplitude of oscillations did increase, they did so at a slower rate.  A rider would still have to consciously stop the wobble (the rider is the thing driving the system at natural frequency), but since the wobbles build slower, it is easier to do.  Also as a side effect of applying brakes to correct the wobbles is the board slows down which makes the whole situation a little less overwhelming for the rider.
- It can be hard to characterize, identify, and react to a speed wobble.  Something like traction control for a car is easier to identify... if the wheel speed is faster than the vehicle speed, you know you have wheel slip.  For speed wobbles, there is no instantaneous identifier for the event, It takes time for a wobble to build.  Imagine looking at a plot of roll angle vs time.  How would you identify a speed wobble?  You can qualitatively measure it easily... 'a series of oscillations occurring at a certain frequency with increasing amplitude'  But how do you quantitatively measure it?  What frequency is the wobble? (it will change with rider's mass and speed) How fast does the amplitude need to increase to consider it a wobble?  How many oscillations must there be to consider this a wobble?  Once you can answer those you'll need to come up with a detection algorithm to implement it real time.  I imagine you would use fast fourier transform so you can analyze the signal in frequency domain, but it could be computationally expensive and require a lot of samples to get good bin resolution....The characterization and detection algorithm is the biggest issue we are trying to deal with right now.  As a result the wobble correction kicks in too soon and slows you down when you are aggressively carving.  It takes a lot of fun out of the ride...

I hope I didn't bore you with the long explanation.  I really hope you can come up with a better solution than us.  Keep us updated with the project!
```

---
## \#41 Posted by: GIP_longboard Posted at: 2017-04-01T12:28:01.031Z Reads: 165

```
Thanks alot for the input! We also have a 9DOF IMU (I don't think we"ll need the magnetic part, but we got it just in case we got some new ideas). Yesterday, we kind of got all the parts we needed to assemble the board and make it run. So until now we didn't really think about the algorithms involved, since we were busy with mechanical design. We will ask our robotics professor for advice on the speedwobble problem, since he has got years of experience in control theory. He will probably get us in the general direction of how to identify it / derive a transfer function etc..
```

---
## \#42 Posted by: Trillium Posted at: 2017-04-02T09:21:39.784Z Reads: 158

```
Justin at ebikes.ca has been working on that type of system for a while.. hopefully coming to market soon.
```

---
## \#43 Posted by: GIP_longboard Posted at: 2017-04-02T11:13:33.754Z Reads: 158

```
A weight sensing longboard, or one with active wobble suppression ? As far as the weight sensing part goes, if you already have a vesc, you could build it pretty cheap. And it was actually pretty easy to do. The only thing that might be a little hard for the average hobbyist is the math involved: linearizing the in/output using a linear regression.
```

---
## \#44 Posted by: Trillium Posted at: 2017-04-02T19:12:31.981Z Reads: 149

```
Wobble suppression seems like cool tech but completely unnecessary. If you have the right hardware and tuning, you won't get wobbles.

Justin I think is working on conversion kit parts as the rest of his site is geared towards DIY
```

---
## \#45 Posted by: flatsp0t Posted at: 2017-04-02T19:40:25.707Z Reads: 150

```
That is not completely true.
Yes, you can minimize the risk of wobble with the perfect setup, but you cant prevent them completely.
But maybe it is possible in the low speed range Esk8ters normally reach.
```

---
## \#46 Posted by: Trillium Posted at: 2017-04-02T20:04:10.968Z Reads: 153

```
I talked to a pro and he said we should be running different rake in the rear
```

---
## \#47 Posted by: GIP_longboard Posted at: 2017-04-04T23:30:47.364Z Reads: 163

```
All parts (including gears) were drawn in CAD and manufactured in the university workshop by professional machinists.
<img src="/uploads/db1493/original/3X/b/c/bc7cd2234c5ada312535adca71497f31e6c5bf2b.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/1/f/1f5fc3b173aa70c006df089d000bf41b4dbbe5e9.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/5/6/56d3035c70f5cdd33d66681061b154d2df57f25f.jpg" width="690" height="388">
mounted to the board:
<img src="/uploads/db1493/original/3X/0/0/0069c001815fdd3e7e5a92ac356e2906f3cdce38.jpg" width="281" height="500">
<img src="/uploads/db1493/original/3X/5/1/5157d46736206a54902d2f7b687f6a121b725d45.jpg" width="690" height="388">
For safety reasons, we have to write code that checks the validity of each signal we have to process. That way the board will not go skating off on its own when a connector/cable breaks or gets loose.
<img src="/uploads/db1493/original/3X/7/2/72ab82440747f1926221637372e67acea43e90dc.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/d/4/d4a58b7dde53d04fa5bbe313b670fd96799cf93b.jpg" width="690" height="388">
```

---
## \#48 Posted by: GIP_longboard Posted at: 2017-05-24T23:27:35.298Z Reads: 154

```
I haven't updated this page in quite a while, since the hardware part was kind of over. And i didn't think anyone would be interested in software updates and bug fixes (they take quite some time). So here are some quick demos of how it all works together:

Switching from controller mode to weight sensing mode:
https://www.youtube.com/watch?v=HL1xcfIH44k

Safety in remote controller mode, when the user falls of the longboard, it gently comes to a stop:
https://www.youtube.com/watch?v=e_ktwKirD5o

Braking in weight sensing mode:
https://www.youtube.com/watch?v=aH69ZlozDZo

All the safety gear i'm wearing is for liability issues since it's a university project :smiley:
```

---
## \#49 Posted by: mikbeng Posted at: 2017-06-09T07:54:46.482Z Reads: 146

```
Hi,

Really cool project! I was wondering what kind of strain gauges you are using?
```

---
## \#50 Posted by: GIP_longboard Posted at: 2017-06-09T18:58:10.792Z Reads: 144

```
The strain gauges we used were regular onedirectional, +- 5% , 350ohm strain gauges made for aluminium. These specific ones are manufactured by HBM, but there are lots of alternatives. Just make sure you use ones made for aluminium when possible, since these strain gauges have the same coefficient of expansion as aluminium, which makes sure you don't end up with skewed readings when your trucks expand differently than your strain gauges.
```

---
## \#51 Posted by: mason Posted at: 2017-08-03T21:16:58.252Z Reads: 132

```
How's this going? Interested to see an update.
```

---
## \#52 Posted by: GIP_longboard Posted at: 2017-08-04T14:03:34.253Z Reads: 127

```
The project is on hold right now, and we have been assigned different projects. Next year another team of students will continue our work. I think we accomplished quite a lot in only 4 months. We currently have a working weight sensing E-skateboard, with a working android app to switch modes. We were not able to work on other goals like wobble suppression since we only had about 1 month to complete all software which included communication between Arduino, 2VESCS, Strain gauge amplifiers, bluetooth module, remote control. As well as making the app and signal conditioning etc.

I'm sorry if this is not exactly what you expected, but we had about 8 hours a week to work on this since this certainly isn't the only thing we have to deal with in school. If you would like any more info about how we did certain things you can always ask!
```

---
## \#53 Posted by: mason Posted at: 2017-08-04T20:58:54.015Z Reads: 116

```
Understood. Remarkable work in the time you had!
```

---
## \#54 Posted by: Trdolan03 Posted at: 2017-09-24T05:35:29.353Z Reads: 105

```
Any chance that you could post your code? I am really onterested in trying it out on my personal board. Really cool tech you have here...
```

---
## \#55 Posted by: GIP_longboard Posted at: 2017-09-30T13:40:58.837Z Reads: 102

```
Which part of the code are you interested in ? We didn't have much time to code left so it really is a mess :smiley:
```

---
## \#56 Posted by: Vanarian Posted at: 2017-09-30T14:43:54.295Z Reads: 110

```
Cool to see you connected ! I'm sending you a PM! I learn to make a similar thing with 4x wheatstone bridge cells and mpu6050 combo with each VESC. 

If you're willing to share your code I'd be very grateful as it will allow me to get to ride my skates sooner than I hoped.

Do you have the following parts available by chance ?

[quote="GIP_longboard, post:1, topic:19193"]
weight sensing operation
maximum acceleration based on weight distribution (compensator with force setpoint on front truck)
maximum deceleration based on weight distribution
[/quote]

I'll figure out how to adapt it !
```

---
## \#57 Posted by: GIP_longboard Posted at: 2017-09-30T15:42:39.296Z Reads: 116

```
Ok, i can't seem to find the code but i can tell you how the algorithms worked. But they weren't perfect by any means!

Weight sensing:
we used proportional current control based on the weight distribution:
weight distribution: weight_front/(weight_front+weight_rear)
Every rider has a different riding position, some stand 55%, some 50%. So we added a calibration using the android app.
You got into your "neutral" position and then this was saved as a calibrated value.
let's say you neutral value was 60% (so in neutral position 60% of your total weight was in the front), full forward was 70% and fully leaning backwards was 40%.
You then have a range from 60-70 pct which was mapped from 0 to max_current.
You then also have a range from 40-60 which was mapped from max_braking_current to 0.

We then still had the following problem:
When the board accelerates you lean backwards, which makes the board think it should brake. once it started braking, your weight shift to the front again and it started speeding up. Cycle repeats :smile:
We just added a low pass filter to the current signal to the motor so smoothen things out a bit. This of course also added some delay, so had to find some tradeoff. 

Now the maxiumum acceleration based on weight distibution:
Our goal here was to use the RC remote, but make the board accelerate in such a way you couldn't fall off.
So at for example 50% throttle, you want 40% of the riders weight in the front, and at 100% throttle you want 30% of the riders weight in the front.
This was done using a PID controller, so once you leaned back too far (falling off), it slowed down a bit. And when you leaned too much to the front (you still have room to accelerate), it sped up. Same thing for the maximum deceleration.

We didn't use out 9DOF module or torque vectoring of any kind. We bit of more than we could chew :wink:
```

---
## \#58 Posted by: Vanarian Posted at: 2017-09-30T20:02:07.539Z Reads: 103

```
Ok thanks for the tips, that's already a good base for me ;) if you find some code back hit me up ! I'll upload what I've done once I get something working.
```

---
## \#59 Posted by: GIP_longboard Posted at: 2017-10-01T00:17:49.703Z Reads: 101

```
Ok, will be interesting to see how others tackle the same problems! :wink: 
I know the low pass filtering of the current signal isn't really the real solution to our problem, and you could probably somehow compensate for the rider falling backwards a bit. But we couldn't really come up with a simple algorithm to model the human balance (and again, every rider has a different COG etc.)
```

---
## \#60 Posted by: Vanarian Posted at: 2017-10-09T21:27:24.666Z Reads: 92

```
If I manage to get a simple "calibration step" to adapt the sensitivity of the strains to each rider it could do the trick with the low pass filter ! Now main issue is I'd like to get an input reactivity of under 20ms max with total calculs... that's asking a lot compared to simple Rf transmitters but it could do the trick. 15ms timing would make the delay virtually undetectable but then signals need to be very relaible. 

Back on the desk !
```

---
## \#61 Posted by: Trdolan03 Posted at: 2017-10-09T23:55:52.697Z Reads: 86

```
So let me confirm that I have my parts list correct here. 
To use the strain gauge setup, you need 
2 strain gauges
A single wheatstone bridge
A low noise filter
An arduino or similar processor
Is this correct?
```

---
## \#62 Posted by: GIP_longboard Posted at: 2017-10-10T00:06:48.980Z Reads: 88

```
1) Yes, you could use 2 strain gauges and make 2 quarter bridge wheatstone bridges.
However, i used a full bridge configuration since it is more accurate and also is less influenced by external factors such as humidity or temperature.

2) The wheatstone bridge was just made using some wire, but a pcb is also possible

3) The low pass filter was implemented in software since you will probably have to tweak the settings a little. This can be exponential smoothing or some Finite Impulse Response filter, I used a FIR, but didn't really put alot of thought into this decision to be honest.

4) you will also need an external ADC since the ADC built into the arduino has very poor resolution with respect to the voltage deflection the wheatstone bridge will put out.
```

---
## \#63 Posted by: Trdolan03 Posted at: 2017-10-11T04:18:25.827Z Reads: 73

```
Will the INA125P voltage amplifier compensate for the adc or do I need something else?
```

---
## \#64 Posted by: GIP_longboard Posted at: 2017-10-11T23:00:15.355Z Reads: 70

```
I used a HX711, which is a voltage amplfier followed by a high resolution ADC.
But you could also use just a voltage amplfier in such a way that you use the complete range of the (lower resolution) arduino ADC. I don't think you need the external ADC since the extra resolution is probably overkill.
```

---
## \#65 Posted by: taroko Posted at: 2017-10-12T01:40:42.499Z Reads: 73

```
Did you modify your HX711 to run at 80sps or left it at 10sps? I haven't tried 80, but I saw a document mentioning that there is a lot more noise at the higher sampling rate. The only problem I have with the HX711 is that it does not explicitly indicate strain gauge failure.
```

---
## \#66 Posted by: Trdolan03 Posted at: 2017-10-12T02:14:02.214Z Reads: 71

```
@taroko So do you use the hx711 or something similar? Also, have you figured out how to bulletproof the HX711 from a strain gauge failure?
```

---
## \#67 Posted by: taroko Posted at: 2017-10-12T02:32:43.700Z Reads: 73

```
I use HX711. I don't have a good solution for strain gauge failure yet. I just detect the following: 1) If the weight reading jumps to an abnormal reading (like a high negative value) 2) if the weight show very little variation.

These detection methods are not bulletproof, but I'll live with it for now. For my next version, I may consider using a volt amp instead. I'm just hoping that I don't rip my strain gauges off while I'm riding.

What I do like about HX711 is that I can convert the sensor signal to digital near the sensor.
```

---
## \#68 Posted by: Trdolan03 Posted at: 2017-10-12T03:34:51.722Z Reads: 71

```
@taroko Ok thanks for the help. I have a year long school project for which we are building one of these. I will dedicate a really good portion of that time to the programming in which I will try to bulletproof it. I will report back with any questions or triumphs.
```

---
## \#69 Posted by: Trdolan03 Posted at: 2017-10-12T04:05:16.206Z Reads: 70

```
@taroko One more thing for now, how do you change the sps of the HX711 board?
```

---
## \#70 Posted by: taroko Posted at: 2017-10-12T06:55:21.803Z Reads: 68

```
If you get the sparkfun version, you can cut a connection on the board. See this thread: https://forum.arduino.cc/index.php?topic=479175.0

The generic breakout boards are not as convenient.
```

---
## \#71 Posted by: GIP_longboard Posted at: 2017-10-12T13:02:13.314Z Reads: 66

```
I left it at 10 sps, the higher sampling rate doesn't really improve responsiveness if you low pass filter it like we did anyways.
```

---
## \#72 Posted by: GIP_longboard Posted at: 2017-10-12T13:05:40.850Z Reads: 67

```
If one of the strain gauges gets damaged, they basically become an open circuit and you will get readings that are abnormal, like a factor of 1000 bigger than usual. You did it the same way we did it. But we always used a remote for extra safety during testing.
```

---
## \#73 Posted by: Trdolan03 Posted at: 2017-10-12T21:47:41.425Z Reads: 64

```
Alright. I know that I am being obnoxious but I have one more question. If I am using 2 total strain gauges, one in the front and one in the back, how would I wire the Wheatstone bridge. The strain gauges are 350 ohm ones...
```

---
## \#74 Posted by: taroko Posted at: 2017-10-13T02:36:16.913Z Reads: 61

```
Are you using just 1 strain gauge for each truck? If so, I would use **quater-bridge type I** (see link below). With quarter-bridge your signal to noise ratio will be lower. Let us know if quarter works ok. 

I'm using full bridge at this time which seems to work well, but this might be over kill. I"ll test half bridge in the future.

https://www.transducertechniques.com/wheatstone-bridge.aspx
```

---
## \#75 Posted by: skyblaster Posted at: 2017-10-23T16:52:26.229Z Reads: 61

```
When you want to sense weight over the rear of the board, but do not require a precise measurement (ie. in a comparator circuit), would you still use a strain gauge, or another form of pressure sensor?

EDIT: Disregard the switch in the example circuit below.
https://www.circuitlab.com/circuit/7whd4t/strain-gauge-comparator/
```

---
## \#76 Posted by: G-Motionboard Posted at: 2018-12-24T15:12:46.315Z Reads: 32

```
Well done, it looks you got how to make it, it's really unbelievable you make such great progress in just 4 mouths. 
but in my experience, you just got how to start and you are still far away to the complete and perfect it. 
From the quick demos, i can see the acceleration and braking is not smooth enough, actually, i should say the acceleration and braking both are not sensitive enough, it means you should test and modify the value of current control  which is based on the weight distribution, it should be more elaborate, i'm not sure you can get a good result after a lot of test, but if you need a better idea, i would like to advise you use best weight sensor and the change the % to accurate weight, then make the current control based on the weight changes, you will get a much better performance.
anyway your this project is on hold already, so you may can't make it now,  it's a little pity that i read your post so late. Otherwise we can have a interesting communication.
good luck!
```

---
