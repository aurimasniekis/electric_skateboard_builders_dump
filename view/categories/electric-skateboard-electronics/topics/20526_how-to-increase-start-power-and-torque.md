# How to increase start power and torque

### Replies: 12 Views: 2623

## \#1 Posted by: emipop Posted at: 2017-04-07T14:29:49.992Z Reads: 276

```
Hello, I have receive great info on this forum. I also have a question about VESC: I have received an advice to change the timing and start power for the VESC/motors. I want to change the start amperage to get more torque when I start the motors. How do I make this settings using BLDC Tool.
My application is a robot and I`m using Alien Power 6364 with latest version of VESC.
```

---
## \#2 Posted by: JLabs Posted at: 2017-04-07T14:47:13.624Z Reads: 271

```
Post your VESC settings so some experts can take a look *coughs @Blasto

Also what's ur battery setup?
```

---
## \#3 Posted by: Blasto Posted at: 2017-04-07T15:03:43.292Z Reads: 263

```
also a better explanation of your application.

for robotics I would use sensored motors in FOC, duty cycle control.

https://www.electric-skateboard.builders/t/midori-esk8-inspired-sumo-robot/1220

I did another one 1800kv motors, but guess i got lazy and did not do a build thread... oh well will never happen haha
```

---
## \#4 Posted by: Hummie Posted at: 2017-04-07T15:33:21.572Z Reads: 246

```
 @blasto @PXSS   
why isn't 160 motor amps ok?  is it purely because it's hard to handle or is there an electrical reason?
```

---
## \#5 Posted by: emipop Posted at: 2017-04-07T15:45:32.666Z Reads: 236

```
6S is the battery config.

The motors are already bought and unfortunattly they are sensorless.

Our main issue now is that he motors are jittering and nundgeing when the robot is loaded with higher wheight.
```

---
## \#6 Posted by: Hummie Posted at: 2017-04-07T16:00:34.947Z Reads: 228

```
What are ur motor amps set at now?
```

---
## \#7 Posted by: Blasto Posted at: 2017-04-07T16:02:07.593Z Reads: 225

```
Sensored motors is the way to go for robotics... you can always play with your startup boost... (in the advance tab in the bldc tool)

What is the application?
```

---
## \#8 Posted by: Hummie Posted at: 2017-04-07T16:24:20.485Z Reads: 211

```
An obvious way to get more power/torque at start up is to increase the motor amps, maybe not to 160 for all applications but something higher than what it's at is worth a shot if the load is high
```

---
## \#9 Posted by: emipop Posted at: 2017-04-07T17:29:45.655Z Reads: 207

```
Ordering sensorless was a mistake.

The stratup boost is set at 0.09 now.

I am unable to find the amp set now in BLDC Tool. Can you instruct me please?

Apliaction is a wieght transportation robot (300kg) in a production facility. 1:25 reduction gearbox. Chain drive. Wheels&tires.
```

---
## \#10 Posted by: Hummie Posted at: 2017-04-07T17:46:28.129Z Reads: 197

```
I forget but motor configuration tab maybe.  Look for the battery and amp limits and see what they're at.  You've got a 1:25 gear ratio you say ..to confirm you're saying the motor will spin one time for 25 revolutions, of something an you have a lot of mechaical advantage?
```

---
## \#11 Posted by: Eboosted Posted at: 2017-04-08T02:36:42.512Z Reads: 170

```
Raise this value in 0.01 increments, default is 0.010

<img src="/uploads/db1493/original/3X/9/7/97de20e869914092a1e25ff271bd7f7f6f1f4e01.png" width="690" height="387">
```

---
## \#12 Posted by: emipop Posted at: 2017-04-08T05:18:01.323Z Reads: 157

```
@Eboosted
 my value is now 0.09 which i understood from the tutorial that is max.
can I go over it? what is the max value you used?



@Hummie
 the reduction gearbox is actually 25:1.  so for 25 motor spins i get 1 wheel spin.
```

---
