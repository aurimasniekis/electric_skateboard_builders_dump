# Low top speed of 35 km/h with my new 6374 3500 W 190 kv. 1

### Replies: 11 Views: 928

## \#1 Posted by: ElskerShadow Posted at: 2017-09-25T15:08:16.095Z Reads: 106

```
hey guys.

I had an enertion 6355 2400 W sensorless 190 kv motor that I just replaced by a 6374 3500 W 190 kv motor from eskating.eu and it's great since I have more torque on my single drive but with the enertion motor I had a top speed of 40 to 43 kmh and now even if the motor is bigger and more powerfull my MAXIMUM top speed is around 35 km h . 
Btw both motor were in FOC with the same settings at 60 A.
If ssomeone could help it would be great
<img src="/uploads/db1493/original/3X/2/b/2be06b773a790b65a14428ec3784976dd60b9512.PNG" width="281" height="500"><img src="/uploads/db1493/original/3X/a/f/afbb017af2454efd9526163ddbb3384651fe0a72.PNG" width="281" height="500">
```

---
## \#2 Posted by: Jinra Posted at: 2017-09-25T15:10:59.581Z Reads: 98

```
power =/= speed.

Run the motor while connected to BLDC tool and type "kv" in the terminal section, this will get you the real kv of your motor. You can compare this with your Enertion motor.

Also, did you make sure you redid detection on the new motor, and is it sensored or sensorless?
```

---
## \#3 Posted by: ElskerShadow Posted at: 2017-09-25T15:15:14.711Z Reads: 93

```
Thanks for the quick reaction. Actually i did not, I just went thru the three step of Foc mode but did not figure out how to use the sensors ( my new motor is sensored )
```

---
## \#4 Posted by: ElskerShadow Posted at: 2017-09-25T15:17:33.214Z Reads: 93

```
<img src="/uploads/db1493/original/3X/e/f/ef7b066dc8024ccb0bae73c599b14d3e6fb30b0a.PNG" width="281" height="500">
```

---
## \#5 Posted by: Jinra Posted at: 2017-09-25T15:18:09.376Z Reads: 88

```
You can keep it sensorless if you'd like. However, you need to redo detection for the new motor since it will likely have different properties.
```

---
## \#6 Posted by: ElskerShadow Posted at: 2017-09-25T15:20:20.446Z Reads: 91

```
Alright thanks mate ! Actualy I'd like to use the sensor since it's why I changed motor in the first place. Should I just run the motor detection on the BLDC configuration and then use Hall mode and run the three calculation parameters of FOC ?
```

---
## \#7 Posted by: Jinra Posted at: 2017-09-25T15:23:34.743Z Reads: 86

```
you dont have to do any detection in BLDC mode at all, just ran all the FOC detection parameters and apply. Then run the hall detection below and apply. Set the sensor mode to "hall" and declare a sensorless erpm or leave it at its default value.
```

---
## \#8 Posted by: ElskerShadow Posted at: 2017-09-25T15:40:14.980Z Reads: 79

```
Did what you said all seems to work fine. Thank you very much I did the Kv calculation and it is 1188.66 rpm/Volt but I don't know what it means.
```

---
## \#9 Posted by: Jinra Posted at: 2017-09-25T15:42:55.546Z Reads: 76

```
it gives you the eRPM per volt for which you divide by 7 (for your motor) which gives you 169kv on that motor.
```

---
## \#10 Posted by: ElskerShadow Posted at: 2017-09-25T15:45:50.489Z Reads: 76

```
Good to know ! So this explain the lower top speed maybe ? 
Something weird happens. When I turn off the remote the motor starts to spin on its own.
```

---
## \#11 Posted by: Jinra Posted at: 2017-09-25T15:46:32.813Z Reads: 76

```
What remote? Sounds like you need to set the failsafe on it.
```

---
