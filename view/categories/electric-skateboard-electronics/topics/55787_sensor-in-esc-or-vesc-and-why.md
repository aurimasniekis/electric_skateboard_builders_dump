# Sensor in ESC or VESC and why?

### Replies: 8 Views: 646

## \#1 Posted by: pedro Posted at: 2018-05-17T15:36:58.713Z Reads: 95

```
Hello, im reading in some post, Sensored motor is good for a start smooth .
And i read, if you have a VESC you can control for a start smooth.
For the last question, Sensored motor can connect in ESC or just in VESC.
```

---
## \#2 Posted by: Burrito Posted at: 2018-05-17T15:50:23.000Z Reads: 91

```
Both. Some esc have sensors too.
```

---
## \#3 Posted by: linsus Posted at: 2018-05-17T16:10:52.002Z Reads: 84

```
In order to control the motor you need to somehow know the position of stator and rotor in relation to eachother. If you're familiar with how a BLDC motor works then you'd know theres three phase wires "activating" different segments of the motor, creating a rotating magneticfield which makes the motor spin. 

If you dont know the position of the rotor before start its very hard for the ESC to know what to do next.
A hallsensor helps communicate that position. Creating a smoother startsequence. The VESC works without it but it attempts to move the rotor very Little in order to get feedback of said position. This is often experienced as a "stutter" by the user. You could just use your foot for startup and you wont experience the stutter.
```

---
## \#4 Posted by: pedro Posted at: 2018-05-17T16:33:06.968Z Reads: 71

```
ok, thank you. i will start with my foot :stuck_out_tongue:
```

---
## \#5 Posted by: Namasaki Posted at: 2018-05-17T17:12:02.606Z Reads: 58

```
I have never used sensors. 
Always foot start. 
Although foot start would not be practical on an EMTB
```

---
## \#6 Posted by: Slak Posted at: 2018-05-17T21:39:13.347Z Reads: 49

```
And even with sensored, "foot start" is good to save battery (less effort asked to battery compared to "stand still start"). Correct, @Namasaki ?
```

---
## \#7 Posted by: Namasaki Posted at: 2018-05-17T22:03:36.897Z Reads: 49

```
I believe that foot start is easier on the system in general.
```

---
## \#8 Posted by: rich Posted at: 2018-05-17T22:46:49.211Z Reads: 39

```
I love sensors in combination with FOC :heart_eyes:
It's not only about avoiding foot start, it means much better control at low speeds or e.g. you can roll backward and accelerate forward, also it's much smoother. From my experience sensors only work well in combination with FOC, in BLDC mode you have to foot start with sensors as well, very bad when you are strapped to a MTB :joy:

https://youtu.be/ptlHqK7kqCA?t=8s
```

---
