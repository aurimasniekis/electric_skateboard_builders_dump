# Gear ratio - explained

### Replies: 6 Views: 2906

## \#1 Posted by: Tycho Posted at: 2017-07-16T09:00:45.809Z Reads: 333

```
Have I understood the concept of "gear ratio" for an electric skateboard senario correctly when I say:

A gear ratio of 2:1 means (motor turns:wheel turns)

As in every time the motor has made 2 turns, the wheel has made 1 turn.

?
```

---
## \#2 Posted by: MontPierre Posted at: 2017-07-16T09:13:09.555Z Reads: 332

```
I think that's right... 

Here is great calculator which will help you play with gear ratio ( number of teeth of each gear) given your battery and motor specs to achieve desired speed ( all approx depending on weight of rider and etc)

http://toddy616.blogspot.co.uk/2013/07/electric-skateboard-calculator.html?m=1
```

---
## \#3 Posted by: Cobber Posted at: 2017-07-16T09:15:30.100Z Reads: 316

```
expecting that your topic will become a resource for future new members X.X is better than X,X...
```

---
## \#4 Posted by: karma Posted at: 2017-07-16T10:17:44.852Z Reads: 289

```
https://www.youtube.com/watch?v=49DxlXs8tyk
```

---
## \#5 Posted by: wafflejock Posted at: 2017-07-18T00:40:41.221Z Reads: 225

```
Yes this is the typical kind of setup and somewhere between 2-4 is where your ratio will land in this case which means a 2-4 times reduction in speed between the motor pulley RPM and the wheel pulley RPM and a 2-4 times increase in torque (turning force) for the speed trade off.  (Overcoming) Torque at a given RPM => power.

http://curriculum.vexrobotics.com/curriculum/mechanical-power-transmission/gear-ratios
```

---
## \#6 Posted by: trampa Posted at: 2017-07-18T07:20:42.849Z Reads: 203

```
Always good to read:

http://vedder.se/2014/10/chosing-the-right-bldc-motor-and-battery-setup-for-an-electric-skateboard/

Basically you want to gear down as much as possible and run your motor at higher RPM and lower torque.
This is the only way to keep the system efficient and cool.
There is a square relation between motor torque and efficiency! The more torque you squeeze out of your motor, the worse things get! Its a steep square function curve! 
The gearing will boost your lower motor torque again, so you get the desired higher torque at the wheel.
The 1:3.9 gearing, using  83mm wheels is theory, since its hard to do that mechanically, using a belt drive. 
1:2.5 is more realistic. Knowing your gearing and your voltage, you can start to chose a motor with a KV, just enough to reach desired top speed. This way you keep the Amps flow as low as possible. This is good for the ESC and the battery. Low amp flow is what keeps your battery and ESC healthy over a long period of time.

Frank
```

---
