# First Build, An All Uphill Beast

### Replies: 21 Views: 1641

## \#1 Posted by: Skifree Posted at: 2017-10-04T19:47:07.748Z Reads: 196

```
Hey all, I would like to build a board for just going uphill. I've been working with BLDC's for a while, but only for quadcopters, so this is a whole new world for me.
I will be manufacturing most of what I can, but am having a hard time wrapping my head around what motor size I need. I'd like to climb 20 degree inclines constantly, and 30 degree now and then. My hope is that if I choose the correct motors and vesc's, I will not have to worry about overheating anything.
My budget isn't really a concern as I have been saving for this project for a while now. That being said, hopefully it doesn't go over $2000.

All uphill, about 20° sometimes 30° on a dirt logging road
8km (5m) range or more if it just means adding more batteries.
Air temperature tends to be between 20°c to 30°c (70f to 85f)
I'm about 220lbs all in with my backpack
25kph (15mph) top speed would be fine

I would like to keep it to two wheel drive for simplicity, but I don't know if that's realistic.

One of the parts that I find difficult to understand is using a higher kv motor for better uphill. I've read that some are suggesting 240kv instead of a lover 150kv.

Thanks for any and all help!
```

---
## \#2 Posted by: cwazy1 Posted at: 2017-10-04T19:49:59.841Z Reads: 196

```
those are some serious requirements. You'd be best to use a high current ESC or a VESC6 for your application to avoid literally exploding chips in your speed controller. 

The lower the motor KV the more torque its going to have. But it is all relevant depending on your battery voltage. If you're running 8s, then 240kv would be okay. But if you're running a 12s, which is what I would recommend for your application, you'd definitely want 150kv motor.
```

---
## \#3 Posted by: Skifree Posted at: 2017-10-04T20:04:57.627Z Reads: 183

```
That sounds alright, I've been reading that most builders are really happy with the VESC6, so I will definitely commit to that.
The VESC6 specs say I could run it at continous 80 Amps, and the motor that I would probably get is the SK3 - 6374 and it states that it has a max load of 70 Amps. Does that mean that I would never have to worry about overheating the VESC? And only the motor would be put at risk if I pushed it?
```

---
## \#4 Posted by: cwazy1 Posted at: 2017-10-04T20:10:14.616Z Reads: 165

```
VESC6 is rated to 80A from battery. If you're running lipo's you can easily go over 80A discharge. A 4000mAh 3s Lipo with a 20c rating by itself has a max discharge of 80A. Now throw a few of those in parallel and series and you can go over the 80A. Thats where people run into issues with these eMTBs. You want to be able to discharge as much as you can without blowing your VESC. This is where configuring your parameters in VESC tool is important. You need to stay as low as you can while still reaching your desired requirements of hill climb and top speed.
```

---
## \#6 Posted by: cwazy1 Posted at: 2017-10-04T20:13:22.209Z Reads: 147

```
Please don't listen to half the stuff this guy is saying. I know you mean well, but honestly your suggestions are totally out of whack for a serious emtb build.
```

---
## \#7 Posted by: Sn4pz Posted at: 2017-10-04T20:14:52.105Z Reads: 141

```
didnt realise it was an emtb build...sorry :confused:
deleting it now
```

---
## \#8 Posted by: cwazy1 Posted at: 2017-10-04T20:15:40.523Z Reads: 139

```
It was good advice for a street build! Sorry if I sounded harsh.
```

---
## \#9 Posted by: Sn4pz Posted at: 2017-10-04T20:16:26.609Z Reads: 144

```
meh

its all good :slight_smile:
you know better than i do when it comes to mountain boards
```

---
## \#10 Posted by: deucesdown Posted at: 2017-10-04T20:16:58.183Z Reads: 153

```
https://www.electric-skateboard.builders/t/a-theory-on-hill-climbing-massive-lipos-dual-6374-and-the-c-word/34437
```

---
## \#11 Posted by: Skifree Posted at: 2017-10-04T20:20:15.756Z Reads: 151

```
[quote="cwazy1, post:4, topic:34781, full:true"]
VESC6 is rated to 80A from battery. If you're running lipo's you can easily go over 80A discharge. A 4000mAh 3s Lipo with a 20c rating by itself has a max discharge of 80A. Now throw a few of those in parallel and series and you can go over the 80A. Thats where people run into issues with these eMTBs. You want to be able to discharge as much as you can without blowing your VESC. This is where configuring your parameters in VESC tool is important. You need to stay as low as you can while still reaching your desired requirements of hill climb and top speed.
[/quote]

Okay, so I can configure the VESC using the VESC tool to only use the maximum current that will keep it cool enough to keep me going? 
And with that in mind the last part of the puzzle is for me to figure out the best ratio of gearing I am assuming?
```

---
## \#12 Posted by: BigBoyToys Posted at: 2017-10-04T20:29:51.350Z Reads: 132

```
Dual vesc 6, 6374 sensored motors and a solid battery will climb 20 percent grades if you have it geared to 15mph but not sure for how long without some time to cool. The vesc 6 is capable of backing off power if the vesc or the motors start to overheat. If the hills are miles long you will probably still hit the soft back off. For comparision,  I can get about a 1/8 mile on a 20 degree hill before my ollins vescs back off. Im 300lbs loaded up on the board and i run sealed 170kv 6364 motors, the board is geared for 25mph.
```

---
## \#13 Posted by: aigenic Posted at: 2017-10-04T20:32:15.989Z Reads: 136

```
20° hill is seriously steep hill, I dont know any that would be 30° :O Where do you live? [This](http://calc.esk8.today/) might help with your calculations...IDK your weight, but dual 6374 should be enough :) Maybe even 6354 but it depends on your desired max speed, gear ratio and other specs...

Lower KV means higher torque, higher KV means higher top speed...
```

---
## \#14 Posted by: deucesdown Posted at: 2017-10-04T20:36:33.707Z Reads: 138

```
Okay, this is all theory no practical experience, but from reading here a bunch...

- power/heat bottlenecks can be at wheel radius, pulleys/belts, motor, esc, battery.
- for vesc4, 12s is highest practical voltage (10s is safer), 50-60a from battery.
- you can size your battery to comfortably deliver 60a to each motor
- 6374 is biggest practical motor, and in hill climb, can overheat vesc.
- from what I've read, it's most likely the vesc that will be the power bottleneck for continuous hillclimb
- 12s will let motors pull more amps than 10s (more power, but hotter everywhere)
- what gearing you need will probably come down to experimentation
- motor kv is like gearing. all else being equal, you should match it to your battery voltage. But low kv is like more torque less speed. There's a lot of nuance here.
- using eskate calculator, try out the highest gearing you can get parts for (including wheel size), and check top speed. If too slow, change gearing.
- you can add active cooling (fans, heatsinks, airflow to outside) to help vesc cool off

@aigenic  20% is very different from 20deg
```

---
## \#15 Posted by: Skifree Posted at: 2017-10-04T20:38:56.929Z Reads: 126

```
[quote="BigBoyToys, post:12, topic:34781, full:true"]
Dual vesc 6, 6374 sensored motors and a solid battery will climb 20 percent grades if you have it geared to 15mph but not sure for how long without some time to cool. The vesc 6 is capable of backing off power if the vesc or the motors start to overheat. If the hills are miles long you will probably still hit the soft back off. For comparision,  I can get about a 1/8 mile on a 20 degree hill before my ollins vescs back off. Im 300lbs loaded up on the board and i run sealed 170kv 6364 motors, the board is geared for 25mph.
[/quote]


That definitely helps, I won't need to go fast at all, I will sacrifice speed for torque completely, I just need to find the balance point to get all the speed that is available to ensure I won't have any troubles climbing. 
I should point out the hill I am going up is actually a mountain, and the distance is 5km.
where do you find sensored motors? I find hobby king has most of what I need for quads, but haven't needed sensored motors till now.
```

---
## \#16 Posted by: Skifree Posted at: 2017-10-04T20:41:07.975Z Reads: 127

```
[quote="aigenic, post:13, topic:34781"]
20° hill is seriously steep hill, I dont know any that would be 30° :open_mouth: Where do you live? This might help with your calculations...IDK your weight, but dual 6374 should be enough :slight_smile: Maybe even 6354 but it depends on your desired max speed, gear ratio and other specs...
[/quote]

It's actually a mountain that I would like to climb, I want to be able to paraglide off the top without doing any hiking.

I am willing to sacrifice speed to not have to stop for any amount of cool down. If that's an option....



[quote="deucesdown, post:14, topic:34781, full:true"]
Okay, this is all theory no practical experience, but from reading here a bunch...


power/heat bottlenecks can be at wheel radius, pulleys/belts, motor, esc, battery.
for vesc4, 12s is highest practical voltage (10s is safer), 50-60a from battery.
you can size your battery to comfortably deliver 60a to each motor
6374 is biggest practical motor, and in hill climb, can overheat vesc.
from what I've read, it's most likely the vesc that will be the power bottleneck for continuous hillclimb
12s will let motors pull more amps than 10s (more power, but hotter everywhere)
what gearing you need will probably come down to experimentation
motor kv is like gearing. all else being equal, you should match it to your battery voltage. But low kv is like more torque less speed. There's a lot of nuance here.
using eskate calculator, try out the highest gearing you can get parts for (including wheel size), and check top speed. If too slow, change gearing.
you can add active cooling (fans, heatsinks, airflow to outside) to help vesc cool off


@aigenic  20% is very different from 20deg
[/quote]

Thanks, all good points.  I should point out that I think I made a mistake in saying the hill is 20', I just looked at a chart and 20' looks intense, I think I meant to say 20% grade. It is an old logging road, it's pretty steep but trucks can go up without much problem.
I'm planning to build a watertight case out of milled aluminum and hope to use it as the heat sink for the VESC6. hopefully that is all the cooling that I would need.
```

---
## \#17 Posted by: BigBoyToys Posted at: 2017-10-04T20:59:32.169Z Reads: 107

```
You gonna para glide down with your emtb on your back? Lol

I think this motor would be a good fit for your application. Its a bit longer at 6384, 130KV and includes an intergrated thermister on the hall sensor board so that the VESC can monitor your motor temperature.
```

---
## \#18 Posted by: Skifree Posted at: 2017-10-04T21:25:08.503Z Reads: 110

```
[quote="BigBoyToys, post:17, topic:34781, full:true"]
You gonna para glide down with your emtb on your back? Lol

I think this motor would be a good fit for your application. Its a bit longer at 6384, 130KV and includes an intergrated thermister on the hall sensor board so that the VESC can monitor your motor temperature.
[/quote]


Absolutely! I might just leave it strapped to my feet!

Who makes that motor?
```

---
## \#19 Posted by: pat.speed Posted at: 2017-10-04T22:23:04.896Z Reads: 105

```
My guess is alien power systems they have great products. I would also recommend double idler pulleys if you are using belts. For motors try and keep the kv under 140kv and the Vesc 6 is your best bet for this sort of build. As for batteries go with 12s lipos. 10000mah minimum and 60c
```

---
## \#20 Posted by: BigBoyToys Posted at: 2017-10-04T22:44:11.540Z Reads: 105

```
That is awesome please send video of that! I feel like 30lbs hanging from your ankles wouldnt be very comfortable. Yeah the motors are made by Alien power Systems and ship from EU.
```

---
## \#21 Posted by: MysticalDork Posted at: 2017-10-04T22:59:52.663Z Reads: 101

```
For sustained load like this, I'd recommend getting some sort of impeller to attach to the motors to force airflow for cooling. Most RC derived motors are rated while they are in the prop wash of the airplane they're powering, which helps a lot with overheating. Adding some sort of fan to the back of the motor to suck air through the stators and keep things cool will improve the thermal endurance of them by quite a bit.
```

---
## \#22 Posted by: Skifree Posted at: 2017-10-06T03:36:50.392Z Reads: 90

```
[quote="MysticalDork, post:21, topic:34781, full:true"]
For sustained load like this, I'd recommend getting some sort of impeller to attach to the motors to force airflow for cooling. Most RC derived motors are rated while they are in the prop wash of the airplane they're powering, which helps a lot with overheating. Adding some sort of fan to the back of the motor to suck air through the stators and keep things cool will improve the thermal endurance of them by quite a bit.
[/quote]

That's a good idea, I could probably machine something to attach to the back of the motor, thanks!

[quote="BigBoyToys, post:20, topic:34781, full:true"]
That is awesome please send video of that! I feel like 30lbs hanging from your ankles wouldnt be very comfortable. Yeah the motors are made by Alien power Systems and ship from EU.
[/quote]

You got it! The vid will at the least get me a few laughs!


I ordered a board from Trampa, and the motors from Alien, thanks to everybody for the help! I will surely have more questions soon!
```

---
