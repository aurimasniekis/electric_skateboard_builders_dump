# Vesc ideal battery amperage discussion

### Replies: 8 Views: 325

## \#1 Posted by: Lunasi Posted at: 2019-04-27T16:35:57.624Z Reads: 111

```
This actually came up as a discussion and I wanted to get the communities input. I was discussing batteries and vesc 6/ unity with a friend and got to the discussion of battery amps. My classic understanding when using a battery with a safer charge/discharge bms that has a set output of (for example) 60 battery amps is that when running two vescs you would split this battery amperage. For instance, because I am splitting the current coming from the battery to two vescs I would program each vesc at only 30 battery amps per motor versus 60 amps per motor.

Opposite to this is the Unity. My understanding, correct me if I'm wrong @Deodand is that part of the genius of the unity is that you figured out a way to take that one single current, not split it, but make it simultaneously fire left to right within milliseconds causing both motors to run and for my battery amperage to run at the full 60 battery amps per motor.

The debate here is that my friend claims you can just run two vescs at the full 60 amps per vesc and there is no reason to split them in the first place because they won't actually ever hit that amperage, but for me I was always told to halve the battery amperage per vesc. What do you all think?
```

---
## \#2 Posted by: Dirt_Bag Posted at: 2019-04-27T16:47:10.947Z Reads: 106

```
could you link me to the post that mentions the split power output? i would love to read more about it
```

---
## \#3 Posted by: JensSjogren Posted at: 2019-04-27T16:50:34.020Z Reads: 106

```
I don't know much about electronics (except common eskate stuff) but i wouldn't guess that the unity is doing this, would be amazing if it was possible though. 

Definitly split the batterys maximum rated amps between the ESCS, on my trampa for example i easily hit over 100 battery amps so i could not imagine that 60A is unreachable on street builds? 

And the argument that it's no reason to split the values because the system wont ever reach the maximum amparege anyways is just unvalid. When setting up the ESCS you still have to go through the process of setting your values, so why not set it to something that you know the system can actually handle. Further if you know the system wont reach set values, why would you set them in the first place.
```

---
## \#4 Posted by: Dirt_Bag Posted at: 2019-04-27T17:02:27.249Z Reads: 92

```
it seems impossible to gain more power from that though. surely splitting the power between motors will result .5x the power per motor? i need more info to understand this because right now i seems to be breaking the laws of physics.
```

---
## \#5 Posted by: AlanZhou Posted at: 2019-04-27T17:26:45.933Z Reads: 86

```
[quote="Dirt_Bag, post:4, topic:91963"]
surely splitting the power between motors will result .5x the power per motor?
[/quote]

i think what lunasi means is it applies full power to one motor and switches to the other in milliseconds? and it repeats this?
```

---
## \#6 Posted by: Lunasi Posted at: 2019-04-27T17:27:59.995Z Reads: 80

```
Correct @AlanZhou it's basically taking a single current and alternating sides it powers so fast its not noticeable
```

---
## \#7 Posted by: mynamesmatt Posted at: 2019-04-28T23:14:15.669Z Reads: 59

```
Idk about others but i basically have my discharge bms (80a) and set the battery max on each of my focboxs to 35a so i have a bit of leeway for my bms. then i just set the motor max according to how much acceleration i want. eg i have my motor max at 95a each side
```

---
## \#8 Posted by: Andy87 Posted at: 2019-04-29T06:08:32.327Z Reads: 52

```
[quote="Lunasi, post:1, topic:91963"]
60 battery amps is that when running two vescs you would split this battery amperage
[/quote]

that´s correct. you probably could set it even higher as your bms act like a fuse and shouldn´t cut off at a 1-4sec peak current which exceed the constant value at 10-20A. sure this depends on your riding as well. if you would do a hill climp and const draw 150% of the bms rating than better stay below the bms rating.

[quote="Lunasi, post:1, topic:91963"]
because I am splitting the current coming from the battery to two vescs I would program each vesc at only 30 **battery amps per motor versus 60 amps per motor**
[/quote]

and i think here the confusion starts. battery amps are not motor amps. your motor amps are not directly regulating your battery draw. it´s the batt max setting. you can run your motors with 80a and non the less only draw 50a from the battery. it´s the duty cycle.

I don´t have an unity so i would be glad if somebody correct me if i´m wrong in this point, but it´s just the bat max setting which is different at the unity.


to make it easy, two controller, two input cables, two points where the battery current is meausured, both parallel to the battery, means you need to split the bat max value, because of... because it´s like this in electrical circuits. If you would write a FW which add up the two values when the vescs connected via CAN bus than you could as well change the config template to set only one value for bat max. I don´t think this would be a good idea thou, but possible. 

unity, one input cable, one bat max value. how that is divided internally after idk. maybe there is just a parallel connection inside, but it doesn´t really matter. the value which regulates the draw from the battery is just measured before it is devided and good.
```

---
