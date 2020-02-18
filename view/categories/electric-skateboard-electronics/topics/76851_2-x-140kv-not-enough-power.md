# 2 x 140kv not enough power?

### Replies: 44 Views: 659

## \#1 Posted by: Soulnatcher Posted at: 2018-12-02T23:49:27.829Z Reads: 194

```
I just totally changed my board electronics and mechanics. I was running one 36v 600w brushed dc motor with 100mm wheels with 16tooth motor pulley and 44tooth wheel pulley and cheap chinese ebike esc and board would push me just fine. I'm 225lbs but I could start from stand still even on incline, maxed at about 25mph and had no issues with hills. Changed over to two 140kv brushless motors, two 4.12 VESC, 6" (150mm) wheels, 15tooth motor pulley and 40tooth wheel pulley and no dice. It peels rubber without me on it but when I get on and pull the trigger it just makes a bunch of racket (like ba ba ba ba ba... that would be cogging i guess?) and wont move. Belts are plenty tight, I'm not skipping or shearing teeth, board just won't move. I have 36v 10S 6P battery and my settings are motor max 75A motor min 50A battery max 35A battery min (brake) -4A. Using Y servo splitter because when I tried slave/master only master would turn. Two 140kv motors should be plenty enough torque... I'm very frustrated. Has anyone got any ideas on what the problem could be? Any help is greatly appreciated.
```

---
## \#2 Posted by: J0ker3366 Posted at: 2018-12-02T23:56:44.395Z Reads: 180

```
Phase wires may be shorting, vesc seetings not set right, shorted motor wires (check the mounting screw arent too long).
```

---
## \#3 Posted by: Jmding Posted at: 2018-12-03T00:02:06.147Z Reads: 173

```
Did you do your motor detection with the belts removed?
```

---
## \#4 Posted by: Soulnatcher Posted at: 2018-12-03T00:04:25.370Z Reads: 172

```
@JOker3366 thanks for reply. I made sure screws aren't too long, I calibrated remote in bldc tool, and I'm not using extended cables (only using the length that came on motors). Which vesc settings not right? Wouldn't it run poorly even with no load if motor wires were shorting?
```

---
## \#5 Posted by: Soulnatcher Posted at: 2018-12-03T00:05:23.021Z Reads: 160

```
Yes. Wheels were not even attached.
```

---
## \#6 Posted by: Jmding Posted at: 2018-12-03T00:11:22.844Z Reads: 150

```
If you are moving already, does it accelerate well? I.e. is it only a problem when accelerating at a dead stop? Thinking if there might be an issue with stator position detection somehow...
```

---
## \#7 Posted by: Fiori Posted at: 2018-12-03T00:11:30.616Z Reads: 146

```
So the board doesn't go at all? Or it does but you are not satisfied with the torque?

If you are running 15/40 on 6 inch wheels thats part of your toque issues. I run 66T on 175mm wheels. 

Also, the cogging or shuddering you explain is normal if you are running sensorless. You have to push off once and then hit the throttle with sensor-less.

EDIT: Also need to know:
-Battery Cell Type/size/capacity(30Q cells?)
-Battery Voltage
-Do you have a bluetooth module?
-Do you have the bluetooth app installed?
-Picture of Vesc settings.
```

---
## \#8 Posted by: linsus Posted at: 2018-12-03T00:16:34.355Z Reads: 139

```
Kv does not specify Power of the motors. Only relation of copper wounds on stator.

Either way, if uncensored, cogging is normal. Try pushing first. Else id guess bad detection
```

---
## \#9 Posted by: Soulnatcher Posted at: 2018-12-03T00:17:46.222Z Reads: 136

```
I've tried pushing first it still does same thing. With the 600w brushed dc I could start without pushing even on an incline and also could creep along very slowly if i wished but you're saying I won't be able to do the same with two 140kv motors? Idk about using bigger wheel pulley, esk8 calc said it should hit about 33mph loaded with the ratio I have and thats plenty fast for me...
```

---
## \#10 Posted by: lrdesigns Posted at: 2018-12-03T00:18:21.610Z Reads: 135

```
[quote="Fiori, post:7, topic:76851"]
Also, the cogging or shuddering you explain is normal if you are running sensorless. You have to push off once and then hit the throttle with sensor-less.
[/quote]

Sounds like this to me. :arrow_up:

Are these motors 5065 size?
```

---
## \#11 Posted by: linsus Posted at: 2018-12-03T00:19:32.798Z Reads: 123

```
[quote="Soulnatcher, post:9, topic:76851"]
I won’t be able to do the same with two 140kv motors
[/quote]

Staph.. Kv is not equal to Power
```

---
## \#12 Posted by: Soulnatcher Posted at: 2018-12-03T00:29:20.087Z Reads: 108

```
Yes motors are BRH5065 140KV.  Battery is 10S 6P lgeamf11865 18650's 2200mAh.
```

---
## \#13 Posted by: Fiori Posted at: 2018-12-03T00:29:32.686Z Reads: 110

```
These aren't your 600W brushed motor. They are different.

You can do the same thing with your "140kv motors", it just has to be set up correctly. 

Yes 33 mph is fast, but high top speed does not == torque. A 60T pulley would but you a lower top speed, but MUCH higher torque. Which is what you said you wanted(you said going up hills). 

IF you get the info I asked for we may be able to help you get it set up correctly.
```

---
## \#14 Posted by: Soulnatcher Posted at: 2018-12-03T00:31:40.781Z Reads: 103

```
Battery is 36v. No bluetooth.
```

---
## \#15 Posted by: Fiori Posted at: 2018-12-03T00:32:59.304Z Reads: 101

```
Cell Type/Brand/Capacity.

The actual voltage of your battery with a volt meter.
```

---
## \#16 Posted by: Soulnatcher Posted at: 2018-12-03T00:34:32.080Z Reads: 102

```
Fully charged with voltmeter is 41.5 volts, that's what I cut off the charging at.
```

---
## \#17 Posted by: Fiori Posted at: 2018-12-03T00:35:37.316Z Reads: 103

```
Ok so your battery is working fine. Do your motors have only 3 large wires, or does it have 3 large wires and several small ones?
```

---
## \#18 Posted by: Soulnatcher Posted at: 2018-12-03T00:37:03.144Z Reads: 104

```
It has sensor wires also but 255 error on hall detection so they are not attached.
```

---
## \#19 Posted by: Fiori Posted at: 2018-12-03T00:49:05.002Z Reads: 102

```
Ok. With the sensors not setup or attached you will not be able to start from a stand still. You will have to push off first.
```

---
## \#20 Posted by: Soulnatcher Posted at: 2018-12-03T00:53:24.581Z Reads: 99

```
Ya I keep hearing that but it does same thing when I push. Just wont go with load.
```

---
## \#21 Posted by: Soulnatcher Posted at: 2018-12-03T00:56:17.179Z Reads: 92

```
Starting to wish I had just kept the heavy dinosaur. Weight was the only real issue. It was way cheaper (esc only $15), worked better, and was much more reliable than this brushless crap.
```

---
## \#22 Posted by: Jmding Posted at: 2018-12-03T01:10:15.932Z Reads: 93

```
Yeah I hear your, this stuff can get frustrating sometimes. This is the way DIY often is, its just the price you pay I guess.

Its not that you dont have enough torque.  If you are running 75A motor max for each motor (which, btw, is probably too high for 5065 motors to reliably run at), even with 6" wheels and relatively tall 15:40 gearing, you should have 50% more thrust than a boosted dual plus at startup.

What you're describing is pretty odd. If I were you, I would start my debugging process by only connecting one motor and VESC, in sensorless BLDC mode. It's a little hard to assess what the issue is remotely, all I can say is pay close attention to what's going on and look for clues I guess. 

Also, using a Y-splitter is supposedly a very bad practice and can apparently destroy VESCs somehow. I dont know why, and it makes no sense to me, but you should look into it. There might be a clue in there somewhere.
```

---
## \#23 Posted by: Jmding Posted at: 2018-12-03T01:16:15.381Z Reads: 96

```
Maybe something in here might help:
https://www.electric-skateboard.builders/t/y-piece-or-canbus/26461

Also wondering why slave/master isn't working. That might be a symptom of some deeper problem.
```

---
## \#24 Posted by: Santino Posted at: 2018-12-03T01:23:53.128Z Reads: 92

```
I would solve the sensor issue, also 40 max motor amp (will try not to saturate the stator with a low kv motor), and I do motor detection with tires on...Check your remote trimming is ok, 0,10 sec for remote to accelerate and stop, PPM no reverse with break. Check if can bus y correct, it should work...Best of luck!
```

---
## \#25 Posted by: Fiori Posted at: 2018-12-03T01:27:46.830Z Reads: 88

```
The brush less motors are not crap, they are easily twice as strong as your old motor. I think you have something configured incorrectly in VESC.

You may have your motors hooked up wrong too. Try switching around any of the 3 motor wires.
```

---
## \#26 Posted by: lrdesigns Posted at: 2018-12-03T01:48:44.776Z Reads: 85

```
Did you change the vesc voltage range, if that is set wrong it can cause you to have no power under load. The esc goes to a limp mode to save the battery. 

I have these exact motors, my board has plenty of power for 200lb person. More than enough power for street use on urethane. 

It has to be something do to with vesc settings. 

I also had trouble getting the sensors to work, but was worth the effort. I tried different combinations of sensor wires and phase wires. Even though the sensor wire order is not meant to matter. Eventually I got a combo that worked. 

Keep in mind im on 12s lipo. But here is mine. 
![image|519x105](upload://o4PGOXoRXbHEf7HRhbHBzRqDBov.png) 

![image|627x226](upload://ztTc09nAwee0KkvHQqmFIJLqWaW.png) 

I also upped my minimum current which helps it stutter less from zero speed. And upped the start up boost just a little. 
![image|613x124](upload://fH5xbTFPLzYjPp7oEM0WSY8Qjcy.png) 

![image|617x227](upload://kjDEEXW43xxWcUajjqgjnf7fKAd.png)
```

---
## \#27 Posted by: dareno Posted at: 2018-12-03T01:52:39.149Z Reads: 77

```
[quote="Jmding, post:22, topic:76851"]
Also, using a Y-splitter is supposedly a very bad practice and can apparently destroy VESCs somehow. I dont know why, and it makes no sense to me, but you should look into it. There might be a clue in there somewhere.
[/quote]

Not true at all.  Removing the canbus while both vescs are powered will destroy vesc but split ppm is not bad practice.  
I know you are trying to help but stick with the issues at hand and the guy won't get confused.  
@Soulnatcher  My friend if you are experiencing this much strife from your set up then it is badly configured.  Do as @Fiori has asked and provide the info so we can help.
```

---
## \#28 Posted by: Pedrodemio Posted at: 2018-12-03T02:08:07.500Z Reads: 74

```
75A on these motors are way too high, try 40A first, what could be happening is that in trying to start you saturate the motor and the VESC completely looses tracking making them stutter 

Try to get it working without sensor first , I run 5055 sensorless and they have plenty of torque to start on flat, sensored they will start you on hills no problem
```

---
## \#29 Posted by: Soulnatcher Posted at: 2018-12-03T02:56:36.253Z Reads: 73

```
@Fiori if I switch any of the 3 motor wires around won't they run in reverse? @Irdesigns no I did not touch the voltage range and vesc tool said 34v low battery and 31v cutoff but I have mine set to low of 34v and cutoff at 33v, @Pedrodemio in reading through the forums I saw several places where it was suggested to increase the motor amps for more power and that it was ultimately regulated by the battery amps (motor won't get more than battery can deliver) but that increasing the motor amps and/or lowering the battery max amps somehow also increases power... Is that not true? Also, my cells are rated for 10A discharge so with a 6P battery they could really be set to 60A max correct? So If I do as you suggest and lower the motor amps to 40 what do you suggest I set the battery max amps to?
```

---
## \#30 Posted by: lrdesigns Posted at: 2018-12-03T03:05:04.701Z Reads: 73

```
[quote="Soulnatcher, post:29, topic:76851"]
I have mine set to low of 34v
[/quote]

Ok, is your pack fully charged? If its at 36v or below it could be the issue. Can you check it with multimeter or in vesc tool. 

Yes changing any two phase wires will make it run backwards. For me it was a combo of sensor wire arrangement and phase wire arrangement that got them to pass the test in vesc tool. 

But you can flip the direction in software. So it was more a matter of getting the sensors test to pass, then switch the direction in software. 
![image|645x151](upload://ihSvnra0aRzyp2cnMP5dARv52TR.png)
```

---
## \#31 Posted by: Soulnatcher Posted at: 2018-12-03T06:09:32.443Z Reads: 59

```
@Irdesigns Ok gotcha on the sensorl wiring. Battery fully charged I stop it at 41.5v. What I'm inquiring about though is the max battery AMP setting not the volts. You said I should have motor max at 40A so what do you suggest my battery amp max should be?
```

---
## \#32 Posted by: lrdesigns Posted at: 2018-12-03T06:23:26.390Z Reads: 58

```
Id start at 15 to 20 amps x2 for battery and see how it is.

Your original setting should work though so its something else.

I think if you post screen caps of all the settings maybe someone can find something that could cause this no torque issue.
```

---
## \#33 Posted by: Andy87 Posted at: 2018-12-03T07:32:26.588Z Reads: 53

```
definitly would be helpfull if you post some screenshots of your vesc set up.
```

---
## \#34 Posted by: Soulnatcher Posted at: 2018-12-03T08:09:00.230Z Reads: 51

```
ok I'll pull it all apart again and take screen shots but I already told you what settings are... running split servo, sensorless, current no reverse with brake, 75A motor max -50A motor min, 35A battery max -4A battery min, battery low 34v battery cutoff 33v, and I didn't change anything else.
```

---
## \#35 Posted by: Andy87 Posted at: 2018-12-03T08:12:11.597Z Reads: 50

```
yeah but, is your ppm right adjusted?
do you get any fault messages when motors don´t start spinning?
how about your motors if you spinn them without wheels attached?
the run easy and without sound or stop fast?
```

---
## \#36 Posted by: Andy87 Posted at: 2018-12-03T08:14:28.868Z Reads: 49

```
if you don´t want, than you don´t need to make screeshots...
as i understood the easy things which could cause it are not the reason...
so pictures from your build and screenshots can maybe help. maybe....
```

---
## \#37 Posted by: Soulnatcher Posted at: 2018-12-03T08:21:46.240Z Reads: 51

```
PPM right adjusted? I set controller in vesc tool in mapping, I believe it was 0.9 something start 1.4 something middle and 1.9 something end for both motors. Motors both spin up fine with or without wheels (when I set them the wheels were not attached), no faults except if I try to connect sensors then I get 255 error, or if I try can bus then only master spins. They both run easy without sound except for the normal whine or whir of a brushless motor and only stop fast if I hit the brake.
```

---
## \#39 Posted by: Soulnatcher Posted at: 2018-12-03T08:35:21.351Z Reads: 50

```
bldc not foc
```

---
## \#40 Posted by: AlexBE Posted at: 2018-12-03T08:35:48.338Z Reads: 50

```
As someone above suggested, I would completely disconnect one motor. You need to isolate the issue. If you have the setup on your bench, with USB connected, can you grab a motor with your hand and get high torque? What do the currents go to?
```

---
## \#41 Posted by: chrisLawrence Posted at: 2018-12-03T09:57:31.996Z Reads: 48

```
I totally agree -- you need about 58t for 6"  to increase the torque.

My evolve on ATs (with 140kv 5065s at 36v) ran fine with the standard AT gear (66t?).

Nothing like the 6374s, 12s, and 8" using 13/66t though :smiley:
```

---
## \#42 Posted by: Soulnatcher Posted at: 2018-12-03T10:11:37.856Z Reads: 49

```
@Pedrodemio & @Irdesigns & @Santino Thank you. I believe you guys nailed it, at least the vast majority of it. I changed the current settings to 35 motor max -35 motor min, 20A battery max -3A battery min, 1A minimum current and now it goes & even w/o pushing, I just put my weight on front foot to start Still got some tweaking to do as I was hoping to get a lil better performance out of these motors & I still gotta try to get sensors working but at least it's now functional. I tried to select all of you for solution answer but I don't know if it will allow me to or not, if it doesn't just let me know and I'll ask a new ? and allow whomever got dissed to solve it for me so that you get credit too. Everyone's input was helpful and most appreciated in spite of my bummed out attitude. Just sucks when you overhaul everything hoping for better performance and get a bunch of headaches. Anyway, thank you everyone!
```

---
## \#43 Posted by: TowerCrisis Posted at: 2018-12-03T10:56:18.643Z Reads: 43

```

[details="EDIT: Ignore me, I'm illiterate 😂"]
One other point I saw, you mentioned you did motor detection with tires on? That's a BIG no-no. Whenever you run detection the motors should be free-spinning with no load. It has the potential to give you funky readings under additional resistance
[/details]
```

---
## \#44 Posted by: Pedrodemio Posted at: 2018-12-03T11:05:23.979Z Reads: 42

```
Glad to hear that, happy riding 

You can increase the motor current but at small steps, ride for a few days as it is and see how hot the motors get, preferably with a thermometer, and then increase a bit the motor current see if the torque improves and how hot it get, there is a point that it will get hotter but no torque will be gained, also try to keep it under 60 °C

One thing you may need to change is battery min, at -3A will have almost no brake at high speed, but as I said, try it first, keep in mind that battery min dictates brake force at higher speed and motor min at lower speeds, even if you don’t use all the time it’s good to have really strong brakes for emergency situations
```

---
## \#45 Posted by: krazor Posted at: 2019-08-04T11:01:09.427Z Reads: 21

```
well at least you didint fry the vesc liek i didi haha glad this worked for you.
```

---
