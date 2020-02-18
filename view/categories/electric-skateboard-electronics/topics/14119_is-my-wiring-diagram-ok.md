# Is my wiring diagram ok?

### Replies: 7 Views: 1008

## \#1 Posted by: gordy Posted at: 2016-12-03T13:32:54.657Z Reads: 100

```
http://www.gordyhand.co.uk/wp-content/uploads/2016/12/Skateboard-768x1024.png

I think that I've got the right idea on the wiring layout, but before I hook it all up I want to double check I have it correct.

I'm going for 2 4S 10,000mAh batteries connected together to provide 8S 10,000mAH.  I've got a loop key for safety and a single charging point with a 8s balance system.

I've got one batteries positive into the other batteries negative and then the other pos and neg provide the power.  

Any help or corrections will be greatly appreciated.
```

---
## \#2 Posted by: rpn314 Posted at: 2016-12-03T16:22:41.584Z Reads: 69

```
So if I'm understanding this correctly the loop turns the system completely on or off and the pwr is the charger input. With this wiring setup you'd need the loop key in to charge and so the VESC (and motor and receiver) would be powered whenever you're charging, which if that's what you wanted is fine. Just to be aware

What's the switch doing? And are you using an external balance charger or an internal BMS?
```

---
## \#3 Posted by: gordy Posted at: 2016-12-03T16:25:13.781Z Reads: 65

```
Thanks

If I have the VESC etc powered when charging is that a bad thing?  I could always put the loop key on the the other side I suppose.

The switch is just to turn the Voltage Alarm/Meter on/off to save battery.

I'm using an external balance charger that does 8S.
```

---
## \#4 Posted by: DilatedPupils Posted at: 2016-12-03T16:32:49.235Z Reads: 56

```
You have to be very careful plugging in the balance wires to the series connector.
```

---
## \#5 Posted by: gordy Posted at: 2016-12-03T17:04:19.611Z Reads: 51

```
I intend to have them permanently wired into place.  I will be making the cable loom myself and double checking the order of cables etc!
```

---
## \#6 Posted by: rpn314 Posted at: 2016-12-03T18:45:07.213Z Reads: 48

```
[quote="gordy, post:3, topic:14119"]
If I have the VESC etc powered when charging is that a bad thing?  I could always put the loop key on the the other side I suppose.
[/quote]

I wouldn't say it's a "bad thing", I just probably wouldn't do it :slight_smile:
As in I don't think it will cause damage to any components, but it could create interesting situations like where you accidentally bump the remote while it's charging and it takes off across the room (and then possibly breaks something, itself or otherwise). My philosophy is only have it on when you're actively using it and paying attention to it. We build these boards with a lot of power and they can cause some serious damage if we're not paying attention to them.
```

---
## \#7 Posted by: gordy Posted at: 2016-12-03T18:49:21.006Z Reads: 40

```
Yeah that is very good advice. Thanks I will rethink the layout.
```

---
