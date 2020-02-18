# Sensorless BLDC startup

### Replies: 5 Views: 186

## \#1 Posted by: vulkan66 Posted at: 2019-08-04T22:02:36.576Z Reads: 59

```
Hi, i am using this [motor](https://www.amainhobbies.com/dynamite-fuze-1-5-6pole-brushless-motor-800kv-dyns1665/p635507) and VESC 6. I have a problem with smooth startup of the motor and keeping low RPM (<1000). I use FOC and current control with own PID speed controller which works great in higher speeds (error +/-1%). I know that sensorless motors are are difficult to control at low speeds but the original ESC did the job pretty good and it managed to start from zero speed smoothly with load. 

My question is, if there might be other problem (for example motor parameters, current PID setting) or it is not possible to control this type of motor with VESC without problems. Can BLDC instead of FOC improve the behavior?

Thank you for your advice.
```

---
## \#2 Posted by: Dirt_Bag Posted at: 2019-08-04T22:52:57.637Z Reads: 54

```
You will never get a smooth start with that motor. It is 800kv and not at all torquey. You need something like a 6374 190kv at 8-12s voltage.


An 8s with 1-5 gearing i can get a smooth start in bldc sensorless with the 6374.

Your only good option for creating a decent board is to sell that motor and buy one the has a kv closer to 200.


Also, what battery voltage are you trying to run that thing on?
```

---
## \#3 Posted by: vulkan66 Posted at: 2019-08-05T06:20:13.416Z Reads: 37

```
It is not supposed to carry a human but approx. 15kg of load. It is powered by 2x4S, 6750mAh, 50C.
```

---
## \#4 Posted by: Dirt_Bag Posted at: 2019-08-07T06:41:13.105Z Reads: 22

```
Nothing about that will work. Its a miracle it has done anything useful at all. 

Build it with the right parts or you will end up with a pile of literal flaming garbage soon.
```

---
## \#5 Posted by: vulkan66 Posted at: 2019-08-07T08:16:52.228Z Reads: 20

```
What are you talking about? I told you that the motor was working great with different controller and with VESC it works very good as well so I don't think it's a miracle. Maybe you can explain a little bit why you think it's not a right part.
```

---
