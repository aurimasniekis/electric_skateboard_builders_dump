# Only one ESC powers on at a time

### Replies: 7 Views: 159

## \#1 Posted by: Jasonkimberson Posted at: 2019-03-30T05:59:26.044Z Reads: 40

```
![image|375x500](upload://5ClV8VNN6kxEwV4b0QvyWL5IyJc.jpeg) ![image|375x500](upload://rNFxqdJ3iP9dRALRLWipWwDGZpF.jpeg) 

I am currently trying to switch out two flipsky 4.12s out for dual focbox.  The problem I am having is only one focbox gets power once everything is plugged in. The y splitter seems to be fine since if I unplug the powered side the other focbox then gets power.

 The battery wire leading to the focboxes is a xt60 because the battery is a battery that was wired for xt60

Any suggestions welcome.
```

---
## \#2 Posted by: Andy87 Posted at: 2019-03-30T06:09:04.191Z Reads: 38

```
Do you plug in the focboxes one after each other?
On the first picture you have the CAN Bus connected. If you plug in the connections on the focboxes after each other you might already fried your communication port 😬
If you didn’t tried already, plug in the y split to both focboxes and than connect the plug of the y split to the battery
```

---
## \#3 Posted by: dareno Posted at: 2019-03-30T06:20:11.571Z Reads: 36

```
Can bus failures are a bit more total.  Dead.  nothing.  From what you have written @Jasonkimberson both vescs power up individually?

I would go back to the beginning.  Disconnect everything from the battery.  Disconnect the phase wiring and everything else.  Connect the canbus cable and the y split and then reconnect the battery and see what you get.  Let us know what lights are going/flashing etc.
```

---
## \#4 Posted by: Jasonkimberson Posted at: 2019-03-30T07:22:14.483Z Reads: 33

```
![image|375x500](upload://nzIkWWsKkanu07G8EznePWk2adn.jpeg) 

No flashing, if I only plug one in, they both run fine and spin the motors.  For this test I removed the canbus wire
```

---
## \#5 Posted by: Jasonkimberson Posted at: 2019-03-30T07:27:38.288Z Reads: 29

```
Your the man, I just reread your post and did what you recommended, seems like the sensors stopped them from working together.
```

---
## \#6 Posted by: dareno Posted at: 2019-03-30T07:27:52.181Z Reads: 29

```
Disconnect the motors and just have the vescs connected to the battery.  You know about can bus though right?  Never disconnect the canbus while the battery is connected?  Connect the canbus and then connect the battery to it and see what powers up when switched on.
```

---
## \#7 Posted by: dareno Posted at: 2019-03-30T07:33:09.769Z Reads: 27

```
All good mate.  Best way to trouble shoot is to start again.  The sensor cabling may be different between the focbox and the flipsky.  I'll pass you back to the man the myth the legend @Andy87

Actually interested to know how this can happen because I had a sensor pcb go on me and it killed a vesc.
```

---
