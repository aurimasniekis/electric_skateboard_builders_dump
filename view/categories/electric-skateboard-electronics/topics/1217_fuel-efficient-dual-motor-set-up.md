# Fuel efficient Dual motor set up?

### Replies: 7 Views: 2084

## \#1 Posted by: Nasty Posted at: 2016-02-04T01:39:29.842Z Reads: 125

```
First off, i am newbie to this whole skateboard/longboard world, so bare with me. Is there a way to have one of two motors turn on only when a certain torque is required? For example when taking off, both motors will operate(due to the load factor). But while coasting, the single motor will not operate, hence the lack of load. Also when approaching a hill, the extra load is sensed, kicking the additional motor on.... i don't know just a thought.

p.s. the only downside i see is when one motor is off, that can create drag/load. Remember im not sure what the vesc's are capable of...
```

---
## \#2 Posted by: onloop Posted at: 2016-02-04T02:23:45.443Z Reads: 120

```
I think it's definitely possible, but maybe over complicated without achieving much.

I suppose it all depends what your main objective is. I think in this case, to improve efficiency & also have the big torque you want, you should just use a big single motor such as a 6374 size motor. These big motors have lots of torque and can climb hills easily if they are fed enough power which you are controlling as the rider. They are also using less power when on the flats. Here is one for reference.

http://www.electric-skateboard.builders/uploads/db1493/original/1X/d13f42d6ada4a6aa74558808a807dc011b05bd62.jpg

What you are describing, regarding sensing increased load when starting to climb a hill, this sort of happens anyway. This is actually the job of the most motor controllers, as the load increases the motor controller will send more current until the load decreases or something burns.

In the case of the VESC you are actually controlling current (if you have that option selected) So as you reach the hill, to maintain your current speed you must increase the current to the motor which you will do by pushing the throttle.

If you have the VESC in Duty cycle mode the VESC will automatically increase current to maintain speed until it reaches its maximum set current or the load decreases.

Some of the new eboard remote controls on the market at the moment have cruise control, Once activated it will try to maintain your speed without the throttle being used. Soon I will test this feature using Current Control & Also Duty Cycle and see what has the most desirable results.
http://www.electric-skateboard.builders/uploads/db1493/original/2X/4/4b56f860aa5396ce345df3c1b35e404d364a0a1d.gif


Anyway... I think a single large motor will probably always be a better option for efficiency than two smaller motors. It is also cheaper & simpler to build.
```

---
## \#3 Posted by: NNGG Posted at: 2016-02-04T02:27:32.595Z Reads: 111

```
Thats why I went with a 149kv SK3 :)
```

---
## \#4 Posted by: Nasty Posted at: 2016-02-04T02:43:32.555Z Reads: 112

```
Makes sense,  and definitely over complicated :sweat_smile: thanks for reply.
```

---
## \#5 Posted by: lowGuido Posted at: 2016-02-04T09:37:46.380Z Reads: 94

```
I would almost always recommend a single motor, unless you absolutely NEED the hill climbing torque of a dual.
I must admit I love riding the dual because of the way it eats up hills.. but it also eats up a bit more battery.
I ride my single daily for a commuter, and the range advantage far outweighs the extra torque.
speaking of outweighs.. my single weighs so much less that the dual as an added benefit.

for what its woth this concept has been discussed here:
http://www.electric-skateboard.builders/t/switchable-dual-or-single-drive-boards/177
```

---
## \#6 Posted by: trbt555 Posted at: 2016-02-04T13:58:37.116Z Reads: 70

```
@lowGuido Could you estimate the % range decrease for a dual compared to a single drive ?
```

---
## \#7 Posted by: lowGuido Posted at: 2016-02-04T14:09:14.829Z Reads: 67

```
I get about 9km on dual and 13km on single. Same route, using zippy 5000's
```

---
