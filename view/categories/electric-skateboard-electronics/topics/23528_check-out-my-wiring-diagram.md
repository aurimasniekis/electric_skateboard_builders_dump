# Check out my Wiring Diagram

### Replies: 9 Views: 955

## \#1 Posted by: jkrider Posted at: 2017-05-20T05:03:40.554Z Reads: 143

```
I need some assistance. Can you guys check if everything is correct with my wiring diagram? I had the most difficulty learning what to do with the balance wires. Also I'm wondering if the volt/battery meter can be placed somewhere else in the diagram. I'm also having a dilemma between installing a power switch vs an anti-spark key. What do you guys think?
Any help is appreciated! 

<img src="/uploads/db1493/original/3X/0/7/070129d52c836ae5e41c2e217ef41e033915d1f3.jpg" width="375" height="500">
```

---
## \#2 Posted by: lowGuido Posted at: 2017-05-20T11:14:16.912Z Reads: 118

```
looks good to me..
personaly I would use a loop key over a FET switch, but its personal preference.
```

---
## \#3 Posted by: Shahar9320 Posted at: 2017-07-02T13:30:15.903Z Reads: 103

```
Looks great but I didn't understand why are you connecting the 2 balance wires. And how did you do it?
```

---
## \#4 Posted by: jkrider Posted at: 2017-07-03T00:01:24.983Z Reads: 95

```
So I connected the 2 batteries into a series through the bullet connectors (red and black wires on top of the batteries). I also need to connect the balance wires into "series". The red balance wire on the left battery is attached to its last cell, right. So that red wire needs to be connected to the negative/black balance wire to create:
[ black/negative - 1 - 2 - 3 - 4 - 5 - 6 - 7 - 8 - red/positive ]
I'm sorry if this did not clear things up. I just followed all the diagrams on here and created my own version of it. I've connected all my electronics and they seem to be working so I'm trusting my diagram lol.
```

---
## \#5 Posted by: Customesk8 Posted at: 2019-01-01T10:27:43.932Z Reads: 48

```
@jkrider  how did you connect the volt meter at that point of the xt-90 just solder it on aswell as the main wires?
```

---
## \#6 Posted by: jkrider Posted at: 2019-01-03T06:45:48.715Z Reads: 40

```
Yup, they are just soldered together.
```

---
## \#7 Posted by: Customesk8 Posted at: 2019-01-03T07:10:00.455Z Reads: 40

```
![image|375x500](upload://vhjRIOkDUD73WJ39ERVno69KAgm.jpeg) 

Is there any reason I can't put the anti-spark in-between the vesc. (red arrows) 

and the volt meter where the blue arrow is (with bullet connectors) directly to the batteries
```

---
## \#8 Posted by: TowerCrisis Posted at: 2019-01-03T09:05:14.137Z Reads: 36

```
You wouldn't particularly want to because the voltage meter will continually drain your battery if you do that.

Of course you can do the math and measure how much current it draws and see how long it would take to deplete your battery.
```

---
## \#9 Posted by: b264 Posted at: 2019-01-03T09:28:47.374Z Reads: 36

```
If you're running through the BMS like that it should be safe to do that.  If you're bypassing the BMS "Charge Only" then you cannot do that.  This diagram is discharging through the BMS.

I would not connect the negative-most balance wire of the positive-most battery though.  Leave that one unhooked.  Also connect them in this order on the BMS:  B-, balance leads for more-negative battery, balance leads for more-positive battery.  Unless they are on the same connector, then B-, balance leads in that order.

Make sure you put [a fuse](https://www.mouser.com/ProductDetail/576-099707.5WXN) in series with your charge port, between it and P-
```

---
