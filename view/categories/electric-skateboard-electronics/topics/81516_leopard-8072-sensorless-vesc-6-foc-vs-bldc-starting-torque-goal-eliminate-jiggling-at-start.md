# Leopard 8072 Sensorless / VESC 6 / Foc VS BLDC / Starting Torque / GOAL: Eliminate Jiggling at start

### Replies: 6 Views: 472

## \#1 Posted by: Carlo Posted at: 2019-01-20T16:56:22.649Z Reads: 110

```
Hi there. Yes new tread about Foc vs Bldc. But Wait ….

GOAL of this tread is to find the best start torque with minimal motor jiggling.

Going through all the discussions, they all very general. I mean the discussions mix too many factors. The only way is to skin it down to a specific setup and discuss it. This may then help for other setups too. So let us talk about above setup. Hopefully I am not the only one with above.

Alright, setup like above, I have tried both FOC and BLDC:
I found that BLDC mode gives me more starting torque. It rattles and jiggles but when I pull the trigger through and give it a little hip swing, it goes.

When I use Foc with sensorless, the starting torque is about 50% of BLDC.
I cant comment on jiggling cause that just doesn't get me going at all, so I did not bother to try.

The way I tested the difference: Board on the bench, holding the motors with my hand, and pull the trigger. This lead me to above conclusion.

Have to add, that I tried FOC once outside a while ago and got same result. 

Let me know if you have any suggestions to reduce jiggling and increase torque.
```

---
## \#2 Posted by: briman05 Posted at: 2019-01-20T17:02:54.465Z Reads: 107

```
The motors don’t get you going because you need a sensored motor to start from a stand still. Sensorless motors need a small push start to go.
```

---
## \#3 Posted by: Bjork3n Posted at: 2019-01-20T17:17:39.442Z Reads: 101

```
From what i understand FOC has better torque on low rpm compared to bldc.
I run foc with sensors and its butterysmooth from 0-100% throttle.
I think you might have something wrong with your settings.

I think there are a setting called start up boost than can help you increase the start torque.
```

---
## \#4 Posted by: Andy87 Posted at: 2019-01-20T17:27:52.507Z Reads: 94

```
It’s not what you asked about, but maybe it is an option for you to upgrade with an AS5047 Encoder?
Better take off you will not get.
```

---
## \#5 Posted by: Carlo Posted at: 2019-01-20T17:30:42.691Z Reads: 87

```
Right, I agree. For a smooth start-up sensor is better. I use sensored too and its really nice.

However, I would like to come near to the best possible without sensor and 8072 motor.

So I wonder what setup in the VESC Tool would be best. I will post mine shortly with an little vid I will do this afternoon to show the jiggling. They already pretty good. 

So maybe someone has better specs for that.
```

---
## \#6 Posted by: Pedrodemio Posted at: 2019-01-20T18:00:57.747Z Reads: 78

```
The main difference between startup in BLDC vs FOC is that BLDC injects a high frequency current that is used to determine the rotor position without actually having sensore and having a smooth start, while FOC sort off ignores the rotor position and just rotates the magnetic filed and hopes that the magnets follow it until the speed generates a high enough back EMF for the position to be determined 

Vedder said somewhere in his forum that he would add high frequency injection to FOC sometime, that should make the startup of both really similar 

That being said adding sensors to my motors was the best thing I did to my board, smooth as hell, can start going backwards and in steep hills
```

---
