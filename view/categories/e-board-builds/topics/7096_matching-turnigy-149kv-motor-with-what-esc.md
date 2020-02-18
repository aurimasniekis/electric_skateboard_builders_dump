# Matching Turnigy 149kv Motor with what ESC?

### Replies: 14 Views: 2314

## \#1 Posted by: abaddon6w Posted at: 2016-08-04T00:52:23.090Z Reads: 159

```
What's going on all. 

Started building this thing a couple of days ago and everything seems to be going pretty smooth. Here's my circuit. (2) [3S 11.1v 5000mah Turnigy Lipo's](http://www.hobbyking.com/hobbyking/store/__9184__Turnigy_5000mAh_3S_20C_Lipo_Pack.html) in series to [Hobbyking 85A BlueSeries ESC](http://www.hobbyking.com/hobbyking/store/__24719__HobbyKing_85A_BlueSeries_Brushless_Speed_Controller.html). The ESC Hooks up to an arduino which takes inputs from a Nyko Kama. The ESC also hooks up to the [Turnigy SK3 149kv motor](http://www.hobbyking.com/hobbyking/store/__18184__Turnigy_Aerodrive_SK3_6374_149kv_Brushless_Outrunner_Motor.html).

When I run the motor without a load the motor runs as expected. When I run it with a small load, sometimes just connecting the belt to the wheel pulley the motor runs very slow. I believe it could be something to do with the low voltage protection of the ESC. I have changed the setting of the ESC's low voltage protection threshold to Low 3.0v/50%, which is the lowest possible setting. Can't turn it off. 

I was wondering if anyone has experienced this problem or can give me some kind of direction moving forward.I know others that have achieved a sustainable build using the 149kv motor and (2x) 3S 11.1V lipos. I believe they used different ESC's. Such as this build [here](http://www.electric-skateboard.builders/t/400-build-ebay-deck-sk3-149kv-20-28t-6s-lipo-150a-car-esc/4386). 

Thanks in advance!
```

---
## \#2 Posted by: willpark16 Posted at: 2016-08-04T03:23:52.438Z Reads: 147

```
in series or parrallel
```

---
## \#3 Posted by: abaddon6w Posted at: 2016-08-04T04:07:02.853Z Reads: 137

```
2 lipos are connected in series so they should be acting as a 6S 22.2V 5000mah battery
```

---
## \#4 Posted by: Maxid Posted at: 2016-08-04T04:37:07.332Z Reads: 128

```
That ESC will not work - you can not use its brake functionality. It is only capable of a 100℅ instantaneous brake which will make riding a pain and dangerous.

Why do people keep buying these plane ESCs? This is the third time in a couple days that I have to tell someone they f*cked up by ordering the wrong stuff.
```

---
## \#5 Posted by: Michaelinvegas Posted at: 2016-08-04T04:38:30.325Z Reads: 136

```
http://calc.esk8.it

Based on your set up and guessing the gearing ...you must be going pretty slow topping out around 12 mph 

Not sure what esc that is for...I'm gonna assume for a helicopter ... Does it have a break? 

To get the benefit of that motor you will need to increase the voltage to at least 10s....or to get a different motor with a higher kv
```

---
## \#6 Posted by: Michaelinvegas Posted at: 2016-08-04T04:42:42.815Z Reads: 134

```
[quote="evoheyax, post:1, topic:2983"]
Electronic Speed Controllers


VESC 50a 12s
DIY's 120a 12s
FVT 120a  6s
FVT 180a  6s
Psycotiller's The Sleeping Lion "Winchester" 120a 12s
Castle Mamba Monster2 6s
Castle XL2 8s
Hobywing EzRun MAX8 6s
Hobywing EzRun MAX5 200a 8s
Hobywing EzRun MAX6 160a 8s
Hobbywing XeRun XR8 Plus 6s
[/quote]

See this thread 

http://www.electric-skateboard.builders/t/new-builder-list-of-known-and-commonly-used-parts/2983?u=michaelinvegas
```

---
## \#7 Posted by: Maxid Posted at: 2016-08-04T04:58:07.336Z Reads: 113

```
[quote="Michaelinvegas, post:5, topic:7096, full:true"]
To get the benefit of that motor you will need to increase the voltage to at least 10s....or to get a different motor with a higher kv
[/quote]

Well that is not completely true: I have the same setup and what is crucial is the gearing. 20/28 will get you ~25mph!
```

---
## \#8 Posted by: NNGG Posted at: 2016-08-04T04:59:45.556Z Reads: 105

```
You can use the yep esc. $99 plus a programming card that has 12s capability. Brake is programmable, but your right the blue series is all or nothing
```

---
## \#9 Posted by: Michaelinvegas Posted at: 2016-08-04T06:21:16.708Z Reads: 109

```
[quote="Maxid, post:7, topic:7096"]
What is crucial is the gearing. 20/28 will get you ~25mph!
[/quote]



True....  

[quote="Michaelinvegas, post:5, topic:7096"]
Based on your set up and guessing the gearing
[/quote]



But please read the whole thing
```

---
## \#10 Posted by: abaddon6w Posted at: 2016-08-04T14:28:55.057Z Reads: 95

```
Thanks for the replies everyone. I have ordered the Hobbywing EZRUN MAX8 and i'll see how that goes. Based on the feedback seems like the Blueseries was the problem. I will be gearing to 20/28 20+mph top speed. Thanks for all your help and I will update you when I'm done!

I guess the reason I bought the Blueseries was because I was just looking for the cheapest 80A 6S speed controller that hobbyking carried. Unfortunately they dont do a great job of distinguishing plane speed controllers from car speed controllers. I just thought one speed controller is the same as any other except for the amps and volts it can take. I have zero experience in anything hobby related. I'm a noob. I'll update you guys when I'm done and thanks again.

Also can someone please explain the difference between a plane and a car controllers?
```

---
## \#11 Posted by: mccloed Posted at: 2016-08-04T15:41:05.416Z Reads: 88

```
Plane/Helicopter ESC's usually do not have brakes or are very limited on the adjustment of the brakes. Car ESC's will have proper braking and and the brakes will have more adjust-ability. Make sure you get a programmer for your Car ESC. The stock settings are usually not ideal and will most likely be set with reverse.
```

---
## \#12 Posted by: SimosMCmuffin Posted at: 2016-08-04T15:53:48.921Z Reads: 86

```
The biggest difference in plane/heli and car ESCs are the throttle profiles.

In a plane when you have the ESC for the prop motor. The throttle profile goes from 0% to 100% and at 0% if you have braking enabled it will start fully braking the motor. and the throttle doesn't go to -100%, because in traditional planes you only want the motor to turn in one direction and you control how fast it spins in that particular direction.

Car ESCs' throttle profile goes from -100% to 100%. The physical controller has the throttle trigger is neutral in the middle position at 0%.
When **pulled** (the trigger direction can be changed), the throttle will move towards the 100% positive end and the ESC will spin the motor in the "forward" direction.
When **pushed** the throttle will go towards the -100% negative side and the ESC knows that reverse or braking is wanted depending if the car is moving or stationary.

TLDR: Plane and heli motors spin only in one direction (forward) and Car motors can spin in both directions (forward and reverse) and therefore have better braking profile.
```

---
## \#13 Posted by: abaddon6w Posted at: 2016-08-04T16:48:46.366Z Reads: 79

```
Hey man thanks for the great response. I'm starting to understand it more.
```

---
## \#14 Posted by: abaddon6w Posted at: 2016-08-09T14:37:49.721Z Reads: 67

```
So I went with the Hobbywing MAX8 150A and all those BlueSeries problems are gone, unfortunately new problems have cropped up. When I try to go up hill the system seems to reset itself. Not sure what could be causing this problem. I find that when I give the board a good couple of kicks it can usually get up the hills just fine. It could be related to settings on my MAX8 or maybe the gear ratio that I have the board at right now (2.86 : 1). What are some common settings I should be setting my ESC to and do you guys thing the gear ratio could be the problem?
```

---
