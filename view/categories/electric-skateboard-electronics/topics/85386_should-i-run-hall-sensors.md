# Should I run Hall Sensors?

### Replies: 7 Views: 396

## \#1 Posted by: badger4life Posted at: 2019-02-25T18:56:42.988Z Reads: 110

```
First I'd like to thank everyone here for helping me so much with my first eSk8 build.


My board is set up with dual Torque Boards 6355 motors which come with Hall Sensor wires.  However, the site I bought them from has this statement: "Motor can be used with or without a sensor. Sensorless operation is most common."  I've been ridding my board without the Hall Sensor wires hooked up for about a month now and I keep wondering if I should have bought the correct adapter to connect the sensors to my VESC.

I've done some research on what Hall Sensors are and it seems like something that would be good, but I keep coming back to that statement that says sensorless is the most common way to run the motors.  Any info to help me decide if I should run with or without sensors would be great.  

Thanks!
```

---
## \#2 Posted by: Acido Posted at: 2019-02-25T19:08:12.402Z Reads: 104

```
Usually if people have sensors they use them, you get a much better slow start and a quieter motor
```

---
## \#3 Posted by: butt_stallion Posted at: 2019-02-25T19:16:52.466Z Reads: 103

```
You could run it in Hybrid mode with the VESC this will allow the motor to utilize the hall sensors at lower erpms for slow starts but then it shuts off at a predeterrmined ermp.  It's usually the most efficient this way.

Edit: I run mine on hybrid and it works like a dream.  I can come to a complete stop on a hill and there's no stuttering at high speeds
```

---
## \#4 Posted by: Mikenopolis Posted at: 2019-02-25T19:17:57.445Z Reads: 102

```
I mostly go sensorless because I'm used to it. I ran sensored on my Carvon SD build for a bit and LOVED how smooth and quiet it was.

The only issue I see with sensored is those damn wires being so tiny and might have a higher potential of breakage?
```

---
## \#5 Posted by: ZachTetra Posted at: 2019-02-25T19:28:36.916Z Reads: 93

```
Is there a situation where sensors are not recommended?  I'm getting a set of dual hubs and a non programable ESC and I'm not sure if it's worth using
```

---
## \#6 Posted by: badger4life Posted at: 2019-02-25T20:09:30.065Z Reads: 76

```
So far it sounds like it's better to run with Hall Sensors.  I'm just confused as to why the site I bought them from says the motors are normally run sensorless.
```

---
## \#7 Posted by: rusins Posted at: 2019-02-25T20:48:02.471Z Reads: 63

```
Some ESCs might not have sensor wire connectors. That description was written quite a while ago, things have changed a lot. I'm pretty sure there are 0 downsides to using Hall sensors if your motor has them.
```

---
