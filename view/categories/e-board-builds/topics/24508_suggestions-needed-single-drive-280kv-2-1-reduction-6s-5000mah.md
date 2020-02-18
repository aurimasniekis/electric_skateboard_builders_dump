# Suggestions needed: Single Drive; 280Kv; 2:1 Reduction; 6S 5000mAh

### Replies: 10 Views: 647

## \#1 Posted by: BabaYaga Posted at: 2017-06-04T00:09:58.986Z Reads: 65

```
Hello all!
Here is my math for my board, I used the assumption of a 70-30 distribution (rear to front) along with the following assumptions and specs:
1) Rider + board weight = 80 kgs
2) Drag coefficient = 1.15 ( I assumed frontal area for aerodynamic drag to be a rectangle of my height as length and shoulder length as breadth)
3) Frontal area = 190 x 42 x pow(10, -4)
4) Rolling Resistance Coefficient = 0.015
5) Weight distribution between wheels on same truck is equal.

Following is a FBD of the system (rider + board) {add in drag force F_d and Grade force of 5 degree angle in direction of f_2 and also it is driver* not driven}:

<img src="/uploads/db1493/original/3X/f/4/f4546518d6056e0884058c1525ef61d454d22a77.JPG" width="375" height="500">
I assumed weight distribution on wheels on same truck is same, hence the frictional forces on front two wheels are the same. Note the directions of friction forces on all wheels except the driver wheel will be same and against direction of motion. This is anyway arbit but the important fact is they will be opposite in direction to the friction force on driver wheel.

In the centre of the below picture, I have drawn the FBD of one of the driven wheels on the front. Here, N' is just the interaction force between the truck and the wheel. Under the rolling resistance relation, we can find the frictional force acting on this wheel. Same procedure is used to find f_3. Which brings us to the bottom of the picture, which is again the FBD of the rider + board system. Since I want to find power consumption at constant speed, I necessarily need to have resultant acceleration as torque as zero. 
<img src="/uploads/db1493/original/3X/9/9/99485fdda6be0ed3f8588d98762314ea9595ca4f.JPG" width="375" height="500">
Applying the former and referring to the FBD, we find ourselves on the third picture:
<img src="/uploads/db1493/original/3X/b/9/b9620bfbed3df37feeeaed1e1fbe2044b4561a15.JPG" width="375" height="500">
Thus f_1 is equal 64N and using the latter condition, we can find torque (assuming that the torque due to the displaced normal will be small). With this torque I found the power required at the driver wheel, which turns out to be a whopping 2600W!

Where am I going wrong here? Also, I'll list my build parts down below, so if you could tell me where I can improve?

Build Parts:
1) Turnigy SK3 280Kv
2) HK RedBrick 70A ESC
3) 6S 5000mAh 20C ( was thinking of using 2 in parallel to get more range)
4) 72mm wheels
5) 2:1 gear ratio

The max current and voltage of the motor is 60A and 10S.

My goals are:
1) 30kmph top speed with a 20-25kmph cruising speed
2) 20km of range

I will be using my own PWM control.

Also, my wheel pulley is quite heavy as it is made out of steel. It weighs around 600gms, will that be a problem? Also, will the RedBrick ESC create problems? Other than stuff like, harsh start etc.
```

---
## \#2 Posted by: Jinra Posted at: 2017-06-04T00:14:05.365Z Reads: 51

```
You'll be lucky to get 10km on that build since the battery capacity is low and current draw will be through the roof. Consider reducing your gearing to 3:1 since your top speed goals are reasonably low anyway. I'd go for the 2 batteries in parallel to perhaps break 20km on flats. Personally, I'd go for a higher voltage and lower kv to be more efficient and produce less heat.
```

---
## \#3 Posted by: BabaYaga Posted at: 2017-06-04T00:16:38.835Z Reads: 52

```
Supposing I cannot change my motor, what should I do?
```

---
## \#4 Posted by: NickTheDude Posted at: 2017-06-04T00:19:29.389Z Reads: 52

```
I'd ditch the RedBrick and go for a x-car beast 150A.
```

---
## \#5 Posted by: BabaYaga Posted at: 2017-06-04T00:19:52.384Z Reads: 52

```
Reason being?
```

---
## \#6 Posted by: Jinra Posted at: 2017-06-04T00:21:15.959Z Reads: 50

```
More reduction like I said 3:1 should be good. Going dual motors would be better.
```

---
## \#7 Posted by: NickTheDude Posted at: 2017-06-04T00:21:45.473Z Reads: 50

```
70A at 6S is very little power. If you go parallel with the batteries then you could probably safely push 100A out of the pack and you'd need a higher amp ESC to handle it. 

Plus the x-car Beast has been used by a few people with good results.
```

---
## \#8 Posted by: BabaYaga Posted at: 2017-06-04T00:23:17.663Z Reads: 48

```
But the motor has a max load current of 60A??
```

---
## \#9 Posted by: NickTheDude Posted at: 2017-06-04T00:26:31.946Z Reads: 51

```
I'd imagine that the max burst amps for the motor are higher than 60A, while the Redbricks peak is 90A. Its also good to have some headroom.

Also, it seems like the redbrick is designed for helis so it won't have very effective brakes if any.
```

---
## \#10 Posted by: BabaYaga Posted at: 2017-06-04T00:27:46.672Z Reads: 51

```
alright thanks 
:)
```

---
