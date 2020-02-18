# 2 motors, same kv, same size, different max wattage - how does this work?

### Replies: 5 Views: 590

## \#1 Posted by: accrobrandon Posted at: 2018-08-07T19:04:01.233Z Reads: 130

```
i was commenting on a different topic and wasnt actually sure how this is possible and would like to understand it better. 

Using meepo hubs vs diyeboard hubs as the main example how can 2 similar motors have a different max wattage.

does it have to do with the thickness of the copper wound around the stator?

thanks just trying to understand this area a bit more.

https://www.electric-skateboard.builders/t/curious-about-amperage-draw-of-500watt-diyeboard-hub-motors/64055/3?u=accrobrandon
```

---
## \#2 Posted by: DeathCookies Posted at: 2018-08-07T19:43:58.114Z Reads: 113

```
The Motors are not exactly the same.
First they probably have slightly different kvs and secondly different free rolling resistance which sums up.
```

---
## \#3 Posted by: professor_shartsis Posted at: 2018-08-07T23:05:57.973Z Reads: 95

```
[quote="accrobrandon, post:1, topic:64160"]
Using meepo hubs vs diyeboard hubs as the main example how can 2 similar motors have a different max wattage.

does it have to do with the thickness of the copper wound around the stator?

thanks just trying to understand this area a bit more.
[/quote]

take 4 identical motors, except for the windings...same stators, magnets, cans, etc.

let's suppose the first motor has 10 turns of wire per tooth and is measured at 100kv.

suppose the second motor also has 10 turns of wire per tooth, but the wire is thinner (half the cross section area). the second motor will also be 100kv (same # turns), but the electrical resistance would be doubled (thinner wire). the same amount of motor current produces twice as many watts of ohmic heating in this motor, but this motor has the same torque per amp and same maximum rpm per volt as the first motor.

suppose a third motor has only 5 turns of wire (same gauge/thickness wire as the first motor)... this motor will be 200kv (changes in kv are inversely proportional to changes in turns) and have half the electrical resistance as the first motor (half length wires). this motor only has half as much copper volume as the first motor, half the torque per amp & double the maximum rpm per volt as the first motor.

suppose a fourth motor has 5 turns of wire (200kv), but the wire has twice the cross section area as the first motor, and therefore the same copper volume as the first motor... this motor will also be 200kv, and will have 1/4 the electrical resistance as the first motor (half length, double thickness), and same KM (size constant) as the first motor. this motor will have half the torque per amp but double the maximum rpm per volt as the first motor.

the "maximum wattage" is a suggestion from the manufacturer to avoid overheating.
```

---
## \#4 Posted by: accrobrandon Posted at: 2018-08-09T03:57:09.764Z Reads: 70

```
thank u for a complete response.... so we would say the first motor would be the 500w in reference and motor 2 would be the 250w with same turns but thinner wire having double the resistance or half the max wattage?? even tho its a manufacturer suggestion...
```

---
## \#5 Posted by: professor_shartsis Posted at: 2018-08-09T04:12:11.429Z Reads: 67

```
here's what happens when you double the resistance with the same KV during full throttle acceleration...

efficiency goes down (green line, top left chart), ohmic motor heating doubles (90w -> 180w), battery amps increase (black line, bottom right chart), acceleration remains identical, top speed is nearly identical.

(50v battery, 0.025ohm vs 0.050ohm, 100kv, 100mm tires, 1:1 gearing, 100% throttle, %95 max duty cycle, 60a motor current limit, 60a battery current limit per motor)

https://image.ibb.co/gAWwFp/0_025_vs_0_050.gif
```

---
