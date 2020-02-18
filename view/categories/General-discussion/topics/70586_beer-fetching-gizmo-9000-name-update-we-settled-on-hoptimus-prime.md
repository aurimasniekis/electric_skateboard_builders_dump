# Beer Fetching Gizmo 9000 (name update we settled on HOPTIMUS PRIME)

### Replies: 17 Views: 415

## \#1 Posted by: wafflejock Posted at: 2018-10-08T18:49:08.161Z Reads: 180

```
Beer delivery robot, need I say more... probably.

So at my day job we typically develop web applications for big companies (I work for a consulting company based out of Seattle but work in Chicago), but as a fun side project we plan to build a 'bot' that can bring you beer wherever you are in the office.  Since I'm one of the few people in the office with any sort of experience with electric motors and building a 'drive train' for my esk8 I've been deemed the drive-train/motor guy and am looking for some advice on how to size the motor and gearing.

Requirements:
  - Safe (it needs to go 4mph max and typically will go 3mph)
  - Quiet (it will roam the office, probably near the end of the day, but it needs to be as quiet as possible)
  - Powerful, it needs to be able to pull at least 90lbs (weight of a cooler full of ice/beer)

Price isn't really a major concern since the company will cover the costs here but I need to be sure the motor will perform well enough given the parameters.

I found a calculator and equations on the robotshop.com website and have started with numbers from there, I'm thinking based on those calculations (and a bit of gut feeling) we'll need at least 300W motors, but I'm having trouble really groking how to account for the pulleys/gear ratio and all.  Guess I'm wondering what is the right way to choose a motor here and if anyone has ideas/suggestions regarding the drive train in general to keep it as quite as possible (so far I'm just thinking sensored BLDC motor with FOC mode and belt/pulley driven).

(appears they have fixed the calc and are actively refining the site but hopefully this link works for a bit https://www.robotshop.com/community/tutorials/show/drive-motor-sizing-tutorial )

I'm thinking about getting a pair of these:

https://hobbyking.com/en_us/turnigy-sk8-5045-150kv-sensored-brushless-motor-14p.html?___store=en_us

Along with a pair of VESCs (probably VESC6 but open to other updated options if anyone has a suggestion)

Again quiet is key so if we can get lower RPM motor that still has the torque necessary and isn't $1000 please let me know.
```

---
## \#2 Posted by: Trdolan03 Posted at: 2018-10-09T20:02:11.480Z Reads: 135

```
That motor will work fine in FOC mode and be nearly silent. VESC 6 will be overkill. FOC Box would work just fine but I guess if you aren’t concerned about cost this doesn’t matter.
```

---
## \#3 Posted by: stormboard1 Posted at: 2018-10-09T20:20:14.015Z Reads: 128

```
Foc box in foc is best option..vesc6 is total overkill..
Really cool project i like it
```

---
## \#4 Posted by: wafflejock Posted at: 2018-11-02T16:24:10.408Z Reads: 109

```
Still waiting on budget approval but should happen in the next week or two.  Random question if we were to get the Unity with two focboxes in one can we send two control signals into it to drive two motors separately (for differential steering) or should we go separate ESCs.

https://www.enertionboards.com/focbox-speed-controller/focbox-unity-dual-motor-foc-controller-esc/

^^ is what I was thinking of for the dual one

Put the question out to enertion support as well but will be a day before I get a response there.
```

---
## \#5 Posted by: Sebike Posted at: 2018-11-02T16:45:11.026Z Reads: 89

```
This will eventually turn into a build thread as your project progresses, right? :heart_eyes_cat:
```

---
## \#6 Posted by: wafflejock Posted at: 2018-11-02T16:47:41.356Z Reads: 85

```
Hah yah I'm hoping everyone at the office is okay with opening up the instructions (and code) we'll probably have to slap all sorts of disclaimers on things if/when we release them, but I'll post as much as I can without getting in trouble for sure.
```

---
## \#7 Posted by: dougpage Posted at: 2018-11-02T16:52:02.889Z Reads: 80

```
[quote="wafflejock, post:4, topic:70586"]
Random question if we were to get the Unity with two focboxes in one can we send two control signals into it to drive two motors separately (for differential steering) or should we go separate ESCs.
[/quote]

You should ask @Deodand or someone else in the focbox unity chat. I cant wait to see where this goes!
```

---
## \#8 Posted by: marsrover001 Posted at: 2018-11-02T16:55:19.205Z Reads: 68

```
I hate to say it, but sealed geared brushed motors are often the most quiet and have the power you are looking for.

Find an old powered wheelchair, take it apart. Apply an adruino to stand between the nav sensors and the esc controls. Done.

Basically stealing all the ideas from here. https://www.youtube.com/watch?v=9ro0_lJSNLw
```

---
## \#9 Posted by: Deodand Posted at: 2018-11-02T16:59:45.446Z Reads: 66

```
differential signals to two motors on the unity is supported! Easiest way to achieve this is through uart/usb depending on what your control unit is (arduino/embedded linux i.e. raspi)
```

---
## \#10 Posted by: wafflejock Posted at: 2018-11-02T17:02:43.792Z Reads: 65

```
Thanks for the confirmation and feedback.  Regarding control computer we do plan on using a raspberry pi for the time being, possibly upgrading to a latte panda or some other more robust board if need be but for now going with movidius compute sticks for doing some on board computer vision and possibly SLAM processing on board (we are still working out the software architecture with ROS to decide what can happen on board and what will happen on the server).

--- 

Regarding geared drive I was avoiding these due to the gear noise and figured the FOC mode with BLDC motors would get the quietest drive system possible but I'll look into the video and quiet geared options too.
```

---
## \#11 Posted by: Deodand Posted at: 2018-11-02T17:05:38.388Z Reads: 70

```
Yeah FOC at 30 kHz is near silent. The key to getting the quietest possible is making sure the motors are mounted with some rubber grommets between to isolate resonance with the frame they are mounted to. Can't speak to sealed geared motors, all the geared motors I've used are very noisy.
```

---
## \#12 Posted by: dougpage Posted at: 2019-05-10T05:50:21.838Z Reads: 51

```
Do you have any updates on this masterpiece?
```

---
## \#13 Posted by: wafflejock Posted at: 2019-05-10T15:05:28.953Z Reads: 48

```
Unfortunately not yet, we've discussed it a bit further here in terms of which wheels to use for the casters and looked at some soft coolers, but think we're stuck a bit on budget (also main dev who was heading this up has just been slammed with project work so hasn't had time to keep pushing on it).  We're doing another robocar rally thing (AWS AI related project for self driving) so maybe can get some more people excited about doing it there.  We've hyped the idea at a few other hackathon events at work, and people are into it they're just not sure about throwing down all the monies without a more real proof of concept... we have an RC car with sensors (ultrasound, 2d lidar, and camera) and a co-worker got all that being read and displayed from a raspi but we need to show some of the self driving and no one has had the time.

Can see the concept model I put together here too: https://cad.onshape.com/documents/f1317a5480b3e931d5786193/w/7ec61a9fc070a170eb64e044/e/343963f512020ae2d4d7c93f

But yah a little bummed we don't have a lot of physical stuff to show for it yet.
```

---
## \#14 Posted by: evoheyax Posted at: 2019-05-10T16:46:47.393Z Reads: 37

```
I would really recommend picking up one of the rpi 360 2d lidar units. You can use it to map out the environment and feed that data into a neural network so the robot can learn the environment, and avoid objects in real time.
```

---
## \#15 Posted by: wafflejock Posted at: 2019-05-10T18:48:29.443Z Reads: 28

```
Pretty sure there's a new revision but we have one of these on there already https://www.slamtec.com/en/Lidar/A2

For the robocar rally thing AWS hosts it just uses a RPi and webcam and control input from the user to feed into a neural network to train the network to give the correct control input based on current stream from the web-cam so we'll be doing some NN stuff.  For the lidar and ultrasounds I think we were planning to mostly use them for immediate object avoidance and the NN for driving assuming the close proximity sensors don't have an issue with the control input the NN has "decided" on (basically if NN says go forward we'll check lidar and ultrasounds to see if that's a viable option or reject the control input until whatever is in the way gets cleared or maybe feedback mechanism for NN to pick a new direction to try.... these are things that need to be worked out).

We also started exploring ROS and the messaging bus it has setup for passing events/messages between different systems (currently being used for reading sensor data and publishing it for sensor consumers, but that's as far as we've gotten on that front).
```

---
## \#16 Posted by: evoheyax Posted at: 2019-05-10T19:01:26.261Z Reads: 28

```
Yep. There is an a3. I use the a2 myself as it was a fair bit cheaper when I got mine. I’m using it on a semi self driving electric bike, and so far, it seems to be good. Not done with my project yet though.

Wish I was in Seattle. I would stop by and check this bot out as it seems really cool.
```

---
## \#17 Posted by: wafflejock Posted at: 2019-05-11T16:21:24.518Z Reads: 17

```
Oh hah thanks for checking out the company we're actually in the Chicago office, though we're hoping if we can show this works here they will adopt the plans at other offices too.
```

---
