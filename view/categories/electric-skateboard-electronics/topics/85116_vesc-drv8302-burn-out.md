# Vesc DRV8302 burn out

### Replies: 10 Views: 279

## \#1 Posted by: Felixxx Posted at: 2019-02-23T09:51:52.676Z Reads: 83

```
Hi,

today I rebuild my esk8. I made new deck and battery case. But when I put all together I tested motor. It was working until I push throttle to max and after I pres brake my DRV8302 on vesc burn out. Can anyone tell me why this hapend? I was using this setup last year and it works like it shuld. And I dont want to this hapen to nev vesc so I need solution why this goes up smoke.
Vesc in warenty from hobbyking. I hope they will replace it.
```

---
## \#2 Posted by: Andy87 Posted at: 2019-02-23T10:17:17.824Z Reads: 81

```
Make sure you don’t have a short in your phase wires of your motor.
Maybe your mounting screws are too long and damaged the isolation.

Which motor and battery you have?
If you have 12s battery and motors with 200+kV you could hit the max erpm limit on your vesc.

There are different things that could have caused that. It’s just a guess here.
```

---
## \#3 Posted by: Felixxx Posted at: 2019-02-23T10:24:49.643Z Reads: 77

```
I dont have any short in motor wires for shure. 
Setup is 12s lipo and 230kv motor.
Is it possible that the reason is becuse I spin it to max and hit thr brake?
And one more thing, I have BLDC enabled from the begining. With this setup with no cheanges I made around 400-500km with no problem, but top speed under 30kmh. Over 30 is tooo much for me :slight_smile:
```

---
## \#4 Posted by: mishrasubhransu Posted at: 2019-02-23T10:37:59.008Z Reads: 70

```
So, when you are braking at max speed, the motor produces a large voltage spike(back emf+inductive spiking). This is used in regenerative braking to charge the battery. At max speed with full brake produces a large voltage spike that the DRV can't tolerate. I hope I made it is easy enough to understand, but there is lot more to it.
```

---
## \#5 Posted by: Felixxx Posted at: 2019-02-23T10:40:27.053Z Reads: 69

```
Ok. Tnx.
Can this hepen when I drive and hit the brake? What I have to do to prevent this?

And this is new custum made board
![20190220_115924|690x388](upload://yHy0AsG4bPBQiCKGpl4jYE3Fzmm.jpeg) ![20190220_115945|281x500](upload://bWtx6EZYcc5VssfzNS6AWD6eOuh.jpeg)
```

---
## \#6 Posted by: Andy87 Posted at: 2019-02-23T10:49:09.888Z Reads: 63

```
[quote="Felixxx, post:3, topic:85116"]
Setup is 12s lipo and 230kv motor
[/quote]

And it happened with full charged batteries on the bench?
Than this is your problem 100%.
This hw4.12 vesc can’t handle more than 60 000erpm
```

---
## \#7 Posted by: Felixxx Posted at: 2019-02-23T10:50:46.140Z Reads: 64

```
Yes batteries at 87% on the bench, just motor not even belt on wheel.
```

---
## \#8 Posted by: Andy87 Posted at: 2019-02-23T10:56:32.202Z Reads: 64

```
https://calc.3dservisas.eu/?Pc_NDsIgEATgd-FsDBSoP1fa9KQhMbF35VATSUl6NL67O0Pr7dthGcJHPcKkzur9KrPayXCVwe4P4iXcxMaSUeiogAWtNYcOk_HV2Glqzk4jLOhoAWz6eq9EpA0VN7HKehJhS_6LnhPPqV501OQd1x2cw9qUWW6ZxRnXHYkf1PdzYIzlNC7CE9I0XNa30jBu6uvp9wc=

Use this calculator to get your max erpm.
Get a focbox or vesc 6 if you want to run a setup which get higher than 60000erpm and this will not happen anymore
```

---
## \#9 Posted by: Sn4pz Posted at: 2019-02-23T11:24:57.994Z Reads: 54

```
You should get a 150kv motor and have a nice blend of torque and speed

I'm guessing your ratio is smth like 16/ 36 or 38
```

---
## \#10 Posted by: Felixxx Posted at: 2019-06-06T18:32:48.206Z Reads: 24

```
I have new vesc v4.12 with firmware 2.81 from hobbyking.
One question. On previous vesc which I burnd I use foc. Now I dont want to burn this one too. So my question is should I use foc or bldc on this vesc?
```

---
