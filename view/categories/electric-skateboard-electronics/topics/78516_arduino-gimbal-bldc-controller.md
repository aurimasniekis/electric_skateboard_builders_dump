# Arduino Gimbal BLDC controller

### Replies: 12 Views: 1114

## \#1 Posted by: Maxid Posted at: 2018-12-20T11:13:22.969Z Reads: 100

```
For a personal project I need to control a small BLDC motor for a maximum of one full rotation - so basically like the drone camera stabilization systems we all know.
For prototyping I'd like to use an Arduino or similar to quickly get this up and running.
My problem is that I don't know of the right controller for the motor, which should be super cheap (in the final "product" I will need to drive almost 100 of them simultaneously), can be weak (1A max should be plenty) but should be as quiet as possible (*cough* FOC?) and be precisely controllable via the Arduino.
Does anybody know of an Open Source project or some other chinese ESC that would give me what I am looking for? VESCs are obviously way overpowered and too expensive.
```

---
## \#2 Posted by: Maxid Posted at: 2018-12-26T10:42:20.560Z Reads: 72

```
Nobody?
@Deodand maybe?
```

---
## \#3 Posted by: ervinelin Posted at: 2018-12-26T10:45:01.800Z Reads: 70

```
People usually run stepper motors for something like this.. when you need precise control over the rotation...

Arduinos will easily be able to adapt to stepper motor controllers...

If it's a gimbal you are after then using dedicated gimbal controllers are better compared to arduino. You can program them as well to take a PWM signal to move around.
```

---
## \#4 Posted by: Maxid Posted at: 2018-12-26T10:56:06.982Z Reads: 62

```
Do you know of a cheap gimbal controller that takes pwm as input? I am not allowed to use stepper motors.
Positioning doesn't need to be super precise but I need to control the speed quite accurately
```

---
## \#5 Posted by: ervinelin Posted at: 2018-12-26T11:18:18.941Z Reads: 61

```
Google for Alexmos or Microstorm 32... I used the latter before but it's a bit of a pain to get going..
```

---
## \#6 Posted by: Jalapeno Posted at: 2018-12-26T11:36:58.259Z Reads: 59

```
https://odriverobotics.com
```

---
## \#7 Posted by: hexakopter Posted at: 2018-12-26T13:55:54.853Z Reads: 55

```
Sounds like you are searching for something like the DRV8313. Some brushless gimbal controllers are using this IC.
A great open hardware brushless gimbal project is this one: [http://www.olliw.eu/2013/storm32bgc/](http://www.olliw.eu/2013/storm32bgc/)
```

---
## \#8 Posted by: Der6FingerJo Posted at: 2018-12-26T14:11:01.867Z Reads: 50

```
I had a cheap ass gimbal ages ago and i think it ran basecam, which should be arduino compatible. 

https://www.ebay.de/itm/New-BGC-3-0-MOS-Gimbal-Controller-Driver-Two-axis-Brushless-Motor-OO/132223097646?hash=item1ec91c5b2e:g:KCgAAOSwGltawez5:rk:2:pf:0

https://www.ebay.de/itm/CNC-FPV-BGC-2-AXIS-BRUSHLESS-GIMBAL-CONTROLLER-FUR-GOPRO-3-KAMERA-DJI-SCHWARZEN/113377777529?hash=item1a65d79779:g:efkAAOSwZ8ZXCyhK:rk:1:pf:0

These are the things i had, the controller should have pwm input.
```

---
## \#9 Posted by: karma Posted at: 2018-12-26T14:42:12.466Z Reads: 42

```
I have 2 Odrives and they are amazing, however they are probably not what he needs. The Odrives are very precise with a good encoder and can handle peak currents up to 100A. A arduino on it's own will not be able to drive a BLDC motor, you will need some sort of power electronics. Since you are going to only do 1 rev, max 1A and probably want them to inexpensive I would recomend trinamic stepper drivers and a small stepper. Why can't you use steppers?
```

---
## \#10 Posted by: chuttney1 Posted at: 2018-12-27T01:52:23.230Z Reads: 32

```
The cheapest gimbal would be using either a servo motor or stepper motors.
```

---
## \#11 Posted by: J0ker3366 Posted at: 2018-12-27T05:39:13.229Z Reads: 22

```
Why not just fad a small housing for the go pro and a servo? Servo will give you full 360 rotation.
```

---
## \#12 Posted by: Maxid Posted at: 2018-12-27T10:01:25.955Z Reads: 13

```
It's not for a camera Gimbal - as I said this will have almost 100 motors in the end.

The stepper motors I found are more expensive than the BLDC Gimbal motors I can get my hands on.
```

---
