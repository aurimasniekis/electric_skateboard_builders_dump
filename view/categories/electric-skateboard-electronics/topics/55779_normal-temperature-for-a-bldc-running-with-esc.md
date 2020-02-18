# Normal temperature for a BLDC running with ESC?

### Replies: 13 Views: 527

## \#1 Posted by: murloc992 Posted at: 2018-05-17T13:31:39.328Z Reads: 86

```
Hello Esk8 people!

Today I did a 10km ride and after it I found out (using my FLIR) my motor was at 90'C at the can(aimed at the sticker) and 115'C at the mount! :open_mouth:

I was wondering why would this happen and if it is safe..

My setup:

Turnigy Aerodrive SK3 5050 (or 5055) 280KV motor
HobbyKing 150A ESC
6S LiPo
18T gear on the motor
36T gear on the wheel

I weigh 100 kilos and rode on a VERY uneven, rumbly road/sidewalk maybe that contributed too..

Maybe I should change something inside the ESC, like timing, acceleration, etc?
```

---
## \#2 Posted by: Battosaii Posted at: 2018-05-17T13:38:45.052Z Reads: 81

```
That's way to hot  I think safe max temp is 80c 

Is that a single drive or dual drive?

If its single drive with that gearing and your weight its too much. What's your wheel size?
```

---
## \#3 Posted by: murloc992 Posted at: 2018-05-17T13:44:51.875Z Reads: 78

```
Today I used 100mm noname wheels, but previously I was using 75mm wheels and didn't seem to notice any problems. This heating is so spontaneous.. I rode 50km on the big ones and didn't see such heating. Maybe it came over time or something..
```

---
## \#4 Posted by: Battosaii Posted at: 2018-05-17T13:46:56.960Z Reads: 72

```
Those are big wheels I'd change the motor pulley to 16t you will lose a little top speed but will gain more torque and the motor will run more efficient and cooler.
```

---
## \#5 Posted by: murloc992 Posted at: 2018-05-17T13:49:07.374Z Reads: 72

```
Well, dropping two teeth doesn't sound like a problem to me as long as it makes it a bit cooler..

Maybe I should adjust ESC timing too, there's mentions about heat being generated between the settings. I am at the middle now which is balanced between temps and efficiency..
```

---
## \#6 Posted by: murloc992 Posted at: 2018-05-17T18:28:57.439Z Reads: 55

```
I put 15T gear on the motor and everything is working perfectly now. Everything you need sometimes is just 3 teeth less. :smiley:
```

---
## \#7 Posted by: professor_shartsis Posted at: 2018-05-17T19:05:56.526Z Reads: 52

```
[quote="murloc992, post:5, topic:55779"]
Maybe I should adjust ESC timing too, there’s mentions about heat being generated between the settings. I am at the middle now which is balanced between temps and efficiency…
[/quote]

one way to limit heating is to reduce the motor current limit setting. if you were to cut your motor current limit in half from the present value, your peak thrust and acceleration will be cut in half, but the rate of motor heating will be 1/4th and your top speed might possibly be unchanged depending on various other factors including your gearing and battery current limit.

40a motor limit vs 80a motor limit (0.1ohm motor)

40a * 40a * 0.1ohm = 160w ohmic motor heating

80a * 80a * 0.1ohm = 640w ohmic motor heating

^with 40a, acceleration is reduced to 1/2 but heating is reduced to 1/4, improving efficiency

in current control mode, half throttle with 80a limit is equivalent to full throttle with 40a limit.
```

---
## \#8 Posted by: murloc992 Posted at: 2018-05-17T19:10:51.720Z Reads: 45

```
So what you're basically saying I should pop the ESC "acceleration" setting to the lowest possible value which means that the motor will not be as "sharp" to accelerate, top speed will not change and the motor will run cooler? :slight_smile:
```

---
## \#9 Posted by: professor_shartsis Posted at: 2018-05-17T19:12:08.827Z Reads: 45

```
basically yes, and top speed *might* not be affected depending on your gearing and battery current limit.
```

---
## \#10 Posted by: murloc992 Posted at: 2018-05-17T19:25:23.985Z Reads: 42

```
I am using 2 3S 5000mAh 20C batteries in series as 6S so that gives me a questionable 200A peak. With a 150A ESC and a 60A motor I am not running into trouble. Right now I am having 15T/36T which is 2.4:1. It feels very smooth now even with acceleration being second from lowest. I will try to reconfigure it later down the road and see if it resolves it even more. As of now top speed recorded is 43km/h which feels way too much to be doing on a plank of wood on tiny wheels.. :slight_smile:
```

---
## \#11 Posted by: professor_shartsis Posted at: 2018-05-17T19:32:47.185Z Reads: 42

```
[quote="murloc992, post:10, topic:55779"]
As of now top speed recorded is 43km/h which feels way too much to be doing on a plank of wood on tiny wheels… :slight_smile:
[/quote]

If you are willing to sacrifice top speed for efficiency, you can try 3:1 or 4:1 gearing... both will give you more peak thrust, acceleration and efficiency for hill climbing without changing the settings (at the sacrifice of top speed). then lowering your “acceleration”/motor current settings on your esc will improve efficiency even further by reducing the rate of motor heating (at the sacrifice of the additional acceleration you gained by changing the gearing).
```

---
## \#12 Posted by: murloc992 Posted at: 2018-05-17T19:35:36.775Z Reads: 38

```
Without getting a huge gear for the wheels I don't think I can do it just yet. I was told that going below 14T is not really an option as it skips a lot and with my weight.. well I bet it would do that.. :slight_smile:

So probably I will aim at something like 18:54 or 15:45 later down the road. :slight_smile:
```

---
## \#13 Posted by: murloc992 Posted at: 2018-05-18T10:38:26.397Z Reads: 30

```
Did a short ride with a hill climb today, I could barely touch the motor and the ambient today is like 19'C with enough wind..

Is there a way to fix this without switching to dual motor?

Maybe some kind of makeshift "fan" which rotates on the end of the motor pulling the air out of it?
```

---
