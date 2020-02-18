# How to program vesc for sensored motors?

### Replies: 5 Views: 1585

## \#1 Posted by: Conor Posted at: 2017-08-14T18:54:50.159Z Reads: 177

```
I just want to get it right.
I had a sensorless motor and now upgraded to sensored motors and I just want to know what all needs to be changed😀
```

---
## \#2 Posted by: rich Posted at: 2017-08-14T19:25:23.747Z Reads: 175

```
Basically just a new motor detection and see if there is a hall table detected or not. Then select hybrid.
But BLDC mode is not best for sensored motors. FOC is much better.

Which vescs do you have (manufacture, version) and which motors (kv)?
```

---
## \#3 Posted by: Conor Posted at: 2017-08-14T21:09:06.102Z Reads: 166

```
I have a  vesc 4.12 and eskating.eu 190kv 6355 motors
```

---
## \#4 Posted by: Conor Posted at: 2017-08-14T22:43:27.752Z Reads: 162

```
So I did a detection and it detected the hall sensors I hit apply. and Now do I put the mode in Sensored or hybrid?
```

---
## \#5 Posted by: rich Posted at: 2017-08-15T09:25:58.943Z Reads: 143

```
Just to get sure, if the detection failed the text is "hall sensor table detection failed:" (I didn't realize that the first time because there is still a hall table visible but with wrong values).
When everything is good the text is "detected hall sensor table:".

Hybrid mode means that the sensored mode is active at low speed only, after hitting the erpm limit the motor switches to unsensored mode where the motor performs better at higher speed. You can change the settings, it's "Sensorless ERPM (hybrid mode) in the BLDC tab beside the hall table but the default setting should work flawlessly. In sensored mode the motor always stays in this mode but hybrid is better because sensors are great at low speed but not necessary at higher speed.

I don't know the quality of the DIY vesc, maybe it's better to stay in BLDC mode. But I realized that the startup from standstill is butter smooth in FOC while in BLDC mode there is cogging and jittering at startup. Maybe you get different results than me (I hope so). The sensors are still geat at low speed compared to unsensored mode. Just to mention, I have 6 vescs and only 2 of them can do FOC.

If your new motor is rated with the same Ampere as your previous one you can keep your remaining settings in BLDC tool (if you did that already).
```

---
